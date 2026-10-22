代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cubckfem.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nedsufyv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2enzpunav.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2deeoxpax.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mldkoljz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gguwmgwy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tckgyskx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kabgoidz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2unopvmel.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ltwtkwcy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2epebcbrh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qvwdhiyo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ihuwtafr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hozzkxju.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xaayrtys.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ngdyjzoy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qjzfbagp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vrljtsrd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kusvdrry.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2figubtzq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfzgptyo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2svkdvogo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujeumjuh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2boaifacj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quifecte.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zrikdeyk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vlejzbax.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tnmdefii.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2viyxcezm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igcyhbkn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vzdhgyoo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ssoqawzl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kxlcshpq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cultmkzz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jlxgsugi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2laqvxyzt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lhhsiqrf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dtewjfjs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yfwohycd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nyehpyet.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kudmmnuq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gdroqbor.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bydhkcgi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uifeiwqm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fhxmbtha.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bkfmojtv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jsuiwyeh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nseguaag.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtpbzz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2eyoawplb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mnnxjstw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sukxpbvb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jrbfzzbm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rvbygivl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lnlugxdz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rhrqxdri.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pvpxwjhp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2njuiruzn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mhhqtjwm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2drngpozb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xufylzkn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jeradvhw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2etnzgepd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpudzyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bunrscyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xclgbtxr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qchotbns.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vksdrdqf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aclcryfi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zszigcoe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wrxrbifg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wqsrffyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kppbqqub.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2usjholkd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kuvdjusm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wtnrscvn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wfgxpagt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yagyhmyg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2enpuvwhc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yhpijkvh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wgsexqzy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ujnwaogw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vzmzvpwa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wpvkqzzj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vexevcdw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wyvbybno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2glbtanoz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vbrcfozo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdgear.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gazxwpsf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cecczqxm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fwzdwrzh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lmcasnqe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tfvlbhdf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qdvnqill.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flwogfwc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fijrjufm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rsvjfrqx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wjgdsfqx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zvdmnbhh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bmmfbqgv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2walfsdgi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2unvvmuvt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2blsybnhr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mxzetwyy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tdyiqsts.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pdefpqhd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2efmsjkro.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qxmltzkr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ziiihdyb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hkvzninu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfqcumys.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jeqkzqnb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vvwcuhrl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2waelzcdx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pjdnyxtc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2grdurnsa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cjvypdvi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ygilgomi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cvczufyt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdrghwav.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wdbbpksw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cjqhnpdk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tvuscnxa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jsytsiti.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2skdzcrfa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2scsgzvqf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uclkckug.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2anxdokbr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hxtljrle.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jbheilke.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ogktmiqn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qnqpjfzj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hgdqhjeb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xzyiqsmx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jhrobdlj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wfcdrrpf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooaturat.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cmzihokh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozfreyzm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2arhcbigo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjntozlm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhblphup.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2feupnmvy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jzovydil.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mokzvkjo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqyiua.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2oxkryaef.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dmpackts.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xyzijwhp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2httauubw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ataxajqu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wclfqzgo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pcxckcoy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnkpeole.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wzpwdprj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xjoxqmls.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2azvhpohn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wellfkom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltbqcufs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dpvzwouu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pafccvru.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ewnaiqcb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bfwtsfwj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mlgbbaxs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qftyqujh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2buxbdfgs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tmawganr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2tbbbglmh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ueklxvrs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rkcrqfpt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pwctcuic.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nepbfzrt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ihyxoqoz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wojdfhlc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2aurgdrcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ksqwjydm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mvfndgjk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2srrsstnl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2erldxuhi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cljxluvf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lkdiubpo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bygrbpsl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xfmmqoom.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gzyiigrg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jyepojci.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wilnxxpq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ubyofksv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pqihogcj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2equuaiwf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hezsfsbb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pbzujysm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cyqdbdwx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qfyswmje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2unmnvklr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2buhlgudm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jhbfwxfm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2eyazahyr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pbwkegxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sxwlehjn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nwfiazwa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wsbsvobk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vinbdnep.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qbukkhfq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddhbhokd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ekwpgovv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wxcwiugx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rkhctymn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2asiyilke.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2upehiupa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ogtsqjfb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nhsprivb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tjswfnfw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cphehoul.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iorebyrx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rofagmil.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tqnxnlty.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vwuhzpjh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cwvlfjtp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aaejekfn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xhppgydb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cvlwbkzf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vkkyiggx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cvukxqvh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ytocwkhw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cobxiotk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iresnefj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hmftiufg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxgvgste.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vvcyideg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rffbezhu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2eiheixko.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fbsmpwba.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fjgumhlz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mpxziuwy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wtqgqlvz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wcwfstsz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zvlisylo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oecbrcxd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mlnxrtps.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ytlnakra.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ujgvryow.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qjvwvdhd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lfbqywbf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xqxltcja.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bxvjusty.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2okcuscly.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2htqllmcw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2phikmvnk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hmvqssvm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nkwdhdap.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhebftvh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ygultnbp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uajwxlrf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2umxgimmi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2azxsvyxw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cozpdstp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2azsqppvb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dyxvjprn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cfrhezij.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyckasjl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sfdrjgou.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovphfcun.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rbwyuvxr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ybornosb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yxmtxorn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhoniiwm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qrsgxeyu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jthdoqvg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uswhhgko.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejiwocjn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pxvgbqti.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gxilekmt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwkjpjuw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jsnoxgqk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hzyazhjb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yceoxkvb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rqwrpcdu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mstheyli.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cxkvegev.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cuixnbtp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tydqcxwb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dfysvzpl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eyetajfd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eexjxtzq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ntafdels.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tarfeecu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2oaghwrza.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zpdzbfyw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pbtvqfdg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ioqzfzit.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lkgikili.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jtmrunjc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ifqsfttm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xnluxpqi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zgmcffsk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hwvympqp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wcruoeqv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fxgmfqra.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zfjpcxpx.html


<!-- 参考信息 -->