代发 wailian999

TS:   // child_process / cluster 模块
来源：http://db.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fw.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ae.shxzskj.cn

Ruby: // fork 块
来源：http://vx.muxihuayi.cn

C#:   Parallel.For
来源：http://yq.lnxyls.cn

================================================================================
来源：http://ua.wgjwhj.cn

P. 常用工具函数
来源：http://pb.panjiajie.cn

================================================================================
来源：http://cb.hahajie.cn

[P01] 生成 UUID
来源：http://pi.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://vl.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qo.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://ep.szsharing.cn

TS:   crypto.randomUUID()
来源：http://mx.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://bt.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://vc.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://ir.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ug.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://do.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://md.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mm.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://an.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hl.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yc.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vi.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yv.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cc.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://mo.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://up.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kb.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bf.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ta.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tk.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xu.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rh.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lx.jianghongdianzi.cn

[P04] 求长度
来源：http://ki.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cq.huixiangedu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yw.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ii.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://va.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://dd.nicolike.cn

Go:   len(arr);  len(m)
来源：http://pe.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://kb.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gh.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://sf.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sx.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://os.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nc.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qy.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://br.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pd.huanxung.cn

Ruby: a == b
来源：http://as.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pm.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lt.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eu.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://jk.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zg.huanxung.cn

TS:   if (x == null) {}
来源：http://nz.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fq.bookmarksfly.cn

Go:   if x == nil {}
来源：http://sh.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zk.shxzukj.cn

C#:   if (x is null) {}
来源：http://ae.bjjhwx.cn

[P07] 防抖与节流
来源：http://pz.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ib.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://sg.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wl.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oi.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kw.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cm.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ew.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hb.521024.cn

[P08] 处理浮点精度问题
来源：http://it.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tb.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://by.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yu.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mq.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://as.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ai.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yg.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pc.bookmarksfly.cn

================================================================================
来源：http://jh.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xo.huanxung.cn

================================================================================
来源：http://tr.jctech888.com.cn

[Q01] 创建表
来源：http://lr.9csxet.cn

CREATE TABLE users (
来源：http://ku.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ez.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://jj.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://mk.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iu.lnxyls.cn

);
来源：http://lj.9csxet.cn

[Q02] 创建带外键的表
来源：http://eq.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://xj.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qk.wgjwhj.cn

user_id INT NOT NULL,
来源：http://zw.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ag.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wm.lnxyls.cn

);
来源：http://lu.nszjky.cn

[Q03] 增加列
来源：http://mx.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dc.muxihuayi.cn

[Q04] 修改列类型
来源：http://zi.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ru.gzmigu.cn

[Q05] 重命名列
来源：http://fe.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ud.colortex.cn

[Q06] 删除列
来源：http://kv.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qy.szsharing.cn

[Q07] 删除表
来源：http://bo.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://xu.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ws.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oo.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://uc.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dh.chemitech.net.cn

[Q10] 插入单行
来源：http://km.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://en.shxzukj.cn

[Q11] 一次插入多行
来源：http://sz.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gi.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ov.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pa.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tt.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://ih.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uw.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://ma.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zz.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qv.jctech888.com.cn

[Q15] 查询全部
来源：http://sj.yuntaijiaju.cn

SELECT * FROM users;
来源：http://kf.muxihuayi.cn

[Q16] 查询指定列
来源：http://qp.jctech888.com.cn

SELECT id, name FROM users;
来源：http://ph.yuntaijiaju.cn

[Q17] 条件查询
来源：http://hp.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qt.colortex.cn

[Q18] 模糊匹配
来源：http://mw.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qg.panjiajie.cn

[Q19] 范围查询
来源：http://zq.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yj.shtwfgs.cn

[Q20] IN 列表
来源：http://kr.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dy.panjiajie.cn

[Q21] 空值判断
来源：http://kr.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pj.huixinmuqiang.cn

[Q22] 排序
来源：http://gs.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oz.521024.cn

[Q23] 分页
来源：http://fn.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pv.yuexingan06.cn

[Q24] 去重
来源：http://nl.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://kz.colortex.cn

[Q25] 只取前 N 条
来源：http://xb.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lx.asd995.cn

[Q26] 计数
来源：http://fs.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://cf.9csxet.cn

[Q27] 条件计数
来源：http://eu.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tw.lnxyls.cn

[Q28] 求和与平均
来源：http://ss.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tv.muxihuayi.cn

[Q29] 最大最小值
来源：http://ip.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kz.bjjhwx.cn

[Q30] 分组统计
来源：http://de.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hy.shxzukj.cn

[Q31] 分组后过滤
来源：http://qk.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wj.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://xf.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ei.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kg.jianghongdianzi.cn

[Q33] 多列分组
来源：http://gh.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yt.asd995.cn

[Q34] 每组取第一条
来源：http://vd.yuntaijiaju.cn

SELECT * FROM (
来源：http://qk.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aw.colortex.cn

) t WHERE rn = 1;
来源：http://gg.shtwfgs.cn

[Q35] 内连接
来源：http://ag.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ke.wgjwhj.cn

[Q36] 左连接
来源：http://zi.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qn.yuexingan06.cn

[Q37] 右连接
来源：http://wo.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cd.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gc.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xs.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://dw.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ry.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cj.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cr.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://px.muxihuayi.cn

[Q41] 多表连接
来源：http://qy.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vt.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://hh.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://wc.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://tn.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://nm.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yl.gzmigu.cn

[Q43] 标量子查询
来源：http://rk.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://er.szsharing.cn

[Q44] IN 子查询
来源：http://bv.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://td.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://ot.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rg.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vk.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hq.asd995.cn

[Q47] 与平均值比较
来源：http://dm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lv.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ut.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vb.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://bh.jianghongdianzi.cn

[Q49] 更新单行
来源：http://re.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hp.9csxet.cn

[Q50] 批量更新
来源：http://xh.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oh.nszjky.cn

[Q51] 用子查询更新
来源：http://vs.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://if.gzmigu.cn

[Q52] 删除指定行
来源：http://ti.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://da.jctech888.com.cn

[Q53] 按条件删除
来源：http://ce.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lx.9csxet.cn

[Q54] 清空表
来源：http://vy.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://jg.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://rk.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oq.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://ra.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://av.9csxet.cn

[Q57] 行号
来源：http://ex.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rp.asd995.cn

[Q58] 累计求和
来源：http://en.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tg.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://fd.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://js.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://av.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zj.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xx.huixinmuqiang.cn

[Q61] 移动平均
来源：http://ty.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aj.muxihuayi.cn

[Q62] 分组占比
来源：http://bd.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bc.lnxyls.cn

[Q63] 开启事务
来源：http://yv.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xx.szxytkj.cn

[Q64] 提交事务
来源：http://av.szxytkj.cn

COMMIT;
来源：http://nb.nszjky.cn

[Q65] 回滚事务
来源：http://ld.colortex.cn

ROLLBACK;
来源：http://ge.huixiangedu.cn

[Q66] 行锁查询
来源：http://ji.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kl.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://rb.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dh.colortex.cn

[Q68] 保存点
来源：http://zl.haigaiapp.cn

SAVEPOINT sp1;
来源：http://uy.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://wg.asd995.cn

[Q69] 查看执行计划
来源：http://av.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wv.nszjky.cn

[Q70] 更新统计信息
来源：http://so.shxzskj.cn

ANALYZE TABLE users;
来源：http://zy.haigaiapp.cn

[Q71] 查看建表语句
来源：http://fp.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iv.haigaiapp.cn

[Q72] 查看索引
来源：http://ij.hahajie.cn

SHOW INDEX FROM users;
来源：http://ws.colortex.cn

[Q73] 查看表状态
来源：http://lv.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ah.panjiajie.cn

[Q74] 强制使用索引
来源：http://io.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ra.huixiangedu.cn

[Q75] 日期格式化
来源：http://gh.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ez.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://at.nicolike.cn

[Q76] 按天统计
来源：http://uz.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jp.szxytkj.cn

[Q77] 时间加减
来源：http://zi.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ka.bjjhwx.cn

[Q78] 当前时间
来源：http://bc.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://os.lnxyls.cn

[Q79] 字符串拼接
来源：http://iw.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nl.huanxung.cn

[Q80] 字符串截取
来源：http://if.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fq.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://ao.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mo.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://ep.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://py.gzmigu.cn

[Q83] 大小写转换
来源：http://qy.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ld.huanxung.cn

[Q84] 去除首尾空格
来源：http://zi.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ea.haigaiapp.cn

[Q85] 数值取整
来源：http://ar.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bk.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ru.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ks.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://fm.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://or.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://nq.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lj.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hq.lnxyls.cn

[Q89] 判断表是否存在
来源：http://xa.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mc.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://qf.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fv.huixinmuqiang.cn

================================================================================
来源：http://rj.muxihuayi.cn

R. Bash 专题
来源：http://fy.colortex.cn

================================================================================
来源：http://kd.gzmigu.cn

[R01] shebang 与严格模式
来源：http://vi.bjjhwx.cn

#!/usr/bin/env bash
来源：http://hi.chemitech.net.cn

set -euo pipefail
来源：http://zu.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ch.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://cj.haigaiapp.cn

[R03] 只读变量
来源：http://sb.shxzskj.cn

readonly PI=3.14
来源：http://uj.panjiajie.cn

[R04] 位置参数
来源：http://gb.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pe.panjiajie.cn

[R05] 参数默认值
来源：http://ip.huixiangedu.cn


<!-- 参考信息 -->