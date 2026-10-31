代发 wailian999

TS:   // child_process / cluster 模块
来源：http://gl.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zv.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vr.huixinmuqiang.cn

Ruby: // fork 块
来源：http://cl.9csxet.cn

C#:   Parallel.For
来源：http://fv.colortex.cn

================================================================================
来源：http://zw.huixiangedu.cn

P. 常用工具函数
来源：http://xd.bjjhwx.cn

================================================================================
来源：http://xl.shtwfgs.cn

[P01] 生成 UUID
来源：http://pa.asd995.cn

Py:   str(uuid.uuid4())
来源：http://rc.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fy.nszjky.cn

JS:   crypto.randomUUID()
来源：http://kl.hahajie.cn

TS:   crypto.randomUUID()
来源：http://st.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://oh.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://jw.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://pq.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://la.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://bw.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iy.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xf.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uc.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ju.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ah.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lm.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://en.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xf.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://kh.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ye.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dq.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nx.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vp.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://co.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sw.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kb.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eb.bookmarksfly.cn

[P04] 求长度
来源：http://tb.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://us.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://af.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ji.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://cl.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://go.colortex.cn

Ruby: x.length;  x.size
来源：http://or.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xt.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://lf.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jp.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ul.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://td.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wo.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ja.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oh.huanxung.cn

Ruby: a == b
来源：http://kc.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ky.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mf.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gv.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ll.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qp.shxzukj.cn

TS:   if (x == null) {}
来源：http://dd.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lt.newstarts.cn

Go:   if x == nil {}
来源：http://yk.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mh.9csxet.cn

C#:   if (x is null) {}
来源：http://qa.hahajie.cn

[P07] 防抖与节流
来源：http://vh.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eq.colortex.cn

PHP:  // 手写时间戳比较
来源：http://le.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gc.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zr.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cm.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ad.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kd.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lp.asd995.cn

[P08] 处理浮点精度问题
来源：http://qy.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rd.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oo.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ao.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qr.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sq.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nn.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gw.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pn.colortex.cn

================================================================================
来源：http://rb.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://hn.jctech888.com.cn

[Q01] 创建表
来源：http://db.9csxet.cn

CREATE TABLE users (
来源：http://ri.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://od.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://ru.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://zj.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qu.panjiajie.cn

);
来源：http://ud.hahajie.cn

[Q02] 创建带外键的表
来源：http://ai.huanxung.cn

CREATE TABLE orders (
来源：http://qx.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://na.lnxyls.cn

user_id INT NOT NULL,
来源：http://lk.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://qp.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ws.nszjky.cn

);
来源：http://xl.lnxyls.cn

[Q03] 增加列
来源：http://bw.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lj.hahajie.cn

[Q04] 修改列类型
来源：http://os.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kc.shtwfgs.cn

[Q05] 重命名列
来源：http://mr.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ra.haigaiapp.cn

[Q06] 删除列
来源：http://sk.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wz.huixinmuqiang.cn

[Q07] 删除表
来源：http://pe.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://nu.bjjhwx.cn

[Q08] 创建普通索引
来源：http://hm.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yj.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://xd.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ai.colortex.cn

[Q10] 插入单行
来源：http://kk.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jj.muxihuayi.cn

[Q11] 一次插入多行
来源：http://az.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://so.colortex.cn

[Q12] 插入后取自增 ID
来源：http://hb.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oj.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ps.colortex.cn

[Q13] 忽略重复插入
来源：http://pu.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xg.521024.cn

[Q14] 存在则更新（upsert）
来源：http://id.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vf.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zc.bjjhwx.cn

[Q15] 查询全部
来源：http://yh.colortex.cn

SELECT * FROM users;
来源：http://uy.bjjhwx.cn

[Q16] 查询指定列
来源：http://ob.shxzskj.cn

SELECT id, name FROM users;
来源：http://ei.shxzskj.cn

[Q17] 条件查询
来源：http://tx.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zh.521024.cn

[Q18] 模糊匹配
来源：http://xg.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tc.huixiangedu.cn

[Q19] 范围查询
来源：http://zk.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zu.shxzskj.cn

[Q20] IN 列表
来源：http://lw.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yw.jianghongdianzi.cn

[Q21] 空值判断
来源：http://av.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fy.shxzskj.cn

[Q22] 排序
来源：http://wn.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tx.szxytkj.cn

[Q23] 分页
来源：http://kf.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gy.chemitech.net.cn

[Q24] 去重
来源：http://wy.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://kj.gzmigu.cn

[Q25] 只取前 N 条
来源：http://gd.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sy.nszjky.cn

[Q26] 计数
来源：http://cq.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://yf.muxihuayi.cn

[Q27] 条件计数
来源：http://je.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nd.haigaiapp.cn

[Q28] 求和与平均
来源：http://jb.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pp.bookmarksfly.cn

[Q29] 最大最小值
来源：http://ub.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ld.szsharing.cn

[Q30] 分组统计
来源：http://dt.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rc.shxzukj.cn

[Q31] 分组后过滤
来源：http://xr.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nq.colortex.cn

[Q32] 分组拼接字符串
来源：http://pq.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cy.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yl.hnjuh.cn

[Q33] 多列分组
来源：http://gd.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ht.hnjuh.cn

[Q34] 每组取第一条
来源：http://ls.hnjuh.cn

SELECT * FROM (
来源：http://ju.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bq.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://ky.9csxet.cn

[Q35] 内连接
来源：http://yo.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ko.newstarts.cn

[Q36] 左连接
来源：http://br.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lx.jianghongdianzi.cn

[Q37] 右连接
来源：http://vp.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fu.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ky.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oc.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://kb.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nd.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fu.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vu.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dx.wgjwhj.cn

[Q41] 多表连接
来源：http://my.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://me.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://qd.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://nd.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://rj.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://eo.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wd.bjjhwx.cn

[Q43] 标量子查询
来源：http://jw.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pg.asd995.cn

[Q44] IN 子查询
来源：http://mp.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://co.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://ck.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://au.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ps.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jv.panjiajie.cn

[Q47] 与平均值比较
来源：http://qz.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ul.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://ak.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gy.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://vs.wgjwhj.cn

[Q49] 更新单行
来源：http://fw.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vs.asd995.cn

[Q50] 批量更新
来源：http://io.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ts.yuexingan06.cn

[Q51] 用子查询更新
来源：http://jl.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gi.huanxung.cn

[Q52] 删除指定行
来源：http://as.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://xc.muxihuayi.cn

[Q53] 按条件删除
来源：http://re.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://to.hahajie.cn

[Q54] 清空表
来源：http://vp.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://wi.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://lr.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kf.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ez.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://js.yuexingan06.cn

[Q57] 行号
来源：http://ag.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lj.jctech888.com.cn

[Q58] 累计求和
来源：http://bs.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vi.colortex.cn

[Q59] 分组内累计
来源：http://kc.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://it.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://qp.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://do.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ad.panjiajie.cn

[Q61] 移动平均
来源：http://jh.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qk.chemitech.net.cn

[Q62] 分组占比
来源：http://ma.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xn.wgjwhj.cn

[Q63] 开启事务
来源：http://ex.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ef.bookmarksfly.cn

[Q64] 提交事务
来源：http://sc.shxzukj.cn

COMMIT;
来源：http://pj.shxzskj.cn

[Q65] 回滚事务
来源：http://np.yuexingan06.cn

ROLLBACK;
来源：http://rp.nszjky.cn

[Q66] 行锁查询
来源：http://pu.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dw.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://fp.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ev.yuexingan06.cn

[Q68] 保存点
来源：http://zb.muxihuayi.cn

SAVEPOINT sp1;
来源：http://gp.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://ct.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://ie.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ek.wgjwhj.cn

[Q70] 更新统计信息
来源：http://ss.panjiajie.cn

ANALYZE TABLE users;
来源：http://cj.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://mi.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qz.shtwfgs.cn

[Q72] 查看索引
来源：http://nq.521024.cn

SHOW INDEX FROM users;
来源：http://nr.panjiajie.cn

[Q73] 查看表状态
来源：http://qn.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sb.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://dx.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wv.yuexingan06.cn

[Q75] 日期格式化
来源：http://al.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zg.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hl.gzmigu.cn

[Q76] 按天统计
来源：http://vo.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lz.szsharing.cn

[Q77] 时间加减
来源：http://pa.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ra.chemitech.net.cn

[Q78] 当前时间
来源：http://qq.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://it.panjiajie.cn

[Q79] 字符串拼接
来源：http://dk.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nc.colortex.cn

[Q80] 字符串截取
来源：http://oj.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uf.nszjky.cn

[Q81] 字符串替换
来源：http://hs.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sg.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://gw.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ms.haigaiapp.cn

[Q83] 大小写转换
来源：http://nw.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ud.szxytkj.cn

[Q84] 去除首尾空格
来源：http://cz.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://ju.shxzukj.cn

[Q85] 数值取整
来源：http://fo.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://co.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://gv.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://th.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://oc.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ik.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://dx.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gr.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sq.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://ma.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rz.colortex.cn

[Q90] 生成序号列
来源：http://eg.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ep.nicolike.cn

================================================================================
来源：http://jr.shtwfgs.cn

R. Bash 专题
来源：http://lc.bookmarksfly.cn

================================================================================
来源：http://uv.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://os.gzmigu.cn

#!/usr/bin/env bash
来源：http://fj.huixiangedu.cn

set -euo pipefail
来源：http://yn.nszjky.cn

[R02] 变量赋值与使用
来源：http://zp.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://is.shxzskj.cn

[R03] 只读变量
来源：http://jy.asd995.cn

readonly PI=3.14
来源：http://fx.huanxung.cn

[R04] 位置参数
来源：http://vz.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gs.huanxung.cn

[R05] 参数默认值
来源：http://yu.bookmarksfly.cn


<!-- 参考信息 -->