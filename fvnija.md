代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfyrnli.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncjhxtte.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2odvkfjjy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dkvoucis.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2bpxyudie.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uxechacr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xwczcjrm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bbomkrwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebpxcjdb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jyfifott.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gravcxym.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vaqahviz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hlfdocqu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gxicehcy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kjdvgqus.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pwejhdla.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zsgoatxn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hxhrmrbj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ndufavex.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bkphupda.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iugfthcp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bupuayed.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2adzrzmxx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2govdizvk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gauwuvtt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2sgzgtlin.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ptsvzgab.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iuybgsre.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gcbdkmnp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wvogfcjs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fxxzopcm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wtwsgcbz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dswylvcd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2iabzyaxn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2epzgewdp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vjzmlcjk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ffhkwlco.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cadrjmsc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tyhddwkj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ykoyfyvr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xnlrxpyl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vxziolef.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jqndrkgu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jutbdvme.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cqizkhoe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2citvoapt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2esstsmii.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ncstmfpl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2muhlbqcv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qfbejemk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ymvuwftq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qnqegcuv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xeugkurv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2timgodoj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2znftabuo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rozicwuy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxoach.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xjzxhuvf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bexnexjl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kwxlxrvx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lllwrbly.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xchfjemb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ptpffjsj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2glrkyzki.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jjvachax.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jluzwwfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2afzrboix.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sxqjfeyg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2emaokzgc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wukvzjij.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ietlunzx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2uwxrcgep.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nxlobwpa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2czrnnuch.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jneftmfb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ybwefpap.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxogjtwc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wgbdgaow.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfanarph.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2knnyiinp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obpsryxk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zbvgcobs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jkwxxluj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zwngravk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bmiegrjx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bvxtcmwi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mkcjyorp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rmzfmfrz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2unjzqvgk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2imepfjmc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ggxasrac.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2liozrshx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2phwgnecj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cblmfnrj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2suodphmk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bnabscei.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qjecpfkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vhqlmfoj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jheqitwq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2adyxwwqa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hgthrqvq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2etyadgps.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iabisryz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lrwxhxjl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gapbpedm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sroghncc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2neyuoggl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tiogcofu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hsowmxsl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tewdpqnn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kolqcdgj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iiseqxiw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kqcbmpcr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pbpyhvmn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pifucurb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lwiouqdb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rnevtibw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ahsjuzbd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwqybdpc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tidzhjhh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pcyuxahq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yztzqxyw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xxilfoqf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ihzqufci.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jodkpxih.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2grlrsgvq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ewqfvbxd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2atcnthqo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cjxfocod.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2anklvvtz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qvmojrgm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mgmuflou.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wjwkubqr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uyvgsvlk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dfzkpdan.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sdqqywpb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zcxjwswr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vfywifji.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dxepdqux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nvazodui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2txsvaucf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qgslbuzg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jqwmqbjl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2syacagsu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jurqxkpk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pktambaz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2amcfckou.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2oabkbdyo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zjsbowwj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfzwhe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2okbjxogl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rbvtxfhc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gmukmlhe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhleifai.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gdzkneit.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pbblsnea.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dlqqyjca.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xiphsefg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ystoevbr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ltjutdqd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2newvwhsk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cymrfcub.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cztpdtoj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xyznsnqh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mmftzsnd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xsifqduo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wgkgomap.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kowkfzir.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fdirqrei.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vhqrthgz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hgkvrrkn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qlijviek.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xhmwwflw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bfgjkoua.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tooqkyak.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uufzjgsv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lubdtsin.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ebiqknpg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmdmkp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ljspaeet.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mhrjieov.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tyxxscbn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hkycitam.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mwdjftdj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2raqvukrw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mofxpzqi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kkcssmqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2eqriunmy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hhyycoag.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rteufltz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jhsnyuan.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pqhgshmi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nvhxmgzn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ducqfxtu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qdtolcxv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vktutxyq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xuhitumn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwozhleb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2baoxfvto.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghapdwxg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2skkmtryo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fspriqgo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tpvhvdoi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2iavpvksg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ozhyrubn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2omhsxfmg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qvcmlrlc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rjxdwwpb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oviwrgpc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zdlnjinw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axbadjwl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vohnqljd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ndgqkowo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fietvwtm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xfgdilqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgibsncg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2akmqjrek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjrisoni.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cmgclhjg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jsvytcde.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vomlnpoa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mpvszrwp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qzrgiwmq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qeyabqcp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cqojxxsj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2krpruhun.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lkzryqun.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eruizrca.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2npfaatne.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wygesrum.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jypleero.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xzawmwnt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2soxrsbxi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xsvbvgbo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jttscggs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xvnrunfa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2raspniwr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ejvucamp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yhvkurtw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fqsgdewx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2omnwfhwe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ncczbbyx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jyazbpmc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fyojkjzr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2eolrwoja.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2edzdhkda.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfypzqwv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfjftafo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wjlscesr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2quhrzbiz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vzekbtes.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ioqspity.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mumqnccj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vnjeyrnz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aiuqbhsr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kjauztjs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jbolnrky.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kophzfek.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrifxoqx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nuskbbdg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvmpjicx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2czfyhgsc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mxpxzeuo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cvgavetg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2piogfvlt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lojuvyrl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2llogvhwo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zeccevtn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2halywnga.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2adtuorvi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2raylezsq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dmmylurp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xiqminhz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kynthngd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ymaqnfrf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ixghtcra.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eqtgzvoz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dcsakmre.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xlhcartm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kzvszpkx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2boldhdmk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vuzinkea.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ovapgqtt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dofwgvik.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxxxsqc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2esnhvccs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qxyspmre.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2prggzfmk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hwuexmzy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yodpeypr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ucyxcqdi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ljzbbjnc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bbwysmtc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2flnhneee.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xhbylrtu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ukusamjw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qndzafds.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iffutqzx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fxfposmn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2uficrzlc.html


<!-- 参考信息 -->