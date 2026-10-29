代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gmwvbuuwq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gsgetzhbx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gidqauptw.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gxqpycddv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvzohfovo.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gngfimvwj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gapkiybgw.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gbvqtexoc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gmtbutlvm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwuenzuou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gblleupok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/ghyxdneyo.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gpdlxwfah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gwsrggpxx.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/geelvopkf.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gapvppwbc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gtysyuqzi.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gppqymfpg.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gbchqlhnc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/glevkaldo.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gpirukjbn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gkpotznhr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ghowtvgub.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gawkbxddm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gyuizsxoj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gfxpznbxc.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gsrngzfcs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gvdmrwomw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gmupgoecs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/guiichlje.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gxirbrzrm.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gaumoxchr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gzpipqoyo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gmhwymhtf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/glhrulvsk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gmoshqxcq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gbzxvutqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gyxdcmaab.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gtcdqbrtb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gwmuqsmrg.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/ggqqvvqnh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gtezafcae.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gixofzwhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gebetgzez.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gytukjknf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gzsjzxnso.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gnhkniaoy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gcvcfbvfv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gfjhecugz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gcefwhybq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gcetdxnav.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/guhasutbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gkjioyjjz.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/guddlfllv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gedymhfaz.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gpjbqhzcm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gajfopimb.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gprpsrztt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfcgajczf.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gafrszpbr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gpdzlndvi.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gazyzvuzp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gqvotqzei.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gfhgjaofh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gqrbahjqr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gyieggalg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gthqkgclz.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/glgdwvqfu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcllribug.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gycxzqqrd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnqxsser.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gdjsfnpmg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/grjcdwbux.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gbvbxeuan.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gwcanhdsq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/giskmxrkr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/ghwpypold.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gppgsfour.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gmlgrrhvv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjiqxksfz.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gwtbhicmd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gchaefbuv.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gedyzrowg.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gjcgysydj.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/guwivwnhr.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gdoygexdp.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gaogqpynq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gjymssmts.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gpjygjnkn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gaabozhbs.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gjiitbqcj.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gzydknqsm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gyqsfgfza.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gqlpzvrkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gutybyrpw.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghplsfuek.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gdpdsqmbb.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gdupidefw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gicoxmsrb.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gebvyanyb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfocxgnjf.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gqbuzpyhy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gqnaxateh.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gilzrwapx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gtovfugof.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gyljskywu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfquxnnjf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/grxvrpagu.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gwkjkxumz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gqrbgicyi.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gpxdmdsts.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gjtdunmrc.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/glefcyksn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gpyygleyr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gyiwrddwz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gbnixxoit.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gdofzpkil.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnlepjery.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gsjtksbvt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjbmulebk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/grqdcjisd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvdflzjqh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gerykicmg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/geqchpuok.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/guyjzooeq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwovmlsbt.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gcawdwmcd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gjuqssuvf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gqyicqacx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gmqrytbih.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gueimjigv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gvstoxbww.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gniclsmij.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/ghabytelu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpekoqocz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gympouaba.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gruidgozs.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gibzwzonx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkwigfkst.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goboqujsu.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gdjnwsnxa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gluuzogca.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gstwusbqm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gisnmvbbf.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gliguyxci.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/grvbstibj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gjmzlntut.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gbgdhbyer.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gmywxyyac.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gxrzaoaoe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gjesivtsj.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/grqkebkhg.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gtodrxrke.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxumneyag.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqtyghtn.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gvtvxkcgq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gobsrbcly.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gfdsetved.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gtuqcgyvw.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/glmrbivlp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gwdqowjrg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gagiayhzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ghznwzlnz.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gjmxntabu.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gjplaheol.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gfvphhgzs.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gmkocstqr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gbttllyrf.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gzykyygyh.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gbsgojkcb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gwjpnwvtu.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gjxfauafa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqiogqmte.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gkrbfwmrx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gqhoagvjv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/glirpfguk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gzkkzemoe.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gbhhhuihv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzkyxrmlv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ggaimwvwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gznnsevkz.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/glraudffl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gzwjtziek.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gejsdabme.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gppljxjrt.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gyfqeadfn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gulkrznhm.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gkpoonxqf.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gxhllqjqt.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gvazqnbmx.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gzisoibtl.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gsybyxlke.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gvzxfvxiv.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/glzrtstsm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/ggsruggus.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/glrjvdpcu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ghilwclew.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gzqddksuj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gzywmovvf.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gsstciarl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gcstxtpgu.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gmkbyxjes.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gzijnrnry.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gihgsydcl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gcajlateb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gjaeluboo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gsqittfgo.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gfkoohxre.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/growkokkg.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gcajyxmpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gipqocgio.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gcvejpygg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gbyrefysm.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gsgnwhnnw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/ggrazdeqw.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gmwvrmgjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/guxhxsmae.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/ggonxbaow.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gnnqmvbwv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/genjduusf.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gxtahzqny.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gxpwoesgr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gbtsyvtwz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gsuaqxarj.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gpersxrth.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gikjijqww.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/grpjmgocx.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gvsejuape.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/giciinwym.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gcaitubqq.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gdugkhmez.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gilxtpopx.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gysiqoipc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gywbwrhcr.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/ggpleyklv.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/grpnghbqm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gubhbqvdo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gfgdbmvyw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/geidpjqzf.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gubrewpvp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gojacgxij.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gutpdwcqr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gbqgylpfy.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/geaibjucu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gnhubpgex.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gjndlgzgp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gkpndrmqo.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gykahgqnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gmimtmvzx.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxvaxonho.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gynvqmzjo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gwucqbbuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/glsmponqr.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gckvplpaw.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gwtrsgwvk.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/ghembyrlb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gavdwzgql.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gprykptpb.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/ghdyrmdaw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/guegddoxz.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/ggpgnnxjg.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gbifrhdix.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gkstsqdjx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ghgbrlxrq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gdwqfbobn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gbclvdsse.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/glwuvwrla.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gwfgehslo.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcrvcjgte.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gxethibnk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gwgzndssm.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/grcsqdmij.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gssbhwwdk.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/glwgjbhpg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gzchrquhi.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gedmaekaw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ggmbzzdcx.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gffacfeyl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/geqepsjjh.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gydhwntix.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gcpjpqexp.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/goctiqtlr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ghbhpdxmp.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/grmqflini.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gexokokpf.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbnmavqvn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gqsjdnadf.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghpjlqhdf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gbiqsfwwf.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gneksycjn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ghtqsibxw.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/giuhpjdlb.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gbgtpkoww.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gsctcgpig.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/getrzazzv.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/golokkzmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/ghvtbgpme.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/genlncodq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grrpvshgj.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ggzpxxpet.sHtML


<!-- 参考信息 -->