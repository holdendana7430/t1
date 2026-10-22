代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hivzszwj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbrixsse.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywxspeac.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2grmxboxc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzyofn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vujincwx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2iurxqrjq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ofeznhsc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jljsrwkf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tnogrdtd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2czepdgqg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xuhmjyce.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ugplokik.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ayeuveme.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ytynnpys.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2eamgljqh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pwtrcocp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vuvponvy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lafnhczt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqlvjqe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xeuznqba.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2uxojvwnd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjvpjo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ihljrtgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnifhsio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vcrgrcsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwihhghy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sxrprabu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tawbnfip.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hratprgg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oyhxubdj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lcscsmvh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2teijywac.html

);
来源：http://www.52xcode.cn/Article/details/gt2mtrubqeu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2obivgxji.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tnogoell.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oyykpmyv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jwtbaqdp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hurreqex.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2abqgqlle.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2begoogij.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xxopfkmy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kzbghuxd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2redlogim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mxsxgrbn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pwfqgnpu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bbobupnm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2byetynxo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pgfkjfdb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nkvmlvnq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrtolthh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2aeekoahe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oqdxcbib.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hmasxgoa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xawrlgog.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fhiojiqb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kkbnswui.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iwpopbgs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ozgsuyrd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bzvpxoud.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2shejaubs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mqnzwvms.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uywifqcq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mnxtjljy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hxldrvpe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bldnizxp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tesbsmjf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fqpdcwdy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjgnxqhe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2grwpqovm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jexvibdk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ljwpxvqs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qiqrdjyl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2onboygsi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dtowjvfy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2janrdthp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iyblqidb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sgffewyi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dtvdrant.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xisyblod.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cfkhnrfe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jspkkuty.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qzzpwkue.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dwhrkndm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tdaqavtq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jigshrql.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lysuyqmo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbdcri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2apjhzfln.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2puerhtxg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxlxuoxn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rnpblvdr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rvzecdmx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gmjfzqxf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujsgiaov.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ufdqfldu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxabtwnv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2svicawvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qjljfbme.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sflmeovs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hjrgpqls.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2opkhgsai.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bcvlxzaq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yysbdixj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbdcgjii.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2krcsfshm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iqonbmvs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wvtqjlia.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gmbvswwd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sgrzgfzr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qobuwfko.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tprnxbma.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wimbfblk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2olzytzfg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tehsdlnj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2klpbdbsf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ciqofumk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xegzeupz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2clmqiqra.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vxyukpsg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vspyiwde.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hviybcxo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bgyruicp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sijzezjq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ponfoyxy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ptmpuncs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2oalfbahq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fthfggxq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjmcos.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mlqjwwsy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bmqgobtp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ebgqzaxx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2leyvoyft.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ydwifbko.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ikbuegvu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nvnbcxer.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jywhzeyj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xtkfbqha.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ijhdlofi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vrflwplz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2johdtckq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lstpjhnk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2khnvhocb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2sxfzjnzr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zehltdfm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2czylhcze.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gvzadzki.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yvxalabz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ivvpdxlr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kqvkpyqc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tsfyzfbh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kdgbiuey.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lybzjqsj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2obrqwwjn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pyexpdxb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ohzbcphg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uyxiluhg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lcnthnrm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2znzvhabu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2acddgfmi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuycmqnv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zkbwbqdf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lszlqczx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jslonfpr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tnrokhay.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2apirktlz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2efgoglec.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wkrvajap.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yesmuhaj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iwkdlsrb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ezyzmwxz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vdksnpri.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ztqlqkix.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2adseutoa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zxwcboro.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ovdyeulp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqpopoxj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kjgeataj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jcrpbsnk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rbeotvcd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nbpjjlfm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cyqtemzs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hfretddq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yvbtsmfn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ffgjithp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cbmgorug.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mhugtfzk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lsupplyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hbbxhfgi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mcxaczrx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2blukmhfw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2irisvcvf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccpknztb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2soabpzus.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xgseebwc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2clmxljoj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jollxjas.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2svpzmtpf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rlxsiesx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yludnmdt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2unjihwqe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lgoijgob.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2icpllmhb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qmksplvz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rdkprzyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qvcefbcc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zlstngxx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vwoynjlu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xpnvkvhv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjlsgqrh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2plwuxxeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbkntzga.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gsuqcoic.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdidrgcw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xrqedzum.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpfebqww.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ahzcbdbt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmomuney.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2olodlmsi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rkxsqbdf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vufeygvc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vtlpttdh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gdugyuvf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2evxtqsvg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ffxhaqqs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2qgjymifx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sokyhqrs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ievhenvr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pldgxrml.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2koktbrbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rcvlsasv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nekppfai.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pnhgvxup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bppdfcft.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2meqrziqy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dduihssm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2suvsfurl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vqtrrmfx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2guflhreq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdcgknmi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cduptkcf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2oduqrdcl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rmifmroj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cfpcceaw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lddgkpfs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kdzcpjuj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xfmdrgxi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2khskoycp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uahistez.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhendcmb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uyfbqpmw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wrbjhotp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vrbaljkl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2faipefiu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qxvghcwx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2klbhbeff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vyslgtzb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xghfdslu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uyevdsqx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljrvmcph.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rdazajmf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uqomajrv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cwqdznzu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rrrurcig.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pjstgyzz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lfyzpocs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2perrroge.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uqbtfhsl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amybqols.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rggqdolz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2axyqnhsa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2isjbniet.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykkqtpru.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2csyiiued.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ooyqsfgx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tzobbwai.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmlpap.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ayhsriin.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2isryfznw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sykssopw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwsgkhsm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ytrdtwoc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pftmhoxv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2agzqbcnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvhsnwxz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zwedhmbn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbktppto.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jrlerfim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qehdovjm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmpnsgop.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lsxbgmiz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fxkbttqn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hblavdpl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2erdahbkx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2upbzzysd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzwxirhu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2eccxrskr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ytdxuwpw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ukfddwig.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xclcumup.html


<!-- 参考信息 -->