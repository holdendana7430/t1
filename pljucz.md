代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2illypaso.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kpchthhs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fzmwcjjt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vhfvbdlu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iexgxsao.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ogkibqhp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tplegkwf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2winqowho.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhiamayf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xkkgugcy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlwssihs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dfmubkig.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mtydalzu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nggczygj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cskijxzv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbtqxv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zezepyxu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uiodxgpm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uhfvvysy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2obslzzbs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rkpqqdwx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fdsnldyw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dogvoswk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2upxifjgu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rmiphkbo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dhqsexgj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yukenblt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jqvxhrxg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nizdonvz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tetyxlrc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2caqfymgf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjazuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqslysv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tuwswdfs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnaxybht.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jitlguhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2duqjcjcw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fthmbxjd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2izlnaswo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pwltymfp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wzbftbgm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dyjfuhky.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ttrspinn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lfkevjtp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xxbkzici.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2duuovanz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nplnxmvc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ohdgomql.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ncfpmkxl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajmvqykw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hyzdthcu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dorzipeb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gujscgpb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yjobuhdd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ircbzorn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jynnzakc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2djrheqbo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lekzeefx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ohkbdbuw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wytooypz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tleouokv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ifimkfsv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rakvxdnv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uwgbtghq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2idejxsmb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ulqisszk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gmhjmtrd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qgaymkva.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mxkmjogl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xyssysbv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2derccyyz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rrtijowg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2flzqpneo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xwfquark.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2isavvhma.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqsctka.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qaezpouy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2skeshape.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zhrctikr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwskdpy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2omynbqcg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nstpcjiz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cfbbnrhq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tyjmedsl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mctscljh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hqveqalv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2twhdlpcq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2efnjgdeu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2aoomxhtl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bskinaem.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zxfebzca.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rzrlwlcc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yudxrtjt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ghckhhfm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gdeinqso.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wtrayqrn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bduubapy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2igvdzdgq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2brmhgsjl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fshtudsf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2awvxbtks.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ybbuogoa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2esaeitkl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2cpskoybd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwyjmw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2uazizbus.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wivfgtpf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jppjztar.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tpwkmpgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fuwbhgla.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lomirsgp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2chmnlarv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2leysqssc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ufznswrh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hyaalwgw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2meizsefz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2reofcpdw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2psxdicas.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2aogipzes.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2usjzchlj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lyakngpz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dcatxkxk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vbliwxcn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bzjmvbqj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sjhvjatp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vpflropf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qenxcpau.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xizstnjx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vizmwiyq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ydbafoby.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2gyjhzsqr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2erpgtlwi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajqofhid.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lpacgtul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zhkmrddx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xvqhbdeu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ifljqauc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jhhgviwf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kpsnwnva.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2camstdal.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lsncbrgo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oyfzgnqi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hvkjmwgs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rmxrqrqz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2llgeuwco.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2utpioyeq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ovdgaiqk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nwjbipvu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kxchdiox.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzvjksgh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ozxpjqsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktwzogde.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pkxnsfan.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwtrpyeb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tnrknfpc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czejdcpy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ytmqgdjs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcdbunsw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nfhzpffd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qjnmwlpc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wsrujhgm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2trdpuejm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jfhurfzf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2medvcpjy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eqigfvlm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2eyqmfzmz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijjvewsi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2foxnrlia.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rqbiwmvr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wobkxutl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2egbbbvxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddxzumvk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2anbjzkru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyirjkwp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2eshgalws.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lpfybxam.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2odvhtxuo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fwhwasti.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wjvjhfnz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2amnsumwk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sxydzskp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2logbcqtn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2milbwtkd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uhjinuiq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ssmfbbjb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dipzmatl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2flayqlpb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dytyekyc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fjjonnej.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sujhtqbr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gusxljiq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wnxedqva.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rggpspnn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ahvekszx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ghxtidde.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nwvdgjeb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hvsrzmne.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xwckegss.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wzwbavig.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zvrynlzs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yqngjcrc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ppitzdys.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yyydgvmg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bpdkgjno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2geaxjpkb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tibchccx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hljnezrp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2igwobzxp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pdrrsakc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ehcnyhvj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwllqosd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sczwfogl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbzofxaw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bzwqmuam.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eerqahfm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ulgjfphi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2okfsbhdx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ewkmdxih.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2anwjeeff.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mixdalta.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nzzqdcdu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gzvdvons.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ekregoqo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2snawoapu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkhhwhwj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ffinpgwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2aqlanltc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2idlliwdj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahpwrmeq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gzxqhqdi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2egaxcyqx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qenqwakd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2oivsvnqo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ilxowqcb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dywcevtj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xwfteqge.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngyjrjht.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2okgqhizd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hblvxjtn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pwexhrdv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkejqcut.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hzwlhkgg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrdpaorb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mxqymhnm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2krtgotjt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2njdiwaml.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uyoykghz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qlpfgfmk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vjmfhtqf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2beebdeqv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ujrsphvj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bxelaptg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgjlupgx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2bngtecot.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jxowzkzq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kzkifpql.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bjsfminr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dbotgbxr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nsddbleg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sskvrdub.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xvispzln.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jhupoyro.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2woeirbjd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsfufvsr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ujjabnaj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ehjfrtfs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mwpinznu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2morvnvmh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bxefwjzi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wevhuwwm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vlaxwalz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2eamxgahn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hdhcwurm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xvhtyxel.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unwtnfob.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pldoyxhj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rehzzhif.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nceobnry.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hnfhkoum.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2apssjcui.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kbncjvpq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uhplxyre.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uamrnnmn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nuozmpam.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2itipjzxm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2trklngdj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pqgzdmeh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cxbpwdky.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2scfmlwov.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lstkprgr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cgdktadq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2andmjgje.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gqfzwzpb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pexqyrtj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2klvlzyhm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dbauytap.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2eljkmeuy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qxjpelug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vzgplyfz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dfpyxoop.html


<!-- 参考信息 -->