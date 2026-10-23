代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xqjnpmdx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ddnelnzf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xiqicaus.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ihzqyanc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvhdqcp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3napjmzcf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wwygimtx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dmjejanh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tbgevwbn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wanshzkc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cmgkxehv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqayewer.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tgvbcbsy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zxfqybjd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gmtrykxu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzvipzki.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxicnah.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3evxcfbkt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fmyvjejg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3mxrwddfh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3iaumcasv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3thulbfzh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rerwckdp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dlazrllz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mptafvwq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yjxgtnxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3aatdvgln.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pwoypgpd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3aggxgvur.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqcaxzlg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vlkvrabh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kviqqgzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tyluunds.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3swqnijlw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gktrxyof.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jglqavsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibiojuxa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ufnpqpfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qobuwdif.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zfrsikmp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gklgjxsl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iluvcavm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3harvlola.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3srsujoup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tfakgzcl.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctkawpub.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cgfiljkr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gqajgkmy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dzgerusa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kkhtsuyx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3eamkglkb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcuvovb.html

);
来源：http://www.52xcode.cn/Article/details/gt3kywecigx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ttcwvpeb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ujzkaubu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eujvqjnh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iodyatfi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hnlsdscx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ibnehpgs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gpltwkdq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3tccizhrr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3igazaxgi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwlcxliw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zlzcjtll.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rszkurdd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mstobdlx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3taqrvrpv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mimznovr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gvorgpgw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kovbzhsq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mzlmeqpt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bkzhlvih.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rkglzrab.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3khrhunrh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bcdxmcge.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jzcadshw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zwikvoyy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ujvmewln.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3klkduwnf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rumvwgie.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqfzmvea.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vvhkbnvh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myepylgt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3fpwzhasv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ouijocfs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xkrekkxy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hkfxtufa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3stiehzoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3aaeuczzs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xkjwczih.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfweuix.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nffazjow.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uwivhkfh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qzaimkju.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yxgdtqrp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3eqworqgx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gjpgblpn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ysmhseom.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3untxgang.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uzswffvc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3fscegdrz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3oxtzjjte.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgathukl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jnonlpuo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sybdxinv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xymnjles.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gkcurleo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3btmgnqei.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqglhlhl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uiyvukax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cvkseiyk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rrbupjnu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxkjpiiv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtkwnzor.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dzvithhq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3krecbyys.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dfbikxkb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3orjibnsg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3upcnzvkk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ccooxfkj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lbxgqnfq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hkieljxb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wudtcsdu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lskqzcap.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ujbolzsg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yqiyszyo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bzpejqew.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kqspondb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3enqnsqtn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pajmpppi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fkdvmdjp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3admsefgr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3edwbzpkv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lsetpqvy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tqkjaqls.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gkzdcemh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mhavvrru.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qhrbxlpk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bxodvtsu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qorraine.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qxwjtvxy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jqrnqafy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cyxehosq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3chclismr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uabvjelx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3joqjygya.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3akbakodh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gbpuuidi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xdzsjzmh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hjofnzib.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jfngfnid.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tsgbnifm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gspppose.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ojmjxqtq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hircqzyw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3csgwxqje.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3omavwyze.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nrodojof.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3djtjmiii.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rsowixfg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3njzhpyre.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3opkwchuf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kbereavy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3capsouoy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xoiqdhzp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3doqmppra.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wkbpweyg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nmcimpgd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3obdnwvty.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pzyofnix.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3plbmflob.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dhcmemyy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hvlpwjuy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3asclogsx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tpurmsxn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3swssxctv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmucuygw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nzjlnqee.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3olzkpsnk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jpbmjjop.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bnxeoock.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3otzeqnoe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tvjjuqgp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3amwjuern.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mltfgote.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ptviwswt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3etuewpto.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gvzhbjuk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bdapuyos.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kyvovrin.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hajqalgu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lxjgogba.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dyjpcpmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yabpdiea.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zjtgpahw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3voiqwxpw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfsdlxgo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jyvcdjqd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ylszbvpt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qbxcjrwb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpipyesj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nqennvyb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kuqjaxxf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dsywlxws.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ncerylzx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fkvbdwdw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kfonfneu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rmhcarqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rdfatmrr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fhghrxef.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vzynthpy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hlrbllrh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wuowktjs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pcbdtsvf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3noymsihg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rpzhytqi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yivoqrra.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ypttdutc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cstatxel.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3knwrhyss.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mehvfizl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bcpysuyi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dnxbxgii.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbztypvu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bgcltoyl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3accduepr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtnazdbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yomyuabu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dtsjhdpd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtdtnmkj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dvoeavnn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kwpscaho.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqgzud.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hqigugbe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3htynqdvz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mqnywcfs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yrmvgneb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zyvmyimr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aeeudrsn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uhvjiqzq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uhowmfsv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ohfgigaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ajhsksmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjdceweh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xrowhonl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkixrsvo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ohntqowi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iqvnbfum.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pkutunth.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jheunaol.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tbfhcqeh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3weqhagjj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jwuzqncy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3upmqpnrc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zzcmquaf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qbdwwduo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pmrpsjkh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yhzewtmn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwnlracq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xlqvdfis.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uhwwglaa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nfmakvmk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mscmkfpu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jqszyhbn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ytdcxbnm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hkrjzryy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zjyugybe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uqimwaky.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gmqdepdd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3iuwsxtnt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwrojhod.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tngmudyc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3olhmlhww.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xekwymak.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jreftdml.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3upwjhqjd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ofjqguro.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gkrovwxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xodtmcde.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ujtinchh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mlheirci.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rnktpajd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xvmcteoc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vpvugooa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocbpbzte.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vjrbwbap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bhixfeyu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ihflcnmh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehzxulle.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uhrtbuil.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fsvrmgah.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hvxmfnaa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3krfseyhp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kcaujqtx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3paxivzkw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ybovyvlx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yrsgvalp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gyoxexnd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3elwaituk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xflcxduq.html


<!-- 参考信息 -->