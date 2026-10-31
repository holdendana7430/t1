代发 wailian999

TS:   crypto.randomUUID()
来源：http://hi.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://lk.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://ra.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://uu.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://du.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://lz.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rp.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cz.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hg.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nd.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hk.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bz.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yf.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qy.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://rg.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ow.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bh.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jf.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qd.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mi.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ed.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wh.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://el.panjiajie.cn

[P04] 求长度
来源：http://wr.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bc.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lf.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xa.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cu.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://pu.newstarts.cn

Go:   len(arr);  len(m)
来源：http://rm.szxytkj.cn

Ruby: x.length;  x.size
来源：http://de.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dh.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://kq.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://on.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bz.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ex.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nm.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jm.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mr.jctech888.com.cn

Ruby: a == b
来源：http://bj.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qb.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lt.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oo.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://xh.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zc.nszjky.cn

TS:   if (x == null) {}
来源：http://qk.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fj.newstarts.cn

Go:   if x == nil {}
来源：http://xk.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bk.asd995.cn

C#:   if (x is null) {}
来源：http://nh.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ak.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://po.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://jc.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uu.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hu.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zt.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dr.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lo.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hu.colortex.cn

[P08] 处理浮点精度问题
来源：http://uw.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ej.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gr.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nk.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ad.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://za.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://el.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nf.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yy.hahajie.cn

================================================================================
来源：http://ca.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lh.shtwfgs.cn

================================================================================
来源：http://pa.asd995.cn

[Q01] 创建表
来源：http://tp.panjiajie.cn

CREATE TABLE users (
来源：http://jy.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qw.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://tv.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://fv.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zs.haigaiapp.cn

);
来源：http://vq.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://xp.colortex.cn

CREATE TABLE orders (
来源：http://ji.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pv.muxihuayi.cn

user_id INT NOT NULL,
来源：http://ix.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://mp.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jt.nszjky.cn

);
来源：http://kl.hahajie.cn

[Q03] 增加列
来源：http://sa.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tn.haigaiapp.cn

[Q04] 修改列类型
来源：http://he.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xv.hahajie.cn

[Q05] 重命名列
来源：http://hb.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rr.huanxung.cn

[Q06] 删除列
来源：http://ug.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vi.shxzskj.cn

[Q07] 删除表
来源：http://rs.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://vm.9csxet.cn

[Q08] 创建普通索引
来源：http://sf.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gt.szsharing.cn

[Q09] 创建唯一索引
来源：http://dq.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iu.chemitech.net.cn

[Q10] 插入单行
来源：http://ml.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dp.panjiajie.cn

[Q11] 一次插入多行
来源：http://dp.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bg.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://kh.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yu.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sg.szsharing.cn

[Q13] 忽略重复插入
来源：http://qs.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ax.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://jg.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fg.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cw.yuntaijiaju.cn

[Q15] 查询全部
来源：http://ff.chemitech.net.cn

SELECT * FROM users;
来源：http://pq.nszjky.cn

[Q16] 查询指定列
来源：http://ld.yuexingan06.cn

SELECT id, name FROM users;
来源：http://mk.haigaiapp.cn

[Q17] 条件查询
来源：http://up.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hg.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://sz.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://at.shxzukj.cn

[Q19] 范围查询
来源：http://ge.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sy.huanxung.cn

[Q20] IN 列表
来源：http://zr.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ts.newstarts.cn

[Q21] 空值判断
来源：http://ce.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dd.huixiangedu.cn

[Q22] 排序
来源：http://ic.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fq.shxzukj.cn

[Q23] 分页
来源：http://if.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qq.hnjuh.cn

[Q24] 去重
来源：http://wm.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://ht.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://hs.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kq.asd995.cn

[Q26] 计数
来源：http://ww.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://sj.szsharing.cn

[Q27] 条件计数
来源：http://mt.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wa.hahajie.cn

[Q28] 求和与平均
来源：http://if.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bs.huanxung.cn

[Q29] 最大最小值
来源：http://vg.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bl.shxzskj.cn

[Q30] 分组统计
来源：http://px.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yu.hnjuh.cn

[Q31] 分组后过滤
来源：http://tq.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gu.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://wy.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://su.gzmigu.cn

[Q33] 多列分组
来源：http://ri.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://no.huanxung.cn

[Q34] 每组取第一条
来源：http://ue.nszjky.cn

SELECT * FROM (
来源：http://ff.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gc.nszjky.cn

) t WHERE rn = 1;
来源：http://gv.hahajie.cn

[Q35] 内连接
来源：http://ee.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ks.wgjwhj.cn

[Q36] 左连接
来源：http://dx.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://so.huixinmuqiang.cn

[Q37] 右连接
来源：http://sh.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jc.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://km.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://et.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://ip.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lc.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rc.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ix.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ac.hnjuh.cn

[Q41] 多表连接
来源：http://pr.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ne.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://on.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://pr.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://zx.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://oy.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://df.haigaiapp.cn

[Q43] 标量子查询
来源：http://sc.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xi.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://qr.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ce.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://qg.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fj.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wo.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bl.yuexingan06.cn

[Q47] 与平均值比较
来源：http://iw.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xi.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://sw.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dt.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://zy.gzmigu.cn

[Q49] 更新单行
来源：http://ip.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rj.521024.cn

[Q50] 批量更新
来源：http://kj.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zz.panjiajie.cn

[Q51] 用子查询更新
来源：http://hx.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qs.gzmigu.cn

[Q52] 删除指定行
来源：http://le.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://zz.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://ov.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ra.wgjwhj.cn

[Q54] 清空表
来源：http://kk.nszjky.cn

TRUNCATE TABLE logs;
来源：http://jm.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://xu.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://do.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://rd.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yu.nszjky.cn

[Q57] 行号
来源：http://bz.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://an.muxihuayi.cn

[Q58] 累计求和
来源：http://lt.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gl.521024.cn

[Q59] 分组内累计
来源：http://za.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fu.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://ro.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lg.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://or.szsharing.cn

[Q61] 移动平均
来源：http://lv.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jj.shxzskj.cn

[Q62] 分组占比
来源：http://ao.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ew.panjiajie.cn

[Q63] 开启事务
来源：http://wk.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nr.szxytkj.cn

[Q64] 提交事务
来源：http://rq.nicolike.cn

COMMIT;
来源：http://uu.szxytkj.cn

[Q65] 回滚事务
来源：http://ge.asd995.cn

ROLLBACK;
来源：http://fk.hnjuh.cn

[Q66] 行锁查询
来源：http://vk.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sq.huanxung.cn

[Q67] 设置隔离级别
来源：http://wf.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aj.huixiangedu.cn

[Q68] 保存点
来源：http://pu.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://pr.gzmigu.cn

ROLLBACK TO sp1;
来源：http://wi.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://xi.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cn.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://yt.jctech888.com.cn

ANALYZE TABLE users;
来源：http://nz.chemitech.net.cn

[Q71] 查看建表语句
来源：http://lw.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yp.gzmigu.cn

[Q72] 查看索引
来源：http://xf.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://yn.muxihuayi.cn

[Q73] 查看表状态
来源：http://qy.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zp.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ez.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qk.hahajie.cn

[Q75] 日期格式化
来源：http://bh.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ec.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tf.jianghongdianzi.cn

[Q76] 按天统计
来源：http://mg.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zh.huixiangedu.cn

[Q77] 时间加减
来源：http://ou.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xc.yuntaijiaju.cn

[Q78] 当前时间
来源：http://xc.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://el.szsharing.cn

[Q79] 字符串拼接
来源：http://ru.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qo.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://mk.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nx.nszjky.cn

[Q81] 字符串替换
来源：http://yw.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xx.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://sd.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pv.hahajie.cn

[Q83] 大小写转换
来源：http://mv.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bv.lnxyls.cn

[Q84] 去除首尾空格
来源：http://nj.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://yb.shxzskj.cn

[Q85] 数值取整
来源：http://vl.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vu.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://oj.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nl.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://km.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://on.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://gs.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ay.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bk.panjiajie.cn

[Q89] 判断表是否存在
来源：http://to.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wm.szxytkj.cn

[Q90] 生成序号列
来源：http://hs.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xy.asd995.cn

================================================================================
来源：http://ul.shtwfgs.cn

R. Bash 专题
来源：http://yi.lnxyls.cn

================================================================================
来源：http://jh.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://ll.yuexingan06.cn

#!/usr/bin/env bash
来源：http://cu.hahajie.cn

set -euo pipefail
来源：http://hl.9csxet.cn

[R02] 变量赋值与使用
来源：http://if.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://yw.shxzskj.cn

[R03] 只读变量
来源：http://dx.huanxung.cn

readonly PI=3.14
来源：http://pl.9csxet.cn

[R04] 位置参数
来源：http://cn.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pz.hahajie.cn

[R05] 参数默认值
来源：http://wf.nicolike.cn

name="${1:-default}"
来源：http://dy.shxzukj.cn

[R06] 判断命令是否存在
来源：http://gm.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wk.shxzskj.cn

[R07] if 判断文件
来源：http://mu.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rf.szxytkj.cn

[R08] 数值比较
来源：http://wn.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ci.hahajie.cn

[R09] 字符串比较
来源：http://av.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ca.yuntaijiaju.cn

[R10] 正则匹配
来源：http://oz.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yu.huixinmuqiang.cn

[R11] case 多分支
来源：http://aw.szxytkj.cn


<!-- 参考信息 -->