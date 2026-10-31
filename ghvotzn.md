代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://kb.huixinmuqiang.cn

Go:   go f()
来源：http://my.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://at.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://yi.9csxet.cn

[O02] 使用线程池
来源：http://xc.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cp.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gs.nszjky.cn

JS:   // worker_threads 线程池
来源：http://jn.huanxung.cn

TS:   // worker_threads 线程池
来源：http://lg.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://je.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bp.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dl.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nb.huanxung.cn

[O03] 加锁保护共享数据
来源：http://sn.nszjky.cn

Py:   with lock: shared += 1
来源：http://la.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://rf.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dg.asd995.cn

TS:   // 同 JS
来源：http://ww.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://tt.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rr.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tp.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ay.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://da.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ch.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ge.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://dj.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ma.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xi.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gi.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jb.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://wq.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://sq.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://iq.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ef.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://hm.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://dy.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dx.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ht.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://qq.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fl.szsharing.cn

[O06] 使用进程池
来源：http://en.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pt.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lf.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://aa.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://mc.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ya.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sd.nicolike.cn

Ruby: // fork 块
来源：http://pk.colortex.cn

C#:   Parallel.For
来源：http://dd.huixinmuqiang.cn

================================================================================
来源：http://di.szsharing.cn

P. 常用工具函数
来源：http://mu.nszjky.cn

================================================================================
来源：http://rq.hnjuh.cn

[P01] 生成 UUID
来源：http://gl.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://st.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rw.newstarts.cn

JS:   crypto.randomUUID()
来源：http://tj.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://cu.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://ku.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://rl.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://rh.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://vj.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://nq.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mn.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wg.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ma.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mu.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hy.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rp.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yq.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ll.shxzukj.cn

[P03] 生成短随机字符串
来源：http://tf.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ss.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qm.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mt.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tz.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pe.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xr.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zk.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yl.shtwfgs.cn

[P04] 求长度
来源：http://vi.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hx.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kz.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ea.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rs.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://sk.9csxet.cn

Go:   len(arr);  len(m)
来源：http://hs.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://el.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tm.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://va.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fs.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bz.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fa.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jp.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ef.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lp.nszjky.cn

Ruby: a == b
来源：http://qj.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ex.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kq.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://is.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://ay.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zq.9csxet.cn

TS:   if (x == null) {}
来源：http://az.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ar.bookmarksfly.cn

Go:   if x == nil {}
来源：http://ox.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xu.newstarts.cn

C#:   if (x is null) {}
来源：http://xj.yuexingan06.cn

[P07] 防抖与节流
来源：http://gi.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ur.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://pt.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ic.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ee.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://km.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bw.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ik.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ja.521024.cn

[P08] 处理浮点精度问题
来源：http://gd.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gp.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ry.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ku.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uq.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://na.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cq.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://es.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hm.newstarts.cn

================================================================================
来源：http://fh.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iz.hnjuh.cn

================================================================================
来源：http://pc.huanxung.cn

[Q01] 创建表
来源：http://vq.nicolike.cn

CREATE TABLE users (
来源：http://bz.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://xh.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://bs.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ng.yuexingan06.cn

);
来源：http://bo.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://nf.bjjhwx.cn

CREATE TABLE orders (
来源：http://re.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hl.huixiangedu.cn

user_id INT NOT NULL,
来源：http://nh.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://on.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bk.521024.cn

);
来源：http://xz.yuexingan06.cn

[Q03] 增加列
来源：http://pf.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ov.szxytkj.cn

[Q04] 修改列类型
来源：http://wg.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sr.yuexingan06.cn

[Q05] 重命名列
来源：http://nf.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uf.jctech888.com.cn

[Q06] 删除列
来源：http://pq.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yh.szsharing.cn

[Q07] 删除表
来源：http://jx.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://wa.nicolike.cn

[Q08] 创建普通索引
来源：http://zp.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uj.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ot.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yu.bjjhwx.cn

[Q10] 插入单行
来源：http://ed.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ra.yuexingan06.cn

[Q11] 一次插入多行
来源：http://is.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://da.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://un.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://so.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wz.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://uu.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://to.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://gb.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vt.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fx.shtwfgs.cn

[Q15] 查询全部
来源：http://km.shxzskj.cn

SELECT * FROM users;
来源：http://ch.shxzukj.cn

[Q16] 查询指定列
来源：http://wf.gzmigu.cn

SELECT id, name FROM users;
来源：http://jb.gzmigu.cn

[Q17] 条件查询
来源：http://la.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fb.hahajie.cn

[Q18] 模糊匹配
来源：http://zl.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vy.chemitech.net.cn

[Q19] 范围查询
来源：http://up.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://if.huixiangedu.cn

[Q20] IN 列表
来源：http://mm.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wy.szsharing.cn

[Q21] 空值判断
来源：http://hu.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ye.huixinmuqiang.cn

[Q22] 排序
来源：http://pa.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ly.bookmarksfly.cn

[Q23] 分页
来源：http://yc.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mn.muxihuayi.cn

[Q24] 去重
来源：http://lb.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://we.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://yy.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yw.huanxung.cn

[Q26] 计数
来源：http://au.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://mv.nicolike.cn

[Q27] 条件计数
来源：http://fc.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ek.szsharing.cn

[Q28] 求和与平均
来源：http://yd.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ai.bjjhwx.cn

[Q29] 最大最小值
来源：http://jz.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xs.hnjuh.cn

[Q30] 分组统计
来源：http://wl.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://co.lnxyls.cn

[Q31] 分组后过滤
来源：http://vo.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xo.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://wh.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eu.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zd.yuntaijiaju.cn

[Q33] 多列分组
来源：http://wl.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kx.shxzukj.cn

[Q34] 每组取第一条
来源：http://is.huixinmuqiang.cn

SELECT * FROM (
来源：http://dy.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ax.hahajie.cn

) t WHERE rn = 1;
来源：http://ct.lnxyls.cn

[Q35] 内连接
来源：http://le.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ed.bjjhwx.cn

[Q36] 左连接
来源：http://tc.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://an.bjjhwx.cn

[Q37] 右连接
来源：http://yg.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zs.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lf.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ts.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://er.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xj.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://li.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vs.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tv.nszjky.cn

[Q41] 多表连接
来源：http://nw.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tf.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://ts.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://eh.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://pi.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://oh.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ga.newstarts.cn

[Q43] 标量子查询
来源：http://qr.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kv.nicolike.cn

[Q44] IN 子查询
来源：http://ap.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rp.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://jq.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uf.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xv.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://pn.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ky.asd995.cn

[Q48] CTE 公用表表达式
来源：http://ob.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hd.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://ko.panjiajie.cn

[Q49] 更新单行
来源：http://fu.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jp.huixinmuqiang.cn

[Q50] 批量更新
来源：http://tg.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://br.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://ri.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dq.jctech888.com.cn

[Q52] 删除指定行
来源：http://mp.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://qd.bjjhwx.cn

[Q53] 按条件删除
来源：http://nr.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ao.asd995.cn

[Q54] 清空表
来源：http://md.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://ig.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://gi.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mi.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://dn.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vv.9csxet.cn

[Q57] 行号
来源：http://gj.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bg.shxzskj.cn

[Q58] 累计求和
来源：http://el.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ay.lnxyls.cn

[Q59] 分组内累计
来源：http://il.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bp.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://jv.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hn.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yb.jctech888.com.cn

[Q61] 移动平均
来源：http://dr.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bt.lnxyls.cn

[Q62] 分组占比
来源：http://em.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kx.shxzskj.cn

[Q63] 开启事务
来源：http://ko.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xn.521024.cn

[Q64] 提交事务
来源：http://oj.nicolike.cn

COMMIT;
来源：http://xx.9csxet.cn

[Q65] 回滚事务
来源：http://ej.lnxyls.cn

ROLLBACK;
来源：http://ur.jctech888.com.cn

[Q66] 行锁查询
来源：http://xe.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rg.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://su.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gp.521024.cn

[Q68] 保存点
来源：http://nm.huixiangedu.cn

SAVEPOINT sp1;
来源：http://sv.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://lp.gzmigu.cn

[Q69] 查看执行计划
来源：http://kw.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hp.huixiangedu.cn

[Q70] 更新统计信息
来源：http://gm.chemitech.net.cn

ANALYZE TABLE users;
来源：http://xd.huanxung.cn

[Q71] 查看建表语句
来源：http://wb.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eo.panjiajie.cn

[Q72] 查看索引
来源：http://xx.asd995.cn

SHOW INDEX FROM users;
来源：http://vc.newstarts.cn

[Q73] 查看表状态
来源：http://jz.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wm.szxytkj.cn

[Q74] 强制使用索引
来源：http://gb.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.bookmarksfly.cn

[Q75] 日期格式化
来源：http://yv.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hn.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tc.hnjuh.cn


<!-- 参考信息 -->