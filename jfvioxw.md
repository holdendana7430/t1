代发 wailian999

TS:   crypto.randomUUID()
来源：http://eq.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://ta.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://ui.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://hs.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://os.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://wr.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pf.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jx.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dj.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pn.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ur.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kp.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cl.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ye.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://gn.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xv.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uo.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zn.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tw.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ww.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ut.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gx.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ur.bookmarksfly.cn

[P04] 求长度
来源：http://ba.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gh.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mm.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kd.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qw.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://di.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://le.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://tb.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vj.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://rt.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tr.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oh.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qo.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ok.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vq.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xo.chemitech.net.cn

Ruby: a == b
来源：http://jc.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dt.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tr.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://il.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://ua.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fq.haigaiapp.cn

TS:   if (x == null) {}
来源：http://ri.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sr.chemitech.net.cn

Go:   if x == nil {}
来源：http://kg.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tj.lnxyls.cn

C#:   if (x is null) {}
来源：http://au.haigaiapp.cn

[P07] 防抖与节流
来源：http://tx.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tl.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://mr.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tw.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://li.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://he.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hu.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gg.521024.cn

[P08] 处理浮点精度问题
来源：http://dd.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wo.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wa.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ck.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ao.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pl.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qw.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sn.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ff.jianghongdianzi.cn

================================================================================
来源：http://io.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gw.jctech888.com.cn

================================================================================
来源：http://nm.muxihuayi.cn

[Q01] 创建表
来源：http://uy.huanxung.cn

CREATE TABLE users (
来源：http://tg.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fj.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://vu.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://bd.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ud.szsharing.cn

);
来源：http://ty.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ef.huixiangedu.cn

CREATE TABLE orders (
来源：http://tu.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cs.colortex.cn

user_id INT NOT NULL,
来源：http://od.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://fr.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mn.colortex.cn

);
来源：http://nn.hahajie.cn

[Q03] 增加列
来源：http://kq.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rh.muxihuayi.cn

[Q04] 修改列类型
来源：http://tv.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zy.bookmarksfly.cn

[Q05] 重命名列
来源：http://hs.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gu.wgjwhj.cn

[Q06] 删除列
来源：http://za.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vj.huixiangedu.cn

[Q07] 删除表
来源：http://dl.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://xt.hahajie.cn

[Q08] 创建普通索引
来源：http://wh.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ca.521024.cn

[Q09] 创建唯一索引
来源：http://ke.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zr.huanxung.cn

[Q10] 插入单行
来源：http://yq.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ke.colortex.cn

[Q11] 一次插入多行
来源：http://fw.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://di.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://vz.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zu.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ou.huanxung.cn

[Q13] 忽略重复插入
来源：http://uj.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cw.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://wb.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nx.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tz.yuntaijiaju.cn

[Q15] 查询全部
来源：http://nq.lnxyls.cn

SELECT * FROM users;
来源：http://wa.bjjhwx.cn

[Q16] 查询指定列
来源：http://bp.shxzskj.cn

SELECT id, name FROM users;
来源：http://tl.nszjky.cn

[Q17] 条件查询
来源：http://id.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fj.shxzskj.cn

[Q18] 模糊匹配
来源：http://da.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pd.huanxung.cn

[Q19] 范围查询
来源：http://dj.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jh.jctech888.com.cn

[Q20] IN 列表
来源：http://jy.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qq.shxzukj.cn

[Q21] 空值判断
来源：http://yl.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sc.huixinmuqiang.cn

[Q22] 排序
来源：http://cn.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://az.szsharing.cn

[Q23] 分页
来源：http://bl.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gs.shxzukj.cn

[Q24] 去重
来源：http://pa.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://ny.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://am.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cq.hahajie.cn

[Q26] 计数
来源：http://jn.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://zp.jctech888.com.cn

[Q27] 条件计数
来源：http://ou.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ks.521024.cn

[Q28] 求和与平均
来源：http://za.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qq.shxzskj.cn

[Q29] 最大最小值
来源：http://kd.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://az.shxzskj.cn

[Q30] 分组统计
来源：http://aw.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ii.yuexingan06.cn

[Q31] 分组后过滤
来源：http://jd.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ne.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://sz.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wj.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wx.hahajie.cn

[Q33] 多列分组
来源：http://bw.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vs.asd995.cn

[Q34] 每组取第一条
来源：http://qo.hnjuh.cn

SELECT * FROM (
来源：http://ge.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gv.jctech888.com.cn

) t WHERE rn = 1;
来源：http://qo.huanxung.cn

[Q35] 内连接
来源：http://gb.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dp.muxihuayi.cn

[Q36] 左连接
来源：http://dw.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ne.shxzskj.cn

[Q37] 右连接
来源：http://jg.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jp.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gx.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ka.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://xq.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vu.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hc.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ly.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jh.colortex.cn

[Q41] 多表连接
来源：http://ww.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cn.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://fb.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://sr.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://mw.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://pk.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://te.chemitech.net.cn

[Q43] 标量子查询
来源：http://lt.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mf.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://vp.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://po.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://np.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gj.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sa.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pi.hnjuh.cn

[Q47] 与平均值比较
来源：http://km.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qh.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://wn.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lr.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://dp.bjjhwx.cn

[Q49] 更新单行
来源：http://xb.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sz.bookmarksfly.cn

[Q50] 批量更新
来源：http://kq.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rb.521024.cn

[Q51] 用子查询更新
来源：http://mx.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vk.wgjwhj.cn

[Q52] 删除指定行
来源：http://jd.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://by.szsharing.cn

[Q53] 按条件删除
来源：http://ff.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oi.bjjhwx.cn

[Q54] 清空表
来源：http://nt.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://kv.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://qo.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wm.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://lc.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://po.yuexingan06.cn

[Q57] 行号
来源：http://wd.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zp.9csxet.cn

[Q58] 累计求和
来源：http://un.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://za.hahajie.cn

[Q59] 分组内累计
来源：http://ty.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yf.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://oe.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yk.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lu.newstarts.cn

[Q61] 移动平均
来源：http://ch.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ps.yuntaijiaju.cn

[Q62] 分组占比
来源：http://su.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ro.yuexingan06.cn

[Q63] 开启事务
来源：http://nz.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pc.nszjky.cn

[Q64] 提交事务
来源：http://tj.chemitech.net.cn

COMMIT;
来源：http://zg.yuexingan06.cn

[Q65] 回滚事务
来源：http://ss.yuntaijiaju.cn

ROLLBACK;
来源：http://df.szsharing.cn

[Q66] 行锁查询
来源：http://il.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fm.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ih.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zl.jianghongdianzi.cn

[Q68] 保存点
来源：http://uk.bjjhwx.cn

SAVEPOINT sp1;
来源：http://id.newstarts.cn

ROLLBACK TO sp1;
来源：http://dx.yuexingan06.cn

[Q69] 查看执行计划
来源：http://mj.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://so.huixiangedu.cn

[Q70] 更新统计信息
来源：http://jw.huanxung.cn

ANALYZE TABLE users;
来源：http://sb.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ak.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qj.jianghongdianzi.cn

[Q72] 查看索引
来源：http://xb.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://yi.muxihuayi.cn

[Q73] 查看表状态
来源：http://dl.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://le.gzmigu.cn

[Q74] 强制使用索引
来源：http://du.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uy.521024.cn

[Q75] 日期格式化
来源：http://zz.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fx.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lm.chemitech.net.cn

[Q76] 按天统计
来源：http://fg.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lt.nicolike.cn

[Q77] 时间加减
来源：http://gd.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ng.huanxung.cn

[Q78] 当前时间
来源：http://fp.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://un.huanxung.cn

[Q79] 字符串拼接
来源：http://cq.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gc.haigaiapp.cn

[Q80] 字符串截取
来源：http://os.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bj.shxzskj.cn

[Q81] 字符串替换
来源：http://wy.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://un.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://du.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wl.szsharing.cn

[Q83] 大小写转换
来源：http://jc.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qx.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://wz.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://oq.chemitech.net.cn

[Q85] 数值取整
来源：http://mr.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jb.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://ot.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dn.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://yt.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ej.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://fh.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jj.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rz.szsharing.cn

[Q89] 判断表是否存在
来源：http://xj.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ye.huanxung.cn

[Q90] 生成序号列
来源：http://oe.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ll.huanxung.cn

================================================================================
来源：http://tl.shxzskj.cn

R. Bash 专题
来源：http://is.hnjuh.cn

================================================================================
来源：http://hr.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://nd.shxzukj.cn

#!/usr/bin/env bash
来源：http://sp.asd995.cn

set -euo pipefail
来源：http://ht.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://ga.newstarts.cn

name="Tom"; echo "$name"
来源：http://yu.shxzukj.cn

[R03] 只读变量
来源：http://tc.muxihuayi.cn

readonly PI=3.14
来源：http://zj.hnjuh.cn

[R04] 位置参数
来源：http://ow.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lc.yuntaijiaju.cn

[R05] 参数默认值
来源：http://ig.colortex.cn

name="${1:-default}"
来源：http://rb.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://fz.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wv.hnjuh.cn

[R07] if 判断文件
来源：http://tt.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qb.newstarts.cn

[R08] 数值比较
来源：http://mg.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cc.jianghongdianzi.cn

[R09] 字符串比较
来源：http://gb.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jx.hnjuh.cn

[R10] 正则匹配
来源：http://ys.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://og.jctech888.com.cn

[R11] case 多分支
来源：http://jk.panjiajie.cn


<!-- 参考信息 -->