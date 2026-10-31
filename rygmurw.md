代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://pe.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xo.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://gw.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://jx.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hd.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qf.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://ym.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nk.szxytkj.cn

[O06] 使用进程池
来源：http://ux.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://er.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ey.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://aq.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://rs.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xw.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vc.yuexingan06.cn

Ruby: // fork 块
来源：http://qw.nszjky.cn

C#:   Parallel.For
来源：http://xd.chemitech.net.cn

================================================================================
来源：http://xn.wgjwhj.cn

P. 常用工具函数
来源：http://bi.asd995.cn

================================================================================
来源：http://rb.panjiajie.cn

[P01] 生成 UUID
来源：http://wo.colortex.cn

Py:   str(uuid.uuid4())
来源：http://jw.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wn.colortex.cn

JS:   crypto.randomUUID()
来源：http://jj.szsharing.cn

TS:   crypto.randomUUID()
来源：http://qr.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://rj.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://it.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://vz.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://yt.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://jn.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://te.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gv.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ns.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eu.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tl.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ul.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ae.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zi.huanxung.cn

[P03] 生成短随机字符串
来源：http://po.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://el.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nj.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://re.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hm.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://co.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bj.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dh.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nd.colortex.cn

[P04] 求长度
来源：http://vf.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gs.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rj.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fh.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ci.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://wp.asd995.cn

Go:   len(arr);  len(m)
来源：http://uw.nicolike.cn

Ruby: x.length;  x.size
来源：http://bn.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bz.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://qw.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ey.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yn.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sp.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nh.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ll.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jt.huixiangedu.cn

Ruby: a == b
来源：http://cr.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://za.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rc.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gi.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://va.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gb.nicolike.cn

TS:   if (x == null) {}
来源：http://se.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jy.newstarts.cn

Go:   if x == nil {}
来源：http://tm.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hv.521024.cn

C#:   if (x is null) {}
来源：http://ve.colortex.cn

[P07] 防抖与节流
来源：http://ri.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yi.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://bi.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ii.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ib.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zh.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dr.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://et.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://kw.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vg.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://di.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ii.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cq.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tr.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qu.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ur.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vv.bjjhwx.cn

================================================================================
来源：http://dh.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ue.bjjhwx.cn

================================================================================
来源：http://oh.wgjwhj.cn

[Q01] 创建表
来源：http://gr.nicolike.cn

CREATE TABLE users (
来源：http://bg.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bj.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://jh.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://md.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://in.jianghongdianzi.cn

);
来源：http://rh.lnxyls.cn

[Q02] 创建带外键的表
来源：http://jl.521024.cn

CREATE TABLE orders (
来源：http://ya.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iz.panjiajie.cn

user_id INT NOT NULL,
来源：http://jd.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://jh.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tk.chemitech.net.cn

);
来源：http://xd.hahajie.cn

[Q03] 增加列
来源：http://yd.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ic.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://zs.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://is.9csxet.cn

[Q05] 重命名列
来源：http://zk.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kd.hahajie.cn

[Q06] 删除列
来源：http://hf.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hp.9csxet.cn

[Q07] 删除表
来源：http://if.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://ak.huixiangedu.cn

[Q08] 创建普通索引
来源：http://jy.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zw.lnxyls.cn

[Q09] 创建唯一索引
来源：http://li.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fm.haigaiapp.cn

[Q10] 插入单行
来源：http://lw.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xe.chemitech.net.cn

[Q11] 一次插入多行
来源：http://vw.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://do.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://pl.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ga.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sh.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ly.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jb.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://tt.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vo.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://os.gzmigu.cn

[Q15] 查询全部
来源：http://at.szxytkj.cn

SELECT * FROM users;
来源：http://gb.nicolike.cn

[Q16] 查询指定列
来源：http://ij.shxzskj.cn

SELECT id, name FROM users;
来源：http://dy.9csxet.cn

[Q17] 条件查询
来源：http://ev.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ug.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://es.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wx.panjiajie.cn

[Q19] 范围查询
来源：http://ig.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bb.shxzukj.cn

[Q20] IN 列表
来源：http://qm.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mx.shxzukj.cn

[Q21] 空值判断
来源：http://ev.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gx.shxzskj.cn

[Q22] 排序
来源：http://iz.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eu.haigaiapp.cn

[Q23] 分页
来源：http://rn.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yj.shxzukj.cn

[Q24] 去重
来源：http://zt.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://uv.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://if.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zm.muxihuayi.cn

[Q26] 计数
来源：http://yn.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://vc.colortex.cn

[Q27] 条件计数
来源：http://sd.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://at.hahajie.cn

[Q28] 求和与平均
来源：http://zt.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zx.newstarts.cn

[Q29] 最大最小值
来源：http://uf.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ec.nicolike.cn

[Q30] 分组统计
来源：http://ew.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aw.asd995.cn

[Q31] 分组后过滤
来源：http://tz.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cd.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://cf.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://po.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cm.9csxet.cn

[Q33] 多列分组
来源：http://df.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dg.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://hp.nszjky.cn

SELECT * FROM (
来源：http://gw.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qj.gzmigu.cn

) t WHERE rn = 1;
来源：http://ov.bookmarksfly.cn

[Q35] 内连接
来源：http://cx.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wb.colortex.cn

[Q36] 左连接
来源：http://xi.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ln.bookmarksfly.cn

[Q37] 右连接
来源：http://bd.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ur.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ol.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ua.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://yl.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nn.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cn.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eh.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vw.haigaiapp.cn

[Q41] 多表连接
来源：http://td.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rd.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://rv.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ou.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://as.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://yh.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ix.gzmigu.cn

[Q43] 标量子查询
来源：http://sw.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dp.jctech888.com.cn

[Q44] IN 子查询
来源：http://tw.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gt.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ry.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rb.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wp.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://au.colortex.cn

[Q47] 与平均值比较
来源：http://qo.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ut.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://qg.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qu.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ib.shxzukj.cn

[Q49] 更新单行
来源：http://gy.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ex.jctech888.com.cn

[Q50] 批量更新
来源：http://qj.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cc.jctech888.com.cn

[Q51] 用子查询更新
来源：http://vr.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gn.9csxet.cn

[Q52] 删除指定行
来源：http://yc.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://sv.jctech888.com.cn

[Q53] 按条件删除
来源：http://sp.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vy.newstarts.cn

[Q54] 清空表
来源：http://ke.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://yz.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://gq.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ye.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://as.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nm.szsharing.cn

[Q57] 行号
来源：http://xn.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pm.nszjky.cn

[Q58] 累计求和
来源：http://ka.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nm.gzmigu.cn

[Q59] 分组内累计
来源：http://cl.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yi.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://yw.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yf.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ww.bjjhwx.cn

[Q61] 移动平均
来源：http://fz.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qz.colortex.cn

[Q62] 分组占比
来源：http://yg.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lu.newstarts.cn

[Q63] 开启事务
来源：http://kk.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zo.yuntaijiaju.cn

[Q64] 提交事务
来源：http://my.huixiangedu.cn

COMMIT;
来源：http://rp.nszjky.cn

[Q65] 回滚事务
来源：http://qb.huixinmuqiang.cn

ROLLBACK;
来源：http://rs.huixiangedu.cn

[Q66] 行锁查询
来源：http://nk.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zt.panjiajie.cn

[Q67] 设置隔离级别
来源：http://nd.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://go.9csxet.cn

[Q68] 保存点
来源：http://ln.szxytkj.cn

SAVEPOINT sp1;
来源：http://ny.gzmigu.cn

ROLLBACK TO sp1;
来源：http://gy.asd995.cn

[Q69] 查看执行计划
来源：http://ty.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qf.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ra.shxzukj.cn

ANALYZE TABLE users;
来源：http://gr.asd995.cn

[Q71] 查看建表语句
来源：http://qi.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wx.asd995.cn

[Q72] 查看索引
来源：http://pk.szsharing.cn

SHOW INDEX FROM users;
来源：http://hn.lnxyls.cn

[Q73] 查看表状态
来源：http://uf.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dv.nszjky.cn

[Q74] 强制使用索引
来源：http://ej.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iz.hnjuh.cn

[Q75] 日期格式化
来源：http://fs.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://la.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bu.hnjuh.cn

[Q76] 按天统计
来源：http://iy.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yt.huixinmuqiang.cn

[Q77] 时间加减
来源：http://kt.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wf.muxihuayi.cn

[Q78] 当前时间
来源：http://dz.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://es.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://dr.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kq.haigaiapp.cn

[Q80] 字符串截取
来源：http://rz.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ca.haigaiapp.cn

[Q81] 字符串替换
来源：http://or.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ll.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://pk.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bv.muxihuayi.cn

[Q83] 大小写转换
来源：http://de.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mc.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://jq.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://dg.huanxung.cn

[Q85] 数值取整
来源：http://vn.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oz.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://jc.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pj.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ij.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kr.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://pn.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lm.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xv.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://rw.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rx.szxytkj.cn

[Q90] 生成序号列
来源：http://js.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xc.jianghongdianzi.cn

================================================================================
来源：http://hi.bookmarksfly.cn


<!-- 参考信息 -->