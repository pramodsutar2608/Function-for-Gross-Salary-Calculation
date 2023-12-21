# Function-for-Gross-Salary-Calculation

Gross Salary Calculator

--------GROSS SALARY CALCULATION-----------    
--------------------------------------------------------------------------------
Write a PLSQL stored function for passing empno as parameter return gross salary
from emp table based on following condition:
gross:=sal+hra+da-pf

hra-->10% of sal
da-->20% of sal
pf-->10% of sal

----------------
create or replace function f1(p_empno number)
return number
is
v_sal number(10);
hra number(10);
da number(10);
pf number(10);
gross number(10);
begin
select sal into v_sal from emp1
where empno=p_empno;

hra:=0.1*v_sal;
da:=0.20*v_sal;
pf:=0.10*v_sal;

gross:=v_sal+hra+da-pf;

return gross;
end;

-------------
select * from emp1;

select f1(7902) from dual;
