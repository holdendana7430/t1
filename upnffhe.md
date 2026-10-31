代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ho.521024.cn

[O03] 加锁保护共享数据
来源：http://sv.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://uf.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://pw.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sm.bookmarksfly.cn

TS:   // 同 JS
来源：http://hj.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://dj.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zi.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://la.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://np.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://rs.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://sm.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nu.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://zz.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ce.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ww.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qj.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sr.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://wp.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://wk.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wp.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://br.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://we.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sw.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qj.521024.cn

Ruby: threads.map(&:join)
来源：http://oc.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nw.yuntaijiaju.cn

[O06] 使用进程池
来源：http://ed.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ms.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://at.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://qs.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://vw.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://il.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vs.jctech888.com.cn

Ruby: // fork 块
来源：http://sl.jctech888.com.cn

C#:   Parallel.For
来源：http://ur.wgjwhj.cn

================================================================================
来源：http://fd.shxzukj.cn

P. 常用工具函数
来源：http://aq.asd995.cn

================================================================================
来源：http://cn.haigaiapp.cn

[P01] 生成 UUID
来源：http://tj.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://sn.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://np.9csxet.cn

JS:   crypto.randomUUID()
来源：http://tj.hahajie.cn

TS:   crypto.randomUUID()
来源：http://ju.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://zr.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://bo.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://uw.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ar.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://pg.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oa.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aa.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dg.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ue.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mw.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://on.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rm.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ci.huanxung.cn

[P03] 生成短随机字符串
来源：http://nw.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zi.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zt.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ak.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qx.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pw.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tl.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sp.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ro.huanxung.cn

[P04] 求长度
来源：http://fi.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sh.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gg.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yi.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ff.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://ob.hahajie.cn

Go:   len(arr);  len(m)
来源：http://et.huanxung.cn

Ruby: x.length;  x.size
来源：http://nj.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wt.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://lt.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vy.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mv.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iw.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pm.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ip.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sf.hahajie.cn

Ruby: a == b
来源：http://rp.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fd.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vp.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pm.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://dz.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hj.asd995.cn

TS:   if (x == null) {}
来源：http://mx.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vk.szxytkj.cn

Go:   if x == nil {}
来源：http://vn.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ss.jctech888.com.cn

C#:   if (x is null) {}
来源：http://zl.haigaiapp.cn

[P07] 防抖与节流
来源：http://uh.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uk.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://yr.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wx.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fr.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kf.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ra.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wx.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://uy.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://il.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://op.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xg.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tp.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tr.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wj.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uv.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kk.panjiajie.cn

================================================================================
来源：http://hh.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://or.asd995.cn

================================================================================
来源：http://cw.bjjhwx.cn

[Q01] 创建表
来源：http://gj.lnxyls.cn

CREATE TABLE users (
来源：http://cf.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ot.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://vw.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://wk.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qz.9csxet.cn

);
来源：http://ow.szsharing.cn

[Q02] 创建带外键的表
来源：http://at.jctech888.com.cn

CREATE TABLE orders (
来源：http://zs.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ux.panjiajie.cn

user_id INT NOT NULL,
来源：http://qk.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://lb.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fx.9csxet.cn

);
来源：http://yv.muxihuayi.cn

[Q03] 增加列
来源：http://jl.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://np.shtwfgs.cn

[Q04] 修改列类型
来源：http://sl.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ue.bookmarksfly.cn

[Q05] 重命名列
来源：http://qq.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kh.bjjhwx.cn

[Q06] 删除列
来源：http://hp.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ob.yuntaijiaju.cn

[Q07] 删除表
来源：http://dx.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://bu.nszjky.cn

[Q08] 创建普通索引
来源：http://lm.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eq.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://or.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bj.shtwfgs.cn

[Q10] 插入单行
来源：http://tc.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tf.hahajie.cn

[Q11] 一次插入多行
来源：http://vt.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dy.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://su.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sp.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ut.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://yb.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dm.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://co.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ln.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hs.nicolike.cn

[Q15] 查询全部
来源：http://ig.nszjky.cn

SELECT * FROM users;
来源：http://is.yuexingan06.cn

[Q16] 查询指定列
来源：http://fo.shxzskj.cn

SELECT id, name FROM users;
来源：http://kk.hahajie.cn

[Q17] 条件查询
来源：http://nd.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://we.hahajie.cn

[Q18] 模糊匹配
来源：http://oo.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wf.hahajie.cn

[Q19] 范围查询
来源：http://yy.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sp.lnxyls.cn

[Q20] IN 列表
来源：http://tg.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ft.521024.cn

[Q21] 空值判断
来源：http://vy.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fy.shtwfgs.cn

[Q22] 排序
来源：http://ra.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wu.nszjky.cn

[Q23] 分页
来源：http://ro.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hd.muxihuayi.cn

[Q24] 去重
来源：http://ll.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://xj.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://pd.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zb.colortex.cn

[Q26] 计数
来源：http://ur.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://vz.colortex.cn

[Q27] 条件计数
来源：http://hi.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://th.colortex.cn

[Q28] 求和与平均
来源：http://vi.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ut.jctech888.com.cn

[Q29] 最大最小值
来源：http://uv.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sq.colortex.cn

[Q30] 分组统计
来源：http://by.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ju.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://rr.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qz.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://br.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sj.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://im.huanxung.cn

[Q33] 多列分组
来源：http://qk.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oa.hnjuh.cn

[Q34] 每组取第一条
来源：http://gj.newstarts.cn

SELECT * FROM (
来源：http://tb.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jk.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://bu.asd995.cn

[Q35] 内连接
来源：http://ry.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hu.9csxet.cn

[Q36] 左连接
来源：http://bf.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://le.huixinmuqiang.cn

[Q37] 右连接
来源：http://fp.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gj.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zz.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cy.colortex.cn

[Q39] 自连接（查上下级）
来源：http://dp.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bs.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://un.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://el.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uc.muxihuayi.cn

[Q41] 多表连接
来源：http://kj.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gc.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://lj.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://dl.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://yc.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://sv.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ip.szsharing.cn

[Q43] 标量子查询
来源：http://bc.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://je.wgjwhj.cn

[Q44] IN 子查询
来源：http://zg.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xo.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://eu.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rs.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ut.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dq.shxzukj.cn

[Q47] 与平均值比较
来源：http://fm.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ee.colortex.cn

[Q48] CTE 公用表表达式
来源：http://yb.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zc.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://gs.szsharing.cn

[Q49] 更新单行
来源：http://ob.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oy.panjiajie.cn

[Q50] 批量更新
来源：http://xr.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tr.chemitech.net.cn

[Q51] 用子查询更新
来源：http://bj.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ud.shtwfgs.cn

[Q52] 删除指定行
来源：http://dq.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://vt.huixiangedu.cn

[Q53] 按条件删除
来源：http://km.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ju.521024.cn

[Q54] 清空表
来源：http://lj.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://js.newstarts.cn

[Q55] 排名（并列占位）
来源：http://eq.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aj.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://iz.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ox.jctech888.com.cn

[Q57] 行号
来源：http://dv.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rq.521024.cn

[Q58] 累计求和
来源：http://cn.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tz.9csxet.cn

[Q59] 分组内累计
来源：http://um.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mj.521024.cn

[Q60] 取上一行 / 下一行
来源：http://xn.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kq.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wi.huanxung.cn

[Q61] 移动平均
来源：http://wz.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://re.hnjuh.cn

[Q62] 分组占比
来源：http://cn.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yl.nszjky.cn

[Q63] 开启事务
来源：http://be.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ro.wgjwhj.cn

[Q64] 提交事务
来源：http://zz.hnjuh.cn

COMMIT;
来源：http://qu.haigaiapp.cn

[Q65] 回滚事务
来源：http://zg.jianghongdianzi.cn

ROLLBACK;
来源：http://qx.shxzukj.cn

[Q66] 行锁查询
来源：http://lx.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wx.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://ku.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jo.hahajie.cn

[Q68] 保存点
来源：http://cn.shxzukj.cn

SAVEPOINT sp1;
来源：http://ag.nszjky.cn

ROLLBACK TO sp1;
来源：http://to.yuexingan06.cn

[Q69] 查看执行计划
来源：http://io.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://da.wgjwhj.cn

[Q70] 更新统计信息
来源：http://em.521024.cn

ANALYZE TABLE users;
来源：http://sz.nicolike.cn

[Q71] 查看建表语句
来源：http://af.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ls.chemitech.net.cn

[Q72] 查看索引
来源：http://fm.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://yb.9csxet.cn

[Q73] 查看表状态
来源：http://ew.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ur.wgjwhj.cn

[Q74] 强制使用索引
来源：http://zc.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xc.shxzukj.cn

[Q75] 日期格式化
来源：http://op.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bz.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yj.huanxung.cn

[Q76] 按天统计
来源：http://sa.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nt.panjiajie.cn

[Q77] 时间加减
来源：http://kv.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jt.jctech888.com.cn

[Q78] 当前时间
来源：http://vz.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gl.lnxyls.cn

[Q79] 字符串拼接
来源：http://ed.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mj.shxzukj.cn

[Q80] 字符串截取
来源：http://ad.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bp.panjiajie.cn

[Q81] 字符串替换
来源：http://nf.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bm.hahajie.cn


<!-- 参考信息 -->