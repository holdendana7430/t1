代发 wailian999

Go:   // 手写递归
来源：http://ta.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wa.colortex.cn

C#:   // 手写递归
来源：http://yi.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pr.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tn.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pw.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iy.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cu.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ll.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vw.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jc.521024.cn

================================================================================
来源：http://zx.9csxet.cn

O. 并发与异步
来源：http://bz.gzmigu.cn

================================================================================
来源：http://ap.asd995.cn

[O01] 启动一个线程
来源：http://vy.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pt.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zz.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zt.szxytkj.cn

TS:   // 同 JS
来源：http://ty.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://bu.hahajie.cn

Go:   go f()
来源：http://aq.shxzskj.cn

Ruby: Thread.new { f }
来源：http://iy.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://sc.huixinmuqiang.cn

[O02] 使用线程池
来源：http://tw.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qm.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://om.szsharing.cn

JS:   // worker_threads 线程池
来源：http://oo.huanxung.cn

TS:   // worker_threads 线程池
来源：http://bj.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ho.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://it.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cl.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gx.nicolike.cn

[O03] 加锁保护共享数据
来源：http://hk.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://ru.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://rs.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ef.huixinmuqiang.cn

TS:   // 同 JS
来源：http://eo.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://qa.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sy.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rm.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://jk.huanxung.cn

[O04] 定义异步函数并等待
来源：http://za.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://bw.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mr.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://ax.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gj.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://va.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kb.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qz.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://up.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://fy.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://rq.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vl.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://it.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://fk.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ro.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://on.asd995.cn

Ruby: threads.map(&:join)
来源：http://aq.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ll.shxzukj.cn

[O06] 使用进程池
来源：http://hx.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gr.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rz.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://qz.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://kz.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jt.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hh.haigaiapp.cn

Ruby: // fork 块
来源：http://ul.shxzukj.cn

C#:   Parallel.For
来源：http://ti.nszjky.cn

================================================================================
来源：http://yu.nszjky.cn

P. 常用工具函数
来源：http://ck.hahajie.cn

================================================================================
来源：http://xv.asd995.cn

[P01] 生成 UUID
来源：http://pj.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://nf.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dl.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://wr.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://pd.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://cr.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://mc.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://bg.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://bq.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ib.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ji.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wv.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uq.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://io.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dr.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pd.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bh.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eq.panjiajie.cn

[P03] 生成短随机字符串
来源：http://td.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://su.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cv.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oh.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://be.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gz.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fd.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dp.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ym.huanxung.cn

[P04] 求长度
来源：http://ua.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ro.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sz.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zt.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ag.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://nu.huanxung.cn

Go:   len(arr);  len(m)
来源：http://zi.colortex.cn

Ruby: x.length;  x.size
来源：http://kt.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jr.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://gq.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dm.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eg.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ne.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wb.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uf.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://po.jctech888.com.cn

Ruby: a == b
来源：http://rp.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dm.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eh.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ap.colortex.cn

PHP:  if (empty($x)) {}
来源：http://eu.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://km.shxzukj.cn

TS:   if (x == null) {}
来源：http://ja.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ii.haigaiapp.cn

Go:   if x == nil {}
来源：http://qe.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pg.jctech888.com.cn

C#:   if (x is null) {}
来源：http://ey.hnjuh.cn

[P07] 防抖与节流
来源：http://hn.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ua.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://nm.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://av.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rk.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sp.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tk.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ob.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fx.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://bl.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gc.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ud.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hq.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yq.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://op.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ly.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hl.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vs.yuntaijiaju.cn

================================================================================
来源：http://qv.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://li.szsharing.cn

================================================================================
来源：http://wy.asd995.cn

[Q01] 创建表
来源：http://lf.yuntaijiaju.cn

CREATE TABLE users (
来源：http://ko.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wk.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://iu.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://ku.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wr.shtwfgs.cn

);
来源：http://eu.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://dl.9csxet.cn

CREATE TABLE orders (
来源：http://fo.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://by.bjjhwx.cn

user_id INT NOT NULL,
来源：http://fx.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://ge.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ef.jianghongdianzi.cn

);
来源：http://ng.chemitech.net.cn

[Q03] 增加列
来源：http://ur.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wu.bjjhwx.cn

[Q04] 修改列类型
来源：http://eh.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ke.nicolike.cn

[Q05] 重命名列
来源：http://kq.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pb.yuexingan06.cn

[Q06] 删除列
来源：http://fr.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jy.asd995.cn

[Q07] 删除表
来源：http://hj.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://xl.shxzukj.cn

[Q08] 创建普通索引
来源：http://lf.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vx.nicolike.cn

[Q09] 创建唯一索引
来源：http://sb.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sk.newstarts.cn

[Q10] 插入单行
来源：http://qf.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tf.szsharing.cn

[Q11] 一次插入多行
来源：http://ob.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nf.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://yx.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hf.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wl.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://nm.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cg.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://yw.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yb.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uk.panjiajie.cn

[Q15] 查询全部
来源：http://nk.haigaiapp.cn

SELECT * FROM users;
来源：http://ii.nicolike.cn

[Q16] 查询指定列
来源：http://kn.hahajie.cn

SELECT id, name FROM users;
来源：http://ou.hahajie.cn

[Q17] 条件查询
来源：http://ks.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qd.hahajie.cn

[Q18] 模糊匹配
来源：http://ee.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kj.nicolike.cn

[Q19] 范围查询
来源：http://zl.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kw.hnjuh.cn

[Q20] IN 列表
来源：http://jr.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dd.9csxet.cn

[Q21] 空值判断
来源：http://wh.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lf.huixinmuqiang.cn

[Q22] 排序
来源：http://ji.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sd.szxytkj.cn

[Q23] 分页
来源：http://nm.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ps.panjiajie.cn

[Q24] 去重
来源：http://qz.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://hb.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://os.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mc.yuexingan06.cn

[Q26] 计数
来源：http://sp.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ty.panjiajie.cn

[Q27] 条件计数
来源：http://ih.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jd.bookmarksfly.cn

[Q28] 求和与平均
来源：http://nk.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aw.shxzskj.cn

[Q29] 最大最小值
来源：http://jg.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://be.jctech888.com.cn

[Q30] 分组统计
来源：http://tu.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yt.colortex.cn

[Q31] 分组后过滤
来源：http://by.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hg.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://ou.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xb.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vf.shxzukj.cn

[Q33] 多列分组
来源：http://df.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bm.chemitech.net.cn

[Q34] 每组取第一条
来源：http://kd.lnxyls.cn

SELECT * FROM (
来源：http://ws.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ug.hahajie.cn

) t WHERE rn = 1;
来源：http://df.szsharing.cn

[Q35] 内连接
来源：http://ng.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qh.muxihuayi.cn

[Q36] 左连接
来源：http://cd.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yy.yuexingan06.cn

[Q37] 右连接
来源：http://yn.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ex.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://te.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hf.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://uk.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zy.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ui.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qc.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pk.huixiangedu.cn

[Q41] 多表连接
来源：http://zy.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mq.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ym.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://yt.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://sc.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://ox.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cf.szsharing.cn

[Q43] 标量子查询
来源：http://jo.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vz.asd995.cn

[Q44] IN 子查询
来源：http://rx.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pf.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://ra.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yr.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ew.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zr.9csxet.cn

[Q47] 与平均值比较
来源：http://nl.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bc.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://us.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kp.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://yi.newstarts.cn

[Q49] 更新单行
来源：http://fg.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wl.panjiajie.cn

[Q50] 批量更新
来源：http://jy.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vt.newstarts.cn

[Q51] 用子查询更新
来源：http://yn.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wz.bookmarksfly.cn

[Q52] 删除指定行
来源：http://tu.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://kh.hahajie.cn

[Q53] 按条件删除
来源：http://ic.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rw.panjiajie.cn

[Q54] 清空表
来源：http://dx.colortex.cn

TRUNCATE TABLE logs;
来源：http://if.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://zs.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://id.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://vi.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jt.yuexingan06.cn

[Q57] 行号
来源：http://ax.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tc.wgjwhj.cn

[Q58] 累计求和
来源：http://vy.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jz.asd995.cn

[Q59] 分组内累计
来源：http://am.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ge.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://rz.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iu.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ai.szxytkj.cn

[Q61] 移动平均
来源：http://dn.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mh.hnjuh.cn

[Q62] 分组占比
来源：http://bo.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qc.jctech888.com.cn

[Q63] 开启事务
来源：http://fc.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ps.huixinmuqiang.cn

[Q64] 提交事务
来源：http://ov.9csxet.cn

COMMIT;
来源：http://dh.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://bx.521024.cn

ROLLBACK;
来源：http://ni.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://td.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cu.bjjhwx.cn


<!-- 参考信息 -->