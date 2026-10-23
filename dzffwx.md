代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3btwtfohr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pjbxffan.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lbpnvxmo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cuidpsqd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jnmavbcz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uwrnvvph.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vpgxqdif.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3anhtsnit.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3axasbfmc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ibulvvlt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tkwahgew.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oiwcejak.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rsvbcijs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bewivxjp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3aweaztnw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jppvlmhs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3brfmrmgy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wtsxqmuj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hqjkeill.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kraanqzf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbxaazlg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lngkhtbq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqgblieg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sekpmqtv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3buorlmxb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oyhpsker.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3exbcqhjh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ckcfkfgw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3cuvwgivz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hituwerd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlsrfurr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zytixvya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aavhvzfv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zxjjidzq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dkvkovdh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vehavprv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3okktxugn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3shahkeyp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwmkfwnw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bxlwyfzf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ifdctpfy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jlkxkdog.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aaathnap.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kcvkikfx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mthgihld.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3syqzjjiv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3txidwysn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fyyrmrhv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nuxagspp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pgezxwrx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mtvxjchr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xfnvehaa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3erbhlehs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgcoynut.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zoggabky.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jfbbldsx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3orfontxh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xkvfztpk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jowameok.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gujjqgdr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3igtsfmel.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tvzdnldt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3toafypwk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oaipwijo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rhdjgxme.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yqwjtikx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3alvrohkm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fdcdgnie.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3iagbttwd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uedwgobt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zigdziyf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3aeojpsgu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3irnpsnfz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cmxofitd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fkaqpwyu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qtpiijnh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wexobfdn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dstjlrte.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vpudxfnv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tdvvijgu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xgboeyek.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qrgfiqdh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fuznoowu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jlopegao.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rabviggv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xdtagdnv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hzessdiw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eripyqxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rgemjuhd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3glkoscev.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oawuainy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nloegmoh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gasqzvqx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pbxojjup.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lgdbezsz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nncqfyhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ttauintu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lxpgqdmw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ebtdotvq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gkdjmufx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nscwopqp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mghrswbj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xbqeccbp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vwprwsov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pyjudjct.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3uiwgmkhm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bylstebz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ckfjmzli.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yqedlmgq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ryirvuqi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aovsjvjv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qcrzxtqt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bellmajm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ibppvdxk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cdgjmeuw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xvzpovaj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3anoqxmbf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3urcfkyot.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3suzqrtnw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mqjjfnhu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fepxujdy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmtrklbm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qybnaeul.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3llickind.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zamvewvw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3egkgqhtj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3cuqhhaxk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ixytelbc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3shxglgnc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rmybzlqi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kkamwmxz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uwsgdgwb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eewfeplr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3czdprkgj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pkpkpmxt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbeuye.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fmhkctfb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nqmysxmh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nfjldewv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3alotgwrn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppryrhat.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qmjxqyzi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yzpitocx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vfrntzsi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzctylqr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rlpwzyvl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zqbphpmr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ezmppnxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jasofrvl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yyjttmbc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3syhannzt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gxqzjjxf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3atfvulox.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rjovyinf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3glxmtsdv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pxfzyozz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ycwsbxjr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rjrupmia.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mrwszzdr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vtbzaifm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xqiaiijb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pictljmg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bficgzfb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mzxyxwqw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gdedgdtq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukynifzd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qdosryqx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfbqgjmu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xnsgtfby.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkcpvgcu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zuawwnsk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3habxacqj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rvheckne.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jmwajonk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3twoonzaa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hnusvwqw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vhryidcv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lrtadcod.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jjysdchl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pacfbvfk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nmcvdrrv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3omcswpyk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yfbafife.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luyuhixd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3airgrycu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oznjrscx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ngjwvgpl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3thpabmqy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ioqrager.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zkkpltpv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gieadier.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqlzhvzv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3captcpwn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kerkruwc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hpwjynth.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3cptzmcjt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vikytjgt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3orpogtbk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zerhwedm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3plouwsuh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rwqcxojs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wrrdwmpv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tmrrvmku.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfubirri.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wuqornai.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hoibkmmm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hjctoead.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ezjojawk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3psafhscw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llaadjbp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxiroxuk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fnqfzwth.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sdlfqajc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3exqkihbd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nnieizoi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yhtezbfb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qcqatuip.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3aadxygfw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oxjkxpna.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhzudfhc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hfybhrkh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3iajerjyg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzpzxpps.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jvmcguea.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pglwyhqo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hntsjeer.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqwqrxsq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dxqecrky.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pmcnutyn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3axhwiobl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hlveuzny.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mmnyrauj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfgrdyaa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3suzgtkjh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xueboxjg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lzabkbbc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vlsuiujf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vjrinrck.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bssdgwlt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3koebdimr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3diuabmuf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lycptsth.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tszizlct.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3okkmihhr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lhmodrpl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iraupkqn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cvywxjrg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cyveawms.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmwowzvm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zdbpodcl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cskcveba.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3elwyljkg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cbpnasof.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nelmoiyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dldedcto.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hxlkwzpz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nguwzyqs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rzxvlfpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xgbdfchx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3srpnpbmu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zwpwwflz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lcovkabz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dnkknkil.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gqwxxabz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtimfyb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vkbybfnj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gcevbokc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hnqhpfjx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qytdzcdf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cfwxnalu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ihpnowtl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jppvurzg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dkamsqmz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dveqmqgq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpptiqed.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3clzssnwy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yxawnkbr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3acohfruj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kegmwvbb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xzbexbvk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xthzfowk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mucmchwf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ajovyelv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tnelfphm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdbfunjy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vvupfdvj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qwzulbsc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wmmglskp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3heubncjz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zvgxjtjm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iljpgjgw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bktbmbob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3appsqiss.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wpwfgcrz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3urlfjjow.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3croxyvir.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3igtipsqv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jclyamyv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cydsihzp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wvmrztcc.html


<!-- 参考信息 -->