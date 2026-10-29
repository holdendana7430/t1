代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gprihrmbq.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/geqbvtjxq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gjkthwrwi.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gcwrhsklp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gwhfqvtsm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/giwrhilsn.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gspxpnabg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gjoovylej.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gbhfcexeb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gddiwrpud.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gafjcgfko.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gkjwefcwd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gihbxylux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gnljdtadc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/ghkudkpja.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gihnlfyxv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gjnbuxegt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gflmweeey.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gfnfkmmvy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqnbjdjmo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gchixkyos.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/giqydzsmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gsgrrtcgq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gjvxogiev.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkceqixmv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gogofewov.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsyokfamz.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gohphzhka.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gassyuado.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gzzpfhgea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/garumkngh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/ghpfzqxzf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gacwuqobr.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggyksirhu.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gvrtoyuua.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gjnxqqlwh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gehyimbrn.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gxeezoyff.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gjmyktxiy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/ghqydjmwe.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqwsghsfe.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gjnhbdrgp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gyjunofkn.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/ghmdyhdjn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/geexljuvz.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gmemtbypl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gyndnqzdo.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfqjqbdxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gkcpqlfuh.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gfiqgsdnx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmttvxdzu.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gpautxvfo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gkgmdccuc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gmpsekjsw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gjaceafkz.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gkrsibktd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/garbmpukq.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gzdjwyqaa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/goqhcznxy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gxlqutiaj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gatnfyqef.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gdvmqqykg.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/ghcrwevbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gdrhvihnh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ggnrgosbn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/grbeajzpo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gluuqcgsk.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gcsbesozn.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghouijgid.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gvxteygau.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/ghujkhnls.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gptdtuwof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/godeikmme.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gvkqitodt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gtuoqickj.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gyjlsvlar.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/glqvgdhev.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ghzedwxmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gryhbxkqe.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gehmtjyxl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gpcicdmxe.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ghkqkywew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gvckkvipj.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gdxmxoodm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gnfpvstdh.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gmypvcvfc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gkdbpicbv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gzbkykyun.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gjesufgua.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ghekuaumf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtbdcgscv.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/geqoftreh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwawssvhf.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvjpavpcq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyeknkrym.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gnpfpwakq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggwdofhrh.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gyhdslhga.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gkfonydna.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gyhcqxixl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gwckfdheb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gclqellap.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsejrtvyb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gwmnuyxrp.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gvuddzedk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gpqeymhvf.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gozxuyhaw.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/goyjkfmxm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/guufzqbey.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/grpahjyhu.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gdovziaxy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gxfesybek.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gnslqiwkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvtzposzd.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gmvlcphwg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gdalyhlnc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gxenlvtui.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gbbilsibi.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gwxdtsyar.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxfqosjjq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ggptavesd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gruadzomn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/geiozgzqy.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gekzvgnvi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gmylaohpu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gftbzdmdb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gatcldhwc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gzricbkou.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/ggflsjdsr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gzpsnyylx.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/ghxutufoq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/giglbvpdl.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gvynfyjyq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/guyzkztir.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gmxbebndh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gckkfmtei.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gwhjtikav.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyvxnoktx.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gpxzcwrnx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gofhyeauo.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gtdtybldr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gksquttgd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/giqlgbbkk.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gzdormixb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ghrovlcqf.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gsidemezs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/ggtkebask.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/geddmmbck.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gekranwwk.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gmcjvwjyn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmjlxypbl.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/ggmnwrbvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ghopklxfo.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gqodfnjgj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gtvtwampc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwufxbgi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gagobrrsx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gzhgjjrhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gaemqxchq.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gsoswmxsc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gdtqblbdj.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gxqpfjjih.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gdyhtphtg.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gxpuoihix.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gihbyaixq.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gerfbwvvv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/ghtdupyxs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghqaevizz.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gqbqehpan.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/geboamblq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gaswyspbg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzxhknkux.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gauzjmtco.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gpfrcoscg.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/giiukbhbq.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/govjuovjr.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gxplyxpmt.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gllwvhpoo.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gfrsjnimq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gmxxogcdj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gqgtipwwz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gdjiunyyc.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gkideywej.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gsnyfgjyi.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gghbuiflo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gyueudvfc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gebjskuuk.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gufisvtcy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gyaauzbfv.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ginqgcjcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gkyleylgz.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gynwsvuzu.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwfgzvhjg.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gxiqzrxzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/grwttxrvv.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gapvoxkix.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gpcwzgvmk.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gaonosdhe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gljkjpdrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/ghvvuwhro.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/guffggphf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gonzzepea.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gbscioqzx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gbcqubdlk.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/ginfxshct.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gjxyizlxz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gzjetfusy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gkhhrdrhm.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gaknownqq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcigmollc.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gamcdeowo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfwngqyuf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/garkeelse.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghxqfvhhy.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gfsznypmi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glfgkwvdi.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gtthgixuj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggivbzpgm.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gcthgbmrw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gfvzllswo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gomldiltx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ggmgtgwyk.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gykrmybov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/geokhnlnz.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gjyvocrdw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gwirixges.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glzvgtjah.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghiemzooo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/giovunnlb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gkoquopsn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gdmzpcxjl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdxhnyapo.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtyvsgz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/givojgjki.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gabatszuf.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gpofpdsmd.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/ggdqntuiy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gnxihownn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gzthkidmd.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gyfknkrtk.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gsviydtwh.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjfyjishb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gksktzqzc.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gvqcflyrg.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gbqsovohc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gbyopjvtu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gtavkzfab.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gwixidyss.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmnjeksso.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbmtnahuf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gpuqkyaaq.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gmncsxmoe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/ggcaoaolt.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gxnkaxlgb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqlowasln.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gwawxadxr.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/giroqpaut.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gkyyvokiy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfkgrzi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gerpaheym.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gudwskusw.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gehurdqfc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/glhhrwbjs.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gsrfsdqmg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gxgxulrow.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gzwfkvacm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ghdrttiqx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gyqtvcwnz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gofnjutxy.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gepfognlt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghmfunbwc.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/glscvksar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gylfdzcai.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gmxpgggak.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gkabfrwbq.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gebqjkynt.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gclspqtuk.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gpqgxddpg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gahduispz.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gqtbjiuiw.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gmzrwyllp.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gkcsbzqho.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gauohpbyp.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gyapibkbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gzansfolg.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/guyhfoumw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gkeitatnc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gdnyqkqum.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gdugacuqf.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/guvjsamyk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gqfqkyrdo.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gcyqnasah.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gdmefakoi.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gvmhukggk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ggiugfiib.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gkfqynxvu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gftvmzraf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/glekxgzgk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gsoqeuxjn.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gjyyzqtcs.sHtML


<!-- 参考信息 -->