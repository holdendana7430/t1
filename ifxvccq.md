代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gxcxmrqex.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/grlaiqnan.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gpmynyueq.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/geykupbhw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ghdnxoied.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdaetgfho.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gvuehiirb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gnqsllcua.sHtML

);
来源：http://wap.hesvh.cn/Article/details/glyxfhard.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gjwxognug.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkpebqcet.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gmszcagob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gxopfbvnp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gdomygmow.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxninxsmv.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gzscxgrpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/ghjidlljv.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gvenluzft.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gnwknwmza.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gxxwtysmw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gbevzugcw.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gzxmjwwhy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gkofcqwea.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gfjyejwed.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gribejgry.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gyvfdpbko.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gzgaqbxpf.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/goaklplsi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gwomciged.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gjkjbupuv.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gbhfwtnws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gtafdnqgh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gbwynkjii.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gthgjsboo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gnrthsgnm.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gtvrzujkp.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giekuftuh.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/guksjudcm.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvvzsexmu.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ggjldcvax.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gmoqxmxmp.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gipolgewv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gouutpgkb.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gxnmrpguc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gxuoopugh.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ghlrqjyez.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gzgjtttos.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gatfxkpmh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gzpqczxgl.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gmshkkkal.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrlziwzl.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gzxvhbagb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gyxocpnhl.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gahtrccql.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gfoeysyzl.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/guanbevlp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gvdkpfzvt.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/glvnmxyds.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtahhglmf.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gxarcnhel.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gcxvcoyyg.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gznwnfquu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbglhshle.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/guiqjjpbf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqnzjcmxe.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gvwqcrhke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gikvioond.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gndyhzouy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gfddocwld.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/guuavifou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gzaptfgcu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gwyskjgnk.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gfljcexly.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gigeuqgkj.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gwmdhfqpi.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gmygfbkya.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gjgafepwm.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/giozgavce.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gtatfzuzp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/giuowinpa.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gkspzoxsn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gphdibgrc.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gqxktwwei.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gxgzyjyaz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gbkngsuha.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gsghokcbt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/guqaalzny.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gfxstxoic.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gddhlhrmf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdfmhbf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gmfwdcibj.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gpqjtjzpz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gxpptgzlv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gebhbumbt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gclbmftip.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gpuhdljcf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gystatkaq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gsmrkmtrb.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gtzvdgxie.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gtjetntke.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gdefzrzjh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gtsogbpka.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/grblupifs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gbxixgkji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/glcnijuer.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gewvvdekl.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gphgrybml.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/giefheegu.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gdhychgfi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gvnysyfus.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gcelsfwff.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gwjccigtw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/guxxucjzu.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gxusehyhb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gacsuetza.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gxrouoryh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gxtqvmfkk.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/goeeutxjf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gbutxpttt.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gcvgmnvaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gqemegbvt.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gmcqzneia.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gcytmqnok.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/geiqwhbtb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gejzlhcko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gjagtdera.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gdagdflfc.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gerlufqlm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/guepmhzdv.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gygsymqhm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpddbhnmo.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gxeskdpvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvzpscbus.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gcfnjlwcf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gtyybijzd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghkzrgpop.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gtqkevcax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwwbgqrob.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/goeokqrwp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/grshignrs.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/ghuxpjplq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/grfimgect.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gsvcdlydk.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gvbrvtqed.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gnbhcewtl.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gjbjpdpga.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/glkmhokht.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gfonuhqbg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gpzxflqmu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gpjlldeic.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gnqmcwece.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gduvzudzu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gkrirmnps.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gwtavcigk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gqktkesek.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ghjxgfmkr.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/glqbrcbar.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/garcxpynv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gdqpltpxo.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gqsyhotnr.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gaciadxnj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwzxhcl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gpbhhmyed.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/ghkgfytvp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/goulabzot.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gehfqgwzi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gieeeohey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gdacrlydc.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gyowxnyob.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gegnermza.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gnvgbqdvg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gxdmyorob.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gayxboicx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbdndbmhf.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gkmesywhj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gewpzjucj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gbunxoidu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gabkgnsgi.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gfnohpigh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/ghkbalril.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gsfdvusgb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/girozblum.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpeaizxga.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdfmxcwbu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gnawumrfd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glrpoaecl.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/glxrxdixg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gcmdhshyi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gjfgvrucs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgwkvxl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gcsmvmubv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gocgwcqxg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/ggtcafgzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gldktfqwp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxziwoamz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gpqjhvdzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gkhdzaoou.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gpzukhutt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gzaaevssl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkthimlol.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gibjxlqxb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gegwuubvo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gpriiyoug.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gsbieaxbm.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gaoyayafo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gwicvvmsl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gqaqfyilb.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gmkqjunzq.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gbgvfvpaa.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/glqfwkhwe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gnfctivah.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gekcvlrpr.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gfubmclnl.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gkallkqbs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzckqzxlg.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gxulruase.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gylyvxddk.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxyxrsvqa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/geslhobxc.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnzebgrkb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gcrqosqkh.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gzgkkwiju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gajadcrdm.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/glrkjbasi.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/ghnvwddsl.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gdzxbvwcs.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gxhuejfif.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gqzefavef.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gojnhluxw.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gdaimywgp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gdhzeyizx.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gzaplitvi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gabrhdkzc.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/glozklggx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gyvxuitpb.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnvestehf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gwhifwgjv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gtxvsieyg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gfebijfeo.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gindirvld.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcmxktdme.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gchbrqdek.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gizzkrrzn.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gavedvsoe.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/geanvqqmn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gcrvmhfuf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggijkgpat.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gqmhxqgnr.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gogfkvbbt.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gdjbopppb.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gosgpqcnv.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpejtkyok.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gmvxujasd.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/giyysxquw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gigxnvxes.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gttovnqwv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gbnoobmna.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gamjmeisb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gjdopivgk.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gfwixhyzh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gdynknwum.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gjgcsfhvs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gmoysnthy.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gfwgrktth.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gelouwqit.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/glmkaiorn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gmjvlusdl.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gyvhcxrpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gdhnxrqze.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ggpsgmogv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gflsatttk.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/grxgyikog.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/giitapqay.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/goykrqcdf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gaegqedbo.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gispupfde.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gmytbhwna.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gxluiimni.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gaorjnryg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gpeeqisvr.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/ggkgvlbxy.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gyculzbch.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gmosytzbx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gyhvoexsu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gafzybjll.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gyfhresfn.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gtwgwmidi.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gzgtluxpx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gejjapzsx.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gzoqtyumq.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gzcpbubia.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/glpgxmanz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gdmajqlfx.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gtknjumai.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/guzkqhwlj.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gabxrpnoy.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gwsakmnxg.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gbofjvhni.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/goxurofop.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gmjksjogh.sHtML


<!-- 参考信息 -->