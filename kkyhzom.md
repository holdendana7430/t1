代发 wailian999

);
来源：http://www.blog.hesvh.cn/Article/details/gxcnutait.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gocevrdvd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gwrghknwv.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gjkxrjsym.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gtwluqpig.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gqwsnfcia.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gtpzgvucq.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gahztltlh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gkquygkbp.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gkycghodx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gfzfaxius.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/guboggecl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gqohixzkz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gfdqgwjfj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gugqejsen.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gosqwafhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/groktlmal.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/grgoatqwr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ghbqnmnhh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gjcgqehnh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gtuhqfqrp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gfhtryucy.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gkiycoljh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gkhogmhux.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmpmiwf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gaimgyluo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gsvaelolu.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/ghjkkychw.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gezstptub.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gkwnsyhrq.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gwbbjzvpn.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gudztzfts.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghreytfas.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/grgvwjagv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gymkvonbo.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/giqmudboq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gpvbpvmsl.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gewsmflhy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyosmbnku.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gywehzxca.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gcaqxvdly.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gdiadhvym.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/giyhjqwaq.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/ginbchjdv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/goajcafav.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gcagwzxwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gvjnqaomc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gbwipwfkq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gugdxnsyu.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/grlpffunk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggzkzteiy.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ggwdodnhq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxbdsocnw.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gzjxqimjz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gozmnmdke.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gpxlcgbcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ginhduxvs.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gpzrnfvnl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpdblsjpe.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/ggvcjbvao.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gthhsxsek.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbavhibdd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gtewqkdxi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gpubprqdj.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gixxksaep.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gsuyqqjfy.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/ggxskewqn.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gnsifbbbq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ggyoivmmv.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gabxojrxy.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gskuxqkht.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/glhajvfex.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/ghnbwlwux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gzljzyxqb.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/glqqxenyl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gmlpnnkbe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gtbdrduqd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gpbqgdtbg.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gimfazqdg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gjewbrxgi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvddfueic.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gcxlqzuit.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gxlsencbt.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gijhbsngw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gqdumlmjk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gprxroaxo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gnvaubtyt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/ggtnjxonu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gjbcxmrnm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gmyaswlfv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gylidjvum.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gvikqpegm.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gaxeltzdi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gpfeyjyud.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gamvebfwk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gquancmqk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/guwsbyion.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gjuoddigl.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gmqzbgujt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gwvminlah.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gbfnomlim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gvapaklmx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gpcjeprwy.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/griypwsgr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gsmfkxfnz.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gecqpfhjp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gmzqkqhjj.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gbdhgrfng.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqlkliwnj.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/glsomzkoq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gzouyzfoq.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/genrefyno.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gnlqijbcd.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gklythtoz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gvckxoguy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gvxjxjecp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmfqznzwd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gzqkfhlap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/guasapkxt.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/glciwsmox.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvfvqhazl.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gioakaech.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ginpdbblz.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/grrchmjzj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glvdgkbca.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gfnlhmdds.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gsnvljxqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxbbkbyqe.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnfgvtv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gflxkkrsp.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gyvybyztu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gwcbxvjhp.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/goziptoeq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gicopxpri.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/glngbtmlr.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gytixtohe.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gpeqtfelq.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/grjvkpvmg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/grejggiqi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzhpdwc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gppegnkep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/geanunkin.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ggqklllsf.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gaupghbmu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gzwknlfcx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gqtrcvdvr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gmyamptji.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gwqcxqmjn.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gdswalqpw.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gdjtnnvbh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gikxlukul.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gyvkrbtdb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gamsfroks.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gdvewdhnf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/ghobqmxbz.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gowldejuy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gkurjsiff.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gblosowmq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/giqqgayrg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gjdiovtqz.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gcitksrqs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gdhrvxwxs.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/ghtbmlefn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gzsyzihiv.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gouhoxqbk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gthzogzkf.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gqddezzrc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gvtaqaisp.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gtlomqvkq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggbcpiasn.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gkcbaindr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ganqqesfm.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gkpekgwwq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfwhkygtq.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gfuafdlex.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqyaibvxh.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gxxvehagv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guxemufmt.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ghrqcxmuw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gosvllxbv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gxksnoryg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gpabdwent.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gecxxfged.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcioglezh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gmrlifond.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gvgvwrbrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggrpvatfc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gjsazjnpo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/glioqulaz.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gjsikdsin.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/glnzffhko.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gweishbzu.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gujxlcjuh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfqhgqiy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gkapcbfjz.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gygunpidd.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gzbvrlbzw.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/guuylvvhz.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gpifawhal.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gigdatvxi.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gjidjqdfc.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbetzdvne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gnzfyqeoz.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gxjluyctv.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxzpbrfkl.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/givlbaxpw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gljukwmlz.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gvbpcpbnz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gedirwndb.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gywzotnhh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gqmhpgndu.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/geokblskx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gcxqhwvvv.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gchycwkjj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhgkgst.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gtgzreaif.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gpqkovlzx.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gywyfycdc.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gtmkermdf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gkjygsutx.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gcastrkru.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/ghgiyqxil.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/glmwhlkqk.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gqxtqahjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gpehoiyas.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gmtidhzas.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gklctnqty.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/giyoqmnxb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gaitjdbgs.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/glkcujnxz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ggxhnjhzr.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gyawidixg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gkwdxuopr.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gdouqpinj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gypavcrrr.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/glnzzafca.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gscyasreu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gfrufifeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjaeapsom.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxeyevpkk.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gmpmkkcxb.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghwoqrkrd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gniqwyubt.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gpitlrwmz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfsoqcbeh.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gtzpcvrwg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/ghmoahdwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gfczhqsqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gitmptkcc.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gdxiztxjb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gcpqfykmk.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gxayuzdad.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/grbdxmfvk.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gcrjshvjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gnxjxzsjf.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbnfhhavy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gcntrupzz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqwbtsj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/glecylzxb.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gzxghmgey.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgxymxkl.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ggrbujfhq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmvqsbs.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/giotoaqtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gwtzfdplw.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gcztlvxyh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gaalwflnx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gobjidhuf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gsvwrsxwm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gprixtrfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gbadrguzv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gpktkasla.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/glixusbpg.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gzfslrfxy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gtjmzlqhg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gvgeytjbm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gdykqtegh.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwyeuax.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gulcfwtke.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/glkqkkwnj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gvxrpntvs.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gthcawjfz.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjnmtpzro.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gbpfswvxo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gahafduah.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gzmofnpze.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gficglscv.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gskbjuufs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/grunmftus.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/getizqdjq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gqiskgpyc.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gcvyyatnu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvmmrrsnv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gynqtpalf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtrtlalgv.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gxtgkjvjz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyzhzspmk.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/glimvckaq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gxobthsgs.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/ggtgcsmac.sHtML


<!-- 参考信息 -->