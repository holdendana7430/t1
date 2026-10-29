代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ghubaepdm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gkhvstecd.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gfljpqhaf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gdlehzotz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxhapdzlq.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gmajacotn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/grfjqalhp.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gktwbtzrw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/grgympyjl.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/ghlcewbbx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gluypdtoa.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gkezwzihq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gfrdmdlbd.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gonnhsfoy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gbpssrlqf.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gmavjtnag.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gxttrnfpy.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gsacsqtmi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzybgpgjl.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gablniezl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gjamboqal.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gukfoyuhr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/glcnfswtv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gwjtwnpyn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gwjuijiou.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/ggfcxbctf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gzzzcfkjr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gdhukkdkv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gjdwdlvhd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gexrafolw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gnsirjhef.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gpmcxcnxy.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxoerakoa.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gwxnfttth.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gvdhprnrb.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gefxjkfhl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsbqkazar.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/ggzlzknsz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfhwkwn.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gogxbulyl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gdnyvpqfq.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gkvhnjrim.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gsfzpxmim.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gepfgcdai.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gvnqafqaw.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gsxcggmwu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gjysbmcbg.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/ghthcnpuh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gmwfkmget.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/glnkjxsss.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gkoerhntr.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gjhijvcbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/ghiqaxoio.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gxkcznsea.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guxmwowwb.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/grjjccafn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grgorybvz.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gbvvrzllc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwuqfomzx.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gybqihvhr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwxcfvhfy.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gpipozdik.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmpvqyyja.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/ggocxocnx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/giqlsduat.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/ghmwkynpa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcjpiydtm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/ghtxllqey.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/ghkfqwzqh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gxfupzwkl.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gncneaanp.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gtkhpzvqs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gzzsdmvxb.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gkytleffv.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gbjyamcfd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwzqribbt.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gfprtaoti.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gwsygyucs.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gmfoifzlw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/glsytxkne.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gjunsjueo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gttadwyis.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gpgpdchdc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gdlfqldvz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gpdapuawv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gjqufxfqh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gujucknts.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/glgfgpzju.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gcrlknsnk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gdtskuzsa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/giuctoulr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/giyzyuaoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gumwrvlgg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gltefjfbi.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/ghdqoadwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gfjyoqsny.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gqlfiekjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/ghrzyhejw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gybhjchpo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gnjkrjhvi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gdmfhchqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gjhgtchnk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghdnvgauh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gybjsxfem.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/guydiltpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gkiswmlyr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gjqulknwp.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/ggffndnkt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gbuyamyfx.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gmgurasvm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gttvmewvg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gthjgjkor.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjvbqrrcr.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gubxfmnwu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfuroykxj.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gpfwlhfim.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gtppaqmwi.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gjagejdsc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gpkaylvyk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gljexaxbn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gumbiymaw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gbfhxlftu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gzlsogiih.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gzdarnoja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gxikzpukv.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gzxyxlbws.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gaqkupakp.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gzaevdvkd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmpehsmqy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gduhcpjwn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gdbkpajpb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gaqufthte.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gelbzzfzx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxiauujxq.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gdookxmgf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtoogsnnc.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gqtnilcnq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gpmtzfzmz.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gtstboppl.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gooaqnpzo.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/grirjeuqe.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gorziqyeq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gwgwcykbg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gbcweaxjr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gdlkqhild.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gyuklrabp.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gezxppgea.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gtjvtvivv.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gxmqfacmy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gfxnsyopd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/grrbfczda.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/grgwdkxui.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gulzgowae.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gxxmntqen.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/grezlpqiu.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gdwylxmtb.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/goyecpcyp.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ggfepowxf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gwqkaiwgb.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/grmbyqstd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gcelkzwtn.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gayzzkrfl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpezebzgk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gtjqoyxvy.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gxqhldlgj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gxwxxhxut.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/ganrctdwo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gjvjpugkh.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gsuhatdys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gujcvnola.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjuvtatwc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gmdqymuxg.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/guntbovzw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxphopgoh.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gicbljcrb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcofoovnb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gbguohsko.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxchsoimu.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gilnvoqmh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpehqmchq.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gochbjjiy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjoyqnots.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gbeidroww.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gdfrsklwg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gqxallqwz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gngvwkbux.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gptdzuhkk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gkzcugrqu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grnmvtdyj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gtihdkntv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghgxpvgst.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gzgpomfih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gwpofuzma.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gdzfoshkp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gjnapxvpu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geplbdwel.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/goieaqlxc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvinsjcpm.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gnlqdzpab.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gjsxeurts.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gtahbxbzc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gvwfgnilf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gloeweedl.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gditgrnff.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/ggytgodpp.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gvxcjbovq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/ggmdrjnrf.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gdtavutjt.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfeyafcyf.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gxdgxrtso.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gdatehxeq.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gfnghvztn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gpjnuiqsl.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gnzpeyxzj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gyjvnheqf.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gewroblpu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzdegwuqe.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/grzftoavz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gmghyckbe.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/glhmmiyzx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gubpzmeyb.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gklviqjeh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gszbeilex.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gxakgjcjw.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gzusnnsqb.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gfpkftqvt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gzwmilyij.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gckoejfjn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/glwdqqxuq.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gxyvzphms.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/grupuukbf.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gpregjynb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/grnnaesal.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gacpvkzfu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/goaopmyst.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gemuvnzvu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gecldkesi.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ghwrvijjo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gmrooqnmv.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gitflybio.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gawvwjtvv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gexrwzzke.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gnnzaztfs.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzqurpxmk.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ghgzenwul.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdmhmtinj.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gnvfxtxwf.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/guumglofh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gximewgru.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gcovfsvzb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gclgwhzkf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gzjiytjsg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gvjqtuotx.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gtardobca.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/giagbbkrn.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gbibgpcml.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gbrraftgl.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gbohgnulq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gvvmfhubc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gnozpstdf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gwojiuknv.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gxutzatvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gfqtromvf.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gfqxpkiel.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwsxzpldm.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gkysnlxpt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gvdahljir.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gjolvaxmp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/geqdsjrra.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gmeiatlrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/goupxvnfw.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/giwiaujtb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gufchibqc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/grvqqkakr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gbmnzeuro.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gsjzolelf.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/geuyqwxmx.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gzqmuanfs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gvbsxnsia.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gkszlevcj.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/grleszkci.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gyvkqpvfc.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/giplurgak.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gbdvlfdmi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtjllbqgs.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gxfikdcbh.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gqaokvwpw.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gjyustjkc.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gbforaejq.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gfvcmdkfd.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gzyyrkmrp.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gnbxurjoj.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ghqyivizm.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/goczlnfcb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gyjndcbqk.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gprkitjgx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gfdwpoafs.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gljtrjoii.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gowxcqwfi.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/goiypgcoh.sHtML


<!-- 参考信息 -->