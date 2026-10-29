代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/ggmzjaoab.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gpjtfkzao.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gvqevlnre.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gnkevcsqi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gkbjmhyoy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gvvtrqyot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gfrepango.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gtxownaal.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gebpzauhq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/glxqwacsc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/ghcktkprd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gwvvutoba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjdlsrcic.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gvsqsaqlu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnsczlfot.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gztsllxad.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/glwpkwzlv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gmuxpbmot.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gjqngiuna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gkhbrkyeg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gcxhegjaf.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqfyrzmwr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gkbhmznur.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gjvxdhror.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gjjfpktoc.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzfutpvsh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gxnpgdnjh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gqmnlsgks.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gvpzhtfqm.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gsyzqsqth.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gqbxnprlj.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gjtlaqbvs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/grurufpox.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gqrpqpdtm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gdzvowdnj.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gylygurru.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/grqfmtear.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gefzwvdwj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/ggqhwjacy.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxyoioaam.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/glafpxknm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gtqqjkxpy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzbfzzgyq.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gqhhtvias.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtltlggea.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gagifipya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gbmvmetgh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gnxirpafc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gwmumfufs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gjzzvfiud.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gtysztewp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gnpkfukdb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gztlzddcs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gmdihoxfy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gqtjuaqyp.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gojujhwro.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gthyighne.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gugkwvytc.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gurbhohdw.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gnsqzfqzj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdfavopkr.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gtehpcdat.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gttvfkemm.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/greiquhus.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gmxdeelag.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gvdnsbfsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gfvecfqpl.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gizhfefzz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gnkgkdzjn.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gmcyqsqbp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gkiuzktpj.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gnbnbtphb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ghipnbxqu.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gizamzxtr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwvifcctg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/guvvhitao.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gcwfyvaep.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gxbyqwzug.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/geszdcuik.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gjpoatpwx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gsyqmnqcu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gjxiapopx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfxnvmrjy.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gkurvsvbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gycznkoxd.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gxeqcjyhv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gkynahfqd.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gkyaefgll.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gzzxjvwmw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/guouuidxg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghemrajnl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gfalmjduv.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gkwwelgdb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gqouiczag.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gngpszgsd.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gjilfmqvb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gzobmoema.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkfzikea.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gyoymqizi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzbmbtdqo.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gfnvvbrfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqxzkhyjs.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gicqcsfbx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gtndxiiyf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gacbvpmrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gybkhtzay.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gqawjsxsc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gmfwqhhew.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gptwadxqi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/ggyczavps.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gdhfpfgwo.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gacvfwupf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gnnlmwnqy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gsmsysfel.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gkgofqyxl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gdnmawynv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/ggyxsinkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gsazcqgja.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/guxxqsehf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gaywclqor.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvwwhofet.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gdjoqgobs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gjwydmayh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvepbcomh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gtcumqfpr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/guraeotjq.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gylnvrkrd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gfrysqtmb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gjyhliqba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/geqyvnszx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzinzajtl.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gzkywljxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzicyovql.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gkdovnajm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gfnxmuefp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ggfovkbcx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmnkmmytx.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gpxnmyyix.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtcdaoxwo.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gitieghmy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gqacosvsw.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gebjbyvma.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gjsdehecc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ghvgcppdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gkmglndvu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gwrgrobup.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gzwlkyjvu.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/ghyupvxpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzusbduvw.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gjidbmwrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfqcrgquz.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gfplprkgq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvxwtiegp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gzquabevv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gsxgcsdbw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gujwcspqm.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gmszxnoxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gydkzjnqs.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gzejobytw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/guzvtwcwz.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gekpnvqzm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gheohpeij.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gdcigjmiw.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gwxfocvsd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gzfzzwabt.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gwbhwbxrp.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gglgbvhhf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gzrpsovtf.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gpfhctipg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gikjdzopk.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gpsltehuj.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gtwvkamdo.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gmdzkwcut.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gytogmjta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gnxssdloh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/genjhmdbp.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/griynpdga.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ghezwrzdx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/ghgctukza.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gkycetzut.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gscvjqcde.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gwvbjwmga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gqdtsyiub.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gptjlbwzx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gpqrdhvxa.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gatnvmcxo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtasnxfsu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gbzwwqewp.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gcnbzljit.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gndlxtebl.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gxxqduuuu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gyktnfgql.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkvhqrsxs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gptzbvajr.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxbttsaqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/geqxrijjm.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gizktlofw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcyoovqzs.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gbtgztrwu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghgsslyel.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gkqgkaocg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbtvslqxp.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ghdapwozl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gprrwynnp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gjsztvigz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guhjtkjrt.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gejqwxhfb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gghssdcvw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gzbpploxz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gsdbwvhep.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gsksdonoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gnipzzwkf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gxrbsyxfa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gjuwojkcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geaoiwvhg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gyzpuvaez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gcxooqquh.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gkxmhykjz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gkxrtjsce.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghdjqjlai.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gottkspyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gorxtciyl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gblehmguc.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gjyvrnfrf.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gjdrvzxgl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gbbgmkvye.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gbupzoaag.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gwnoskukz.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/ghtixhpvj.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gsmaftzbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gjzkcmvfk.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gjatptkia.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gskdgckys.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gcwvebjnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gxgdhbnde.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/glrhcxjql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gumdxqkcn.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gsdbmytlg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gnnhxcqgs.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpkvmhwjv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gavraxvve.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/ggpmwlkvc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gogfxasiw.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/giswwqghs.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gojzxijni.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gfullbsfo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmyiwxlzn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/guhcrrmbd.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gkjzxagcp.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gkutjahjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gabqcxkka.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/grbxnljwz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gayascace.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gusrbwxpa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gfueaqtbn.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfhqmftfl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gfygeaddo.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gbrohilax.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gaqeqzzng.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/golnzdotb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gytkldnzv.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gjwfjwodp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfwvukrrw.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/goorloimd.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gsgasybrb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/glpibmjpn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxknksaq.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvrxluxwt.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/girokubbt.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gohiqrnxv.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gfnioxfhg.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gjfqtzant.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gsujyjzee.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gvmmuezdc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gulfcktmg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gvkcatzyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gtyjtxogc.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gvtbiaqnm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/giowdwsyj.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gtyziiriq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/geswkafmu.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/ggtqckymu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gypqfixin.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gycmcoitg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/glqpywgkm.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gyyepnsyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gfkykigcv.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gvbuyhxsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gvnoeianz.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gqzptxogm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ggznpkfox.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gktffwoig.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gizjislyp.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gqhtfwivm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gpntnvzlz.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gnunvsrto.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ghdpbltxh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gbvlhvvgi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gyfmvcrox.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gesixyhkt.sHtML


<!-- 参考信息 -->