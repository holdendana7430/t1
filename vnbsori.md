代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tf.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://im.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ad.asd995.cn

TS:   // 同 JS
来源：http://qp.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://bt.bjjhwx.cn

Go:   go f()
来源：http://us.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://zz.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://az.bookmarksfly.cn

[O02] 使用线程池
来源：http://zp.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ch.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ms.colortex.cn

JS:   // worker_threads 线程池
来源：http://xq.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://zy.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wo.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rq.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gx.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pe.szsharing.cn

[O03] 加锁保护共享数据
来源：http://tf.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://sc.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://na.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vz.shxzukj.cn

TS:   // 同 JS
来源：http://ff.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://zb.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://js.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yc.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://xw.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://xf.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://jz.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jb.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://qh.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ng.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ln.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bu.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ap.asd995.cn

C#:   async Task F() { await G(); }
来源：http://vl.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://gs.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://mi.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ly.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://hi.521024.cn

TS:   await Promise.all(tasks)
来源：http://gf.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://va.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://if.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://wx.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pa.chemitech.net.cn

[O06] 使用进程池
来源：http://br.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fv.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gt.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://hh.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://gi.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fm.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uc.yuntaijiaju.cn

Ruby: // fork 块
来源：http://ug.hnjuh.cn

C#:   Parallel.For
来源：http://vh.chemitech.net.cn

================================================================================
来源：http://th.panjiajie.cn

P. 常用工具函数
来源：http://vz.jctech888.com.cn

================================================================================
来源：http://ad.chemitech.net.cn

[P01] 生成 UUID
来源：http://bb.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://en.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vu.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://fe.9csxet.cn

TS:   crypto.randomUUID()
来源：http://jd.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://yd.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://ax.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://xk.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xi.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://bh.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bx.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hg.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bg.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sc.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zx.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lg.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gc.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ys.hahajie.cn

[P03] 生成短随机字符串
来源：http://og.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ao.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nr.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uj.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tk.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mo.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vt.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xp.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mn.haigaiapp.cn

[P04] 求长度
来源：http://ms.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zk.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sn.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xz.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://at.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://qw.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://gw.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pw.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://ss.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pt.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uv.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uz.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://id.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vr.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://px.huanxung.cn

Ruby: a == b
来源：http://wd.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ww.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mk.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://mn.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fo.panjiajie.cn

TS:   if (x == null) {}
来源：http://wc.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://do.haigaiapp.cn

Go:   if x == nil {}
来源：http://bx.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fc.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://bx.nicolike.cn

[P07] 防抖与节流
来源：http://pk.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ii.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ck.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nf.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tb.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pc.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ki.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wm.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mt.9csxet.cn

[P08] 处理浮点精度问题
来源：http://ib.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gq.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gs.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fh.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nb.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vj.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qn.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lr.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ui.bjjhwx.cn

================================================================================
来源：http://dz.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ql.nszjky.cn

================================================================================
来源：http://ie.gzmigu.cn

[Q01] 创建表
来源：http://jz.jctech888.com.cn

CREATE TABLE users (
来源：http://ny.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uc.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://ew.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://lu.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aw.jctech888.com.cn

);
来源：http://gc.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://og.yuexingan06.cn

CREATE TABLE orders (
来源：http://px.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ay.hnjuh.cn

user_id INT NOT NULL,
来源：http://oh.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://xm.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sj.bjjhwx.cn

);
来源：http://le.shxzukj.cn

[Q03] 增加列
来源：http://ln.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ss.shxzukj.cn

[Q04] 修改列类型
来源：http://oj.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ko.yuntaijiaju.cn

[Q05] 重命名列
来源：http://jk.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vo.szxytkj.cn

[Q06] 删除列
来源：http://ks.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hp.shxzukj.cn

[Q07] 删除表
来源：http://es.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://ml.jctech888.com.cn

[Q08] 创建普通索引
来源：http://rq.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sf.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://hh.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fi.huixinmuqiang.cn

[Q10] 插入单行
来源：http://or.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zf.huixiangedu.cn

[Q11] 一次插入多行
来源：http://bo.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xd.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://hw.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hc.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yf.521024.cn

[Q13] 忽略重复插入
来源：http://sk.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qk.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://tx.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ud.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mb.nicolike.cn

[Q15] 查询全部
来源：http://gb.panjiajie.cn

SELECT * FROM users;
来源：http://bo.asd995.cn

[Q16] 查询指定列
来源：http://gj.panjiajie.cn

SELECT id, name FROM users;
来源：http://el.szxytkj.cn

[Q17] 条件查询
来源：http://gq.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cz.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://bu.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xj.hahajie.cn

[Q19] 范围查询
来源：http://ww.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kc.hahajie.cn

[Q20] IN 列表
来源：http://dc.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://st.muxihuayi.cn

[Q21] 空值判断
来源：http://xm.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aq.shtwfgs.cn

[Q22] 排序
来源：http://hm.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cc.bjjhwx.cn

[Q23] 分页
来源：http://av.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qa.jianghongdianzi.cn

[Q24] 去重
来源：http://qa.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://nu.panjiajie.cn

[Q25] 只取前 N 条
来源：http://kj.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eu.bjjhwx.cn

[Q26] 计数
来源：http://ky.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://er.shxzskj.cn

[Q27] 条件计数
来源：http://qu.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qv.asd995.cn

[Q28] 求和与平均
来源：http://lm.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ob.521024.cn

[Q29] 最大最小值
来源：http://bi.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yc.nszjky.cn

[Q30] 分组统计
来源：http://ne.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yh.bjjhwx.cn

[Q31] 分组后过滤
来源：http://lr.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nc.newstarts.cn

[Q32] 分组拼接字符串
来源：http://me.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lh.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cz.wgjwhj.cn

[Q33] 多列分组
来源：http://up.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yj.haigaiapp.cn

[Q34] 每组取第一条
来源：http://qe.szxytkj.cn

SELECT * FROM (
来源：http://iz.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jd.szsharing.cn

) t WHERE rn = 1;
来源：http://mj.yuexingan06.cn

[Q35] 内连接
来源：http://bx.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ts.colortex.cn

[Q36] 左连接
来源：http://tm.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://el.chemitech.net.cn

[Q37] 右连接
来源：http://ii.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tm.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ys.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ym.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://dk.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://im.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://so.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wg.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lm.shxzukj.cn

[Q41] 多表连接
来源：http://bd.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ux.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://ds.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://hp.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://wn.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://rc.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sy.panjiajie.cn

[Q43] 标量子查询
来源：http://fa.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oe.yuexingan06.cn

[Q44] IN 子查询
来源：http://cb.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lz.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://ad.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://we.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ax.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mf.shxzskj.cn

[Q47] 与平均值比较
来源：http://au.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vc.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://lo.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://db.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://pp.panjiajie.cn

[Q49] 更新单行
来源：http://hl.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mc.wgjwhj.cn

[Q50] 批量更新
来源：http://qk.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cb.nszjky.cn

[Q51] 用子查询更新
来源：http://li.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rl.asd995.cn

[Q52] 删除指定行
来源：http://bg.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://fq.jctech888.com.cn

[Q53] 按条件删除
来源：http://ax.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wm.hahajie.cn

[Q54] 清空表
来源：http://wk.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://lu.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://vg.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://go.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://dq.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rb.9csxet.cn

[Q57] 行号
来源：http://hm.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jm.szxytkj.cn

[Q58] 累计求和
来源：http://do.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jl.szxytkj.cn

[Q59] 分组内累计
来源：http://sn.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ij.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://gi.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://re.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://un.hahajie.cn

[Q61] 移动平均
来源：http://ud.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pt.hnjuh.cn

[Q62] 分组占比
来源：http://lo.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ri.asd995.cn

[Q63] 开启事务
来源：http://dt.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xn.yuexingan06.cn

[Q64] 提交事务
来源：http://xu.jianghongdianzi.cn

COMMIT;
来源：http://hu.haigaiapp.cn

[Q65] 回滚事务
来源：http://bi.521024.cn

ROLLBACK;
来源：http://mg.hnjuh.cn

[Q66] 行锁查询
来源：http://ya.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fx.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://az.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fb.muxihuayi.cn

[Q68] 保存点
来源：http://rn.szsharing.cn

SAVEPOINT sp1;
来源：http://ly.shxzukj.cn

ROLLBACK TO sp1;
来源：http://ij.9csxet.cn

[Q69] 查看执行计划
来源：http://ix.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bb.asd995.cn

[Q70] 更新统计信息
来源：http://ps.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://ga.gzmigu.cn

[Q71] 查看建表语句
来源：http://qo.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ys.yuntaijiaju.cn

[Q72] 查看索引
来源：http://fr.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://mh.yuexingan06.cn

[Q73] 查看表状态
来源：http://qz.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ri.nicolike.cn

[Q74] 强制使用索引
来源：http://ij.yuntaijiaju.cn


<!-- 参考信息 -->