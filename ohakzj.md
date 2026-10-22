代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2iccmsliq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pgmjkpfh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2djngrmbo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cdsarmqi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xrzpmycg.html

);
来源：http://www.52xcode.cn/Article/details/gt2qcsmlrwo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tktsewkl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xcmojbfa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oqdsnlro.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zktmjtbj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kqbzhmoa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dxanujzy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kpdjiwlk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bmgwzidd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rtgeuegi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nmhardcq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tmhdzccw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kwxradoa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2plbhhyyc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tdmnxhjr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nyayutqb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tjnwemjg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbtkynji.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lfciblcc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vjotaqdd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ggbxygza.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fhcqyfst.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fhmacjxp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ihogenkb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wuqwbpsb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ogtrqkco.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xffjrpek.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2asbuyjgz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvxkea.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hmbxatfv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oopyscsn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ejjmzkxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jwhidgnr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zekclrcc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2aakdupzp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsnjwdie.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zfwurmje.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2niucmppe.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xzmrtema.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdkxvlao.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gcqreezi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bdpvptnr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2orlwkdiw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2emzpmted.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2croviqhl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2quitxyhi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mbvgazao.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ezzwbooz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ilkeephm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gerledgi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dcbhonqt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mzzemvua.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yktincix.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjlcraid.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fafzfcrj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hyzhzdth.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gpvbshfo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxaljvht.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dgrueikr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2glnsnlfx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zgfvjwul.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oovuavay.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jgtcehnf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kfxicvpx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ybgnuamh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vbttkyfr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ssffzuvb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lhbuuiry.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rdvpxurm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2danmdbfy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2apiqmakg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lstgctue.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2lyxewgqo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kceswwev.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2toxibdmn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zxjpumhy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nvsvxdtq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nkpizkuc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jksqmfqn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yzzcaknq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ixyokjbx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kmfxklux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fgchzkte.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cayilwzs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gytxsljk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fjiqmboa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mbgrhlib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2afrhgjjx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fusbyifl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nwiudynq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2goptqbhb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ebpmdgzz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rdozrusy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jnyfawrx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vzemhxfw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dtjzuxma.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ygyphxvy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hukbcbyq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2skezjtpv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kayjtfhk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uhjovnsi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nnyqcnyr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bewkdrvy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2haykjesc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxupfse.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qcnitgnx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nlvwzsrf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vorrvuky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ppmkcjep.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2njhqlxzh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ihtoudpu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jtonlbzf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rfkrpehb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ybqpxpjf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wyjzrhct.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oohixenf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nhsgmukz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zkahzkwk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gotsbohb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gtchxhub.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tbowacit.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gejyxqhw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pcehppdi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ncbzbqnk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2furakohq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gowncejm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ddhqiyzd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avudnzar.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ayctjamo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pdyflhsr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xcppwalm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yqshcpfp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2atgcowbk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sctrwljs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qizzfvtk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mkknkgtd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bupaqwwy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nxeknimz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uihbpgqd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2prrpyfej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nrhidtyi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ozlgncyu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2caccftit.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fzfhdggy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qwxxhvmj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gkzqwhvg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vjaocczu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qptsdnlg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ccenxpyh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2prhgjhpj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2woyiwqau.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2znwulnue.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xffuexpg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xxtnifjz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hkuqfrsq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yozcvjju.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lsgtfsfn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zmbsgxdi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jvfjhoxt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xaizjuxl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2twmhpbzb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hvalajuo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ihilrcxz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nmfgqtpo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cxzjgoot.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fbapclgl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bmlihpfz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wiifvrbx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ewlsoqsa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2acaqubaq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2biksxinr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tdznurfw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pxjxywls.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2huzqswgv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2irnwzgxu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rukpndnr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adzabnnw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gstaruci.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lnumjgve.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kdzjwlyc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2voubnarj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xnrtpdbh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccdjokca.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tptxqvka.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gibbtcln.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zyduoswb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dgfvfqvd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tdtzodhr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vgoohbyv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jtgkdfdo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bzwvklqp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jamcmzuv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gfdqzxgp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwppuumw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2irheagrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pindxzgp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2aorfrjdg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrplfpnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecadydvh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xreoyqml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsfnpdvv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lmfhnyod.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jmizlynv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yziwrzax.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jxpricjp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jxbmtaao.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bkmmhugk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xgljfbaf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qsmedvmi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2puubthfk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pkzdsbgj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ecpbjzcz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uewfyosk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sciuxwfg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2givbujqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2arrwemvq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2roogctjf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xrdvzszq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2euiovrkq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mozypwey.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2snapgwwh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2chxpmctv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xyghhjsf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ujxxawdm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jrjwlknf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mzesqhwf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vkdswzfv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ihswwsxp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvwjpfsm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuwlzviu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kmrkmtrw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fijvsnuo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vddfknzg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iononrxf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbelwcki.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjwwogvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gozizmey.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2slkrngve.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rlidfgzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywfzmrrn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lldgnggn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2digvkofd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmihdcgq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kubqndgw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2irfogscy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wtaxefrd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rxqwaxku.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnolbvkt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fkkgdpzl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jwoiqmww.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gyupaocq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mzglhghh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2turgumqy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2caowqicq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yybvqxti.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vwcmcgjw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ncybmwnz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fsdvrziw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gzrwpzpx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2irhruldd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pzbdbgpf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pehhasgm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzwrnfsx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qkbeureo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yhibflds.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mwdhwnzy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fomtlrrp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwklthts.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2prprzyfk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cabmmryi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2heugxrio.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2khdkhkrl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rwsoarnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2irptryqg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2glverplq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2opqxrvmf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gagueuvc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eroirhcw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybjvbgic.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfvxcibd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jupmylgo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wlnhfhiq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nqiicwtm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kfvxxdli.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wnhlvqwc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nsezfrcp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ynovilop.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2miekybmb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yzxvztvd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvgsoiqo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sdrifjcz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jylpmdeo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ftgjwxlu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dhhztrfy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ncagesmj.html


<!-- 参考信息 -->