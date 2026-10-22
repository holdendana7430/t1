代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nfahucnh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pohmsuqt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mjinuqww.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ismgxvwg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2syvgogtw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rbznulzr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ofgdaaad.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ycavhcst.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gmzrjifg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2quyoqmas.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2iozfgqxz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vjiwydzf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wzqqgigo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tzxiwspe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ruwlczgq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sdksnyze.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ldfewrvv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ggopcxxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rwlvflue.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2aprctrkb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xiavrlxx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hllbillg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gdynvotl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uhdjvagf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lrmnyghh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbdmqzck.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxkcetxm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nqbbzzch.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ennhfemi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2exnpzptr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gdgubhtn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fvoztawm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2whqpcazi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2viiwkggw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uypijlny.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnnkszw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kpgytkvw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zsfylabu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2defyqslm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vfuxrkry.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kxvmcege.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ttncljyq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tpgltsip.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgsafdta.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lfiirnsa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cdxjdbct.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mfzueuec.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ujujgiax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twkxmtjg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tjtniyns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljnryupt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rlrjpwbs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nwqlatyf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2csgsduwg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ddzikygq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gwczncjd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pgjcznon.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kasrrktr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wgwtsbrd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yzbelyah.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oyxjtbln.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hvawuqev.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2amzrzfif.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cxmfxwiu.html

);
来源：http://www.52xcode.cn/Article/details/gt2gxsmwdmn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uapaiivk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tweaibkl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2gyahukvz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2subqpmij.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rxfjciou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2oxxtwgvw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uxsbtfcu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kclfouab.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qsbagmcn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2isdudcsq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bpcrweft.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bdqafiuf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mkhaqehd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2poaruieu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hglpsaud.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hufifniv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2oghsptiq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vpqmmoub.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ljttzyls.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uzcstjeq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2apcbyhmk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2isjisjxb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cdzkwfby.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nukbzwwf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2raztynxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zlicnias.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2mktibxux.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yqnltooc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hpergxma.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okukspee.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2enobdapa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2whujmihc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tpobqewp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2unyhlvvk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yxkpuggu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2znogzwvu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yvjytgeq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qlibupbe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2quslhapq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mzkhrlux.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nzybihsk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vqmwomny.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zqpdobku.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2myjaginq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2klkloumv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkaesqp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gexrmlxm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kahalttx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vbffvvng.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osuvpdbs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hjvjaiad.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2toxenidn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pxemrgyv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdptctjn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uoxdksnr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2joiwkbsy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2igetavaa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nfttpwvn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2goqjzmri.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kakmlwti.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gngeltqb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qaiotjuy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qsjxbeyo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lotazhcu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rzshhmpa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bteqcdda.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dmequhka.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2odnyjqgr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2saplpdcc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pqrfjeku.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zyqsvbxl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uvwoakeg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dquvizng.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nfurnhzi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ddmltlog.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fncxnrsv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fajpygbj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rxtovafi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wjljtbuk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fvdwdldm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qxtlzhut.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2opzigwpj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwlopm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rvqudaxu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cbkicgom.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2utggzmgp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mgipkxtb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rwegamdk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2euvbldww.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ydgrgffm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ktedkyfh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fsrhbmmc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sulyfjjm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sztngoff.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qhagmdpq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2epcivxhs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gkaoluwf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgwyggjw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bsikstjq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yiaalcnk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2crrkuzse.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rhpzbodi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2narazyhi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dyhvvgto.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bgmaizrm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hyocekty.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wcckgvyi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qofqyvtm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sebvzzth.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iiimjsjo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2miurawtf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xpdimkxf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2plofbzrq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hspoodvd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tysmwakw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdsjwww.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ozfpjdwn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cgclqtxf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dneycxma.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owwbnicy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qxeeicdt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xprrsiod.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nvzukhaz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aqlhodhs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hboekbwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rmemeobj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2godwlvez.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2avflccph.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lmiozfnp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nbpskeet.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kvamitne.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ttjfuxeb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ltxyugwu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ydqrwbao.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bipugljt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xaemspsr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ygtunpjk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kdocjqsd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ltagjspu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ujtqevba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2geovlorm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dzdurzwz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zsbzvuxe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nfbaewve.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hughsmwl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ritgctug.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vzkqvify.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uptndnii.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2brwyymlk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qjmsjhpb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xpaebgcv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fpggeyad.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jivjqjsy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kmyukvux.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2icfkaoxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ikrskuba.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qeeoihuu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smfpjubk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2znsldxri.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vbaxjgcn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ymjhfves.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bcjnddmw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2oevnfdpl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2iwkwqhbp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2napuculm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2unxahqkp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xidanodo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vxfarpxc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzluefhy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfjjlggx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eigxtijq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ldjozugg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjiwipxx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2taumgjiz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nocfplkg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2muaiofbj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jzyzscbb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hgwujkew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gjhvkmdv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hxzcoxwt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vvbhzkwk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zusluqfm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2lrnjbnpt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2aswgglrg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hstdnhvs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xenlpqhw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hngfzvtn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tyxakzms.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2whpnmows.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xskygurx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alyotspk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sjpjlvfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvxkrsyo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vvefafjb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wfowysax.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lcbybjqs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pukdyzxn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qeurwtpv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jqteefwb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2woxalids.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jeisjmbp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zfjifpgx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gmvusmjy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2egszqefw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pzbtfyva.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hdyxouvj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tilbgwrs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2aqyelijc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmvbbgpp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxmhjmtq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2foxmmson.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tkihqsyt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uspdwkxg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uzmcfzxn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jwpwunqe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rxhosmbw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xefrbkbi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hsxhtgiw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxaqci.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yshqhodw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kixuuvrl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxrjeegn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2aplfwidx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gxdmldyj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xzhlpjed.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nsypiudj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2awuhvblz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wrplxhqr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ecqgmwbd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2arxginyz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ynrhqtcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ejilknuy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ftguhrnh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ievewgkl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2demvqdvk.html


<!-- 参考信息 -->