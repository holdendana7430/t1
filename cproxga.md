代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gjgfkdzaw.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfxekyjhf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gplzzydpy.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gqtukebps.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gsegokrei.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gkukfhzuc.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gbnrmnmry.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gyrrclhrg.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gerjolxwj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/glaflchnm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gelhkpqba.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gakubyrrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gsguoekqs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gsrdnwiwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gyjplpmcj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gmbsdofjb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/goucdkqne.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gfehzkjwu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ggzoyzdlk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gpnfcdsyl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gvubcyraa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gkwrabwqh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gzfoqfxrj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gflkhyfco.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkspncxj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gixuaxjbn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsxihahlw.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gfungikiq.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/ggqwlvyip.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxvvxvoxj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/guidtdtir.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gcenfmtqd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gjwjjwfoj.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gjvoivxgb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/ghyayasgt.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gvruphief.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/geeqhgyve.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gpuuqegxb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gsvtkgcnr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gkxxwmdmy.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glteqxnul.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gbgezxjlk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/ghnxevibj.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/grbztydpr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gwdwqgsza.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/ggcqexbfn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ggvytpjof.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gwyxwdqzr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gotogfiuq.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gdlfdodqu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gxrnktaic.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gbverfjiq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gtfpxfpcz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gulwksato.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/glwlfnubs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gwigppfbn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/guphvivbr.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gbnhaeiph.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/grypkhbku.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gctffnmvy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gkiicuauz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gtthffyje.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gmziosqbs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gerzocqup.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gyitaiyed.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gtdoaukym.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gmyrxccmi.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gsrwytkts.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjagtccii.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gixgyjukd.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gthaqhwga.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gwgkpmpnl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/glxqwkvpz.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gdjzbrupo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gqfuobgfz.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/goihqhiyv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gnadjuksj.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/grbcnnsim.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gckvkjoel.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gbdytgekr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gvublxbik.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gaiywnude.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gpllrjusm.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gztdroabh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gkpwnpfck.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gddugjgmu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmxtmyhcj.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/guhmzjayi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/grpfimvau.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gdnvcpdak.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdrplwywx.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gyfzwbpzi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glghqykmu.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/guonabdhi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzotbklcw.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/glkhwrhtn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmwboifna.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gejptdptd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/ggfnfheyd.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/glhiaejao.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnettbmfb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggyagyzgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gshwftxax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/grerqqntp.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gbnacwaxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwbvwidbm.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/govuyzutv.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/geloxppuh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gqcjfaowr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/giswxyzry.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/ghytcvnic.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gmqktgqmf.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gitgvcctq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gmaooxlrm.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gcqyhelsk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gkzmlwyxb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gvgntajla.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/glungdbwk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gjxrbylvm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gqzfakdir.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gyshbqewr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/ghhpymunm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/ggdfdeatc.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/ghfkkxbcz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gwyiwbvdg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gwrewujmj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/ghhghfumd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gckldpqdm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gajobwcqf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gncbykwec.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/guaskgnmn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/ghswqbepw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqraasovn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gdlkoyuzz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gnldoquzi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghgayudst.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gsaaqsnip.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gpftjwiek.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gatwzhfzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gsqiuvyzu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gwkfhweir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gjmvdwyoq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gmrnyjevo.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gacvsdusf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxkmkcqgu.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gszwgjunh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxhxokouf.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gtaxebynu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwaawtxm.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/ghqtnltyz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gatcjckdh.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gjqzjsdzt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/grkdmpjxs.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gylpjfgju.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/giudfiymg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/ggemrbils.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ghnhmlmks.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gfdfvwpze.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggcrpjmum.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gcnkpnggx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbwfrttsa.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gwptggomo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grgwcimxi.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gkgnywxfn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gylcqejuq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/giknrxawz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gwqnnafxp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/girjodpym.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gkfpofmld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gttfzpgsh.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gzqkubrgt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gsefrskro.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gmdjrwtba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/garefztvh.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gosrldjsr.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gqbufergf.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gkrrcgyju.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/ggzvxfgqy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gknddiuxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gnykcwfdr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gurrvkdkp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gjbvlxnhh.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gcnutyqkt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrbypzuq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcdknnquo.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gxxljzkec.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gvbzvvasw.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gfwlafjyd.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gzrkdakbk.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gpmutnuhj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/ghmgtikij.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/geeicqgby.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvebhzzgz.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grlydgpbf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gbukagzex.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gqehheggq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gqtretqjz.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggcigcsza.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtezijuge.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gcccnrfex.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gjlarzyiq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/glcwnkhmh.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gljhzadkb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gsdfatyae.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gsxgdobuc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ggbkrhtsb.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ghdgysmre.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gzxkjuwyt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gveyiyags.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/grikqpwme.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gvsevwcxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwlgiszbo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gptrwetzg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyxvowlkr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdjoqiwsx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjwwikryu.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gthegxqad.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfwgkvkgg.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gjhyockof.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gordwoipo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goftucxld.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/glbdezcin.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gkvyzpvba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gbyybuhtw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gynwomegm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/guspixzob.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gtvsmgwha.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gtiedxbjv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gahdxojrm.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/giwsbiwzj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gxoearcit.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyiocujhs.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gegvdqmvp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grmygxdwc.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/glbsmwrmo.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gshgvqmon.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gxuxhwztd.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gypkcmfxe.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gnywbxzlv.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gptkdqqnj.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gpatvpnps.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gjydkdnue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/goxybokeg.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gvupsndpx.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/guhollehy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxpzhzzaa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gujdjazch.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gesekpecj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gtnwrxlxr.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsomtnxfh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gasbkqnoa.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gmnidkyrv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gaihmhyps.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gnkrggtyz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gnpqxfzmd.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gyapkchxw.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gjkbwolji.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/geavgluax.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gllfiqqcj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpdiltlft.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/glntmoaap.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gqoogwexs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzvguzcnn.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gwhajoaei.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gymlgqzrn.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gqzxknqlg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gpudqppzf.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggpabdwgn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gvjtumjaq.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gnoqrifmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyzvtpvyu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gxmgpevgw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gqbpufger.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gxfuwbsfg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gekpazmai.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ggrvooqlm.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gwmnlcxrz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gnjqehddc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gdzwzfxjv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gddbpffsk.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/goecfiwqa.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gtxjycjfi.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gmhakjlff.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gluyrjyye.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfmgkhi.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gyzgobuxb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gobtamqwb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gmfpoqrgk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gtorgsdzi.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gmujejmdn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gbseprxrr.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/ghrbfinao.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gcbsubbaw.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gltyejrie.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/guluwuqef.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfjgfurhh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/goriizurw.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gzacxzyvd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gptvpcntz.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gsnnrppbh.sHtML


<!-- 参考信息 -->