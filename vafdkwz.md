代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qp.nicolike.cn

JS:   async function f() { await g(); }
来源：http://ua.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jp.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ey.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zm.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bz.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://uc.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://qg.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://xl.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://et.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://zk.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://hu.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nr.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sk.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://qa.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://il.lnxyls.cn

[O06] 使用进程池
来源：http://xo.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sz.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ig.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://uv.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://ro.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yb.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bc.bookmarksfly.cn

Ruby: // fork 块
来源：http://by.lnxyls.cn

C#:   Parallel.For
来源：http://pe.jctech888.com.cn

================================================================================
来源：http://tb.asd995.cn

P. 常用工具函数
来源：http://rq.haigaiapp.cn

================================================================================
来源：http://li.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://ax.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://ol.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wx.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://gv.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ge.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://hv.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://pm.521024.cn

Ruby: SecureRandom.uuid
来源：http://bg.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://hu.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://jl.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yv.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nr.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gv.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vs.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://to.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lh.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vr.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xz.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://qz.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rr.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mg.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qp.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nk.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gf.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://if.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nt.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ur.szsharing.cn

[P04] 求长度
来源：http://ez.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yt.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iu.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lh.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wq.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://oj.hahajie.cn

Go:   len(arr);  len(m)
来源：http://fl.521024.cn

Ruby: x.length;  x.size
来源：http://xp.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hs.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://kj.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ld.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bt.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qq.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hk.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kx.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ye.muxihuayi.cn

Ruby: a == b
来源：http://dc.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ya.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nu.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yu.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://qk.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://by.hnjuh.cn

TS:   if (x == null) {}
来源：http://sx.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zg.newstarts.cn

Go:   if x == nil {}
来源：http://hh.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://os.muxihuayi.cn

C#:   if (x is null) {}
来源：http://ay.newstarts.cn

[P07] 防抖与节流
来源：http://nm.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cn.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://ml.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zg.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mp.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lm.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rk.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jg.colortex.cn

[P08] 处理浮点精度问题
来源：http://kc.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cb.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ty.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kt.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aq.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://br.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jj.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://an.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ms.panjiajie.cn

================================================================================
来源：http://wo.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yi.haigaiapp.cn

================================================================================
来源：http://by.asd995.cn

[Q01] 创建表
来源：http://zk.panjiajie.cn

CREATE TABLE users (
来源：http://ji.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zx.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://yi.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://bd.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sf.bjjhwx.cn

);
来源：http://ov.521024.cn

[Q02] 创建带外键的表
来源：http://ed.huixiangedu.cn

CREATE TABLE orders (
来源：http://op.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zg.bjjhwx.cn

user_id INT NOT NULL,
来源：http://md.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://yp.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ug.newstarts.cn

);
来源：http://qx.shtwfgs.cn

[Q03] 增加列
来源：http://zh.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://um.haigaiapp.cn

[Q04] 修改列类型
来源：http://dl.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ku.nicolike.cn

[Q05] 重命名列
来源：http://cq.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zm.hnjuh.cn

[Q06] 删除列
来源：http://za.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cj.nszjky.cn

[Q07] 删除表
来源：http://rd.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://gp.bjjhwx.cn

[Q08] 创建普通索引
来源：http://iw.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jp.shxzukj.cn

[Q09] 创建唯一索引
来源：http://gx.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gs.shxzukj.cn

[Q10] 插入单行
来源：http://pd.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vk.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://wq.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vj.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://tn.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dd.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bp.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://yw.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nw.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://jt.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ac.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://as.9csxet.cn

[Q15] 查询全部
来源：http://ca.szsharing.cn

SELECT * FROM users;
来源：http://kx.521024.cn

[Q16] 查询指定列
来源：http://kj.huixiangedu.cn

SELECT id, name FROM users;
来源：http://vq.521024.cn

[Q17] 条件查询
来源：http://rn.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://im.wgjwhj.cn

[Q18] 模糊匹配
来源：http://pu.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ac.hnjuh.cn

[Q19] 范围查询
来源：http://tq.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vw.9csxet.cn

[Q20] IN 列表
来源：http://bt.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xm.nszjky.cn

[Q21] 空值判断
来源：http://jr.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xo.haigaiapp.cn

[Q22] 排序
来源：http://lf.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qh.jianghongdianzi.cn

[Q23] 分页
来源：http://ve.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qf.huanxung.cn

[Q24] 去重
来源：http://vk.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://iv.shxzukj.cn

[Q25] 只取前 N 条
来源：http://fq.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bu.gzmigu.cn

[Q26] 计数
来源：http://rh.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://no.huixiangedu.cn

[Q27] 条件计数
来源：http://jv.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.shxzukj.cn

[Q28] 求和与平均
来源：http://kl.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rv.hnjuh.cn

[Q29] 最大最小值
来源：http://gf.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pg.wgjwhj.cn

[Q30] 分组统计
来源：http://lg.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pa.nicolike.cn

[Q31] 分组后过滤
来源：http://ta.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oe.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://pw.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eh.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://le.yuexingan06.cn

[Q33] 多列分组
来源：http://ui.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ns.huixiangedu.cn

[Q34] 每组取第一条
来源：http://km.szsharing.cn

SELECT * FROM (
来源：http://wc.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://er.jctech888.com.cn

) t WHERE rn = 1;
来源：http://ts.szsharing.cn

[Q35] 内连接
来源：http://xh.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zq.9csxet.cn

[Q36] 左连接
来源：http://ie.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fj.haigaiapp.cn

[Q37] 右连接
来源：http://yd.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gw.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pa.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ec.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://mg.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tm.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zc.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pf.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zi.521024.cn

[Q41] 多表连接
来源：http://hg.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nr.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://lc.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://ob.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://ps.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://kt.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ji.huixiangedu.cn

[Q43] 标量子查询
来源：http://hr.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gp.hahajie.cn

[Q44] IN 子查询
来源：http://vt.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lt.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ck.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://to.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fa.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kj.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://wv.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iv.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://iw.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kq.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://gf.yuexingan06.cn

[Q49] 更新单行
来源：http://rx.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pp.shxzukj.cn

[Q50] 批量更新
来源：http://ge.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ui.colortex.cn

[Q51] 用子查询更新
来源：http://ki.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.wgjwhj.cn

[Q52] 删除指定行
来源：http://pe.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://fn.521024.cn

[Q53] 按条件删除
来源：http://vi.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://br.yuexingan06.cn

[Q54] 清空表
来源：http://ht.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://vq.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ae.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qp.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://og.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vm.huixinmuqiang.cn

[Q57] 行号
来源：http://lz.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wz.huixiangedu.cn

[Q58] 累计求和
来源：http://hs.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://de.muxihuayi.cn

[Q59] 分组内累计
来源：http://zy.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yb.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://oc.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nz.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pf.hahajie.cn

[Q61] 移动平均
来源：http://tv.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lr.asd995.cn

[Q62] 分组占比
来源：http://tu.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dr.huanxung.cn

[Q63] 开启事务
来源：http://tc.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gx.nszjky.cn

[Q64] 提交事务
来源：http://vb.shxzukj.cn

COMMIT;
来源：http://ve.bjjhwx.cn

[Q65] 回滚事务
来源：http://ad.hahajie.cn

ROLLBACK;
来源：http://za.panjiajie.cn

[Q66] 行锁查询
来源：http://ge.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wp.nszjky.cn

[Q67] 设置隔离级别
来源：http://rn.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bm.haigaiapp.cn

[Q68] 保存点
来源：http://sg.colortex.cn

SAVEPOINT sp1;
来源：http://wc.521024.cn

ROLLBACK TO sp1;
来源：http://bm.szxytkj.cn

[Q69] 查看执行计划
来源：http://gf.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wo.shxzukj.cn

[Q70] 更新统计信息
来源：http://re.hnjuh.cn

ANALYZE TABLE users;
来源：http://tr.gzmigu.cn

[Q71] 查看建表语句
来源：http://el.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ym.haigaiapp.cn

[Q72] 查看索引
来源：http://jm.521024.cn

SHOW INDEX FROM users;
来源：http://sz.chemitech.net.cn

[Q73] 查看表状态
来源：http://hf.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hc.shxzskj.cn

[Q74] 强制使用索引
来源：http://pb.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wj.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://ks.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rz.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ij.huixinmuqiang.cn

[Q76] 按天统计
来源：http://py.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tt.gzmigu.cn

[Q77] 时间加减
来源：http://le.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hg.chemitech.net.cn

[Q78] 当前时间
来源：http://oe.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sn.shtwfgs.cn

[Q79] 字符串拼接
来源：http://uu.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mf.nicolike.cn

[Q80] 字符串截取
来源：http://qz.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sk.szsharing.cn

[Q81] 字符串替换
来源：http://cf.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pv.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://wj.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xf.asd995.cn

[Q83] 大小写转换
来源：http://xu.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zg.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://qi.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://mu.yuntaijiaju.cn

[Q85] 数值取整
来源：http://gv.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pw.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://ua.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://en.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ei.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sb.nicolike.cn


<!-- 参考信息 -->