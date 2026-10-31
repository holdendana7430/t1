代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vm.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://if.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mv.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lg.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ax.shxzskj.cn

[N10] 链表节点定义
来源：http://bi.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lh.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ef.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bs.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kc.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://jn.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ft.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qx.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ne.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://vr.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pq.hahajie.cn

PHP:  // 手写递归函数
来源：http://ze.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pu.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qe.szsharing.cn

Java: // 手写递归
来源：http://ma.huanxung.cn

Go:   // 手写递归
来源：http://km.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xi.szsharing.cn

C#:   // 手写递归
来源：http://jh.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gg.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pl.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aq.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oe.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zt.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ac.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://so.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iv.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uj.nszjky.cn

================================================================================
来源：http://ah.shxzskj.cn

O. 并发与异步
来源：http://cm.muxihuayi.cn

================================================================================
来源：http://zd.9csxet.cn

[O01] 启动一个线程
来源：http://ja.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bd.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jc.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yj.haigaiapp.cn

TS:   // 同 JS
来源：http://vo.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://th.9csxet.cn

Go:   go f()
来源：http://sw.shxzukj.cn

Ruby: Thread.new { f }
来源：http://zr.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://du.huixiangedu.cn

[O02] 使用线程池
来源：http://gs.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dk.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wd.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://vu.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://ef.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fz.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ff.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ha.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ti.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ur.nszjky.cn

Py:   with lock: shared += 1
来源：http://gb.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://wr.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kb.shxzskj.cn

TS:   // 同 JS
来源：http://uj.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ih.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jn.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://em.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://oo.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://zs.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://ed.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bc.asd995.cn

JS:   async function f() { await g(); }
来源：http://zu.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dd.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oy.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ej.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wd.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://cq.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://ko.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ox.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bc.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ie.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://bu.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cr.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gk.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://ed.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kg.lnxyls.cn

[O06] 使用进程池
来源：http://oe.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fh.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eb.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://pw.asd995.cn

TS:   // child_process / cluster 模块
来源：http://za.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zr.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ei.hahajie.cn

Ruby: // fork 块
来源：http://py.muxihuayi.cn

C#:   Parallel.For
来源：http://gz.shxzukj.cn

================================================================================
来源：http://pt.panjiajie.cn

P. 常用工具函数
来源：http://yr.huixiangedu.cn

================================================================================
来源：http://px.huixiangedu.cn

[P01] 生成 UUID
来源：http://bk.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://ii.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yv.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://vr.asd995.cn

TS:   crypto.randomUUID()
来源：http://am.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://dl.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://ol.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://ey.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://bm.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://oe.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lh.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://or.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wm.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ii.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bx.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vz.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iu.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ie.panjiajie.cn

[P03] 生成短随机字符串
来源：http://bw.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iy.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://su.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rp.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://py.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oc.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eh.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wc.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tx.jianghongdianzi.cn

[P04] 求长度
来源：http://tv.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ox.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oj.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gc.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nw.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://jm.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://pd.hahajie.cn

Ruby: x.length;  x.size
来源：http://wi.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ex.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://mq.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tc.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xf.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ov.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ui.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vv.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://re.gzmigu.cn

Ruby: a == b
来源：http://xp.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rq.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ec.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zg.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://hp.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ye.gzmigu.cn

TS:   if (x == null) {}
来源：http://lr.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://re.panjiajie.cn

Go:   if x == nil {}
来源：http://ig.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ek.wgjwhj.cn

C#:   if (x is null) {}
来源：http://cc.muxihuayi.cn

[P07] 防抖与节流
来源：http://ay.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jb.asd995.cn

PHP:  // 手写时间戳比较
来源：http://ck.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ov.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ia.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dj.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://td.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ix.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yl.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://ao.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qu.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zt.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yf.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iv.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aw.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jg.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lp.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nz.jianghongdianzi.cn

================================================================================
来源：http://si.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kk.asd995.cn

================================================================================
来源：http://um.huixiangedu.cn

[Q01] 创建表
来源：http://xx.huixinmuqiang.cn

CREATE TABLE users (
来源：http://if.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hw.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://tg.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://wa.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nd.panjiajie.cn

);
来源：http://ap.hahajie.cn

[Q02] 创建带外键的表
来源：http://au.shxzukj.cn

CREATE TABLE orders (
来源：http://jj.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://et.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://jc.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://gi.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lw.newstarts.cn

);
来源：http://hj.jianghongdianzi.cn

[Q03] 增加列
来源：http://at.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mh.shtwfgs.cn

[Q04] 修改列类型
来源：http://uc.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zz.haigaiapp.cn

[Q05] 重命名列
来源：http://wm.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ld.shxzskj.cn

[Q06] 删除列
来源：http://by.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qn.521024.cn

[Q07] 删除表
来源：http://lo.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://tk.521024.cn

[Q08] 创建普通索引
来源：http://vb.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://of.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://bz.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ot.shtwfgs.cn

[Q10] 插入单行
来源：http://th.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bi.jctech888.com.cn

[Q11] 一次插入多行
来源：http://ws.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yl.asd995.cn

[Q12] 插入后取自增 ID
来源：http://cv.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lp.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xn.hnjuh.cn

[Q13] 忽略重复插入
来源：http://cg.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gj.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://cu.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hw.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nq.huixinmuqiang.cn

[Q15] 查询全部
来源：http://wy.lnxyls.cn

SELECT * FROM users;
来源：http://qi.muxihuayi.cn

[Q16] 查询指定列
来源：http://lx.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://kx.panjiajie.cn

[Q17] 条件查询
来源：http://ho.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bm.nicolike.cn

[Q18] 模糊匹配
来源：http://yf.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zl.panjiajie.cn

[Q19] 范围查询
来源：http://xf.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kl.panjiajie.cn

[Q20] IN 列表
来源：http://xq.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vg.9csxet.cn

[Q21] 空值判断
来源：http://th.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ft.gzmigu.cn

[Q22] 排序
来源：http://qt.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rb.jianghongdianzi.cn

[Q23] 分页
来源：http://cd.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fv.lnxyls.cn

[Q24] 去重
来源：http://fj.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://gn.gzmigu.cn

[Q25] 只取前 N 条
来源：http://oi.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xm.gzmigu.cn

[Q26] 计数
来源：http://id.521024.cn

SELECT COUNT(*) FROM users;
来源：http://rg.huanxung.cn

[Q27] 条件计数
来源：http://fq.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://br.nszjky.cn

[Q28] 求和与平均
来源：http://vf.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nh.chemitech.net.cn

[Q29] 最大最小值
来源：http://xo.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://th.shxzukj.cn

[Q30] 分组统计
来源：http://zs.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ph.bjjhwx.cn

[Q31] 分组后过滤
来源：http://lh.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://my.szsharing.cn

[Q32] 分组拼接字符串
来源：http://nk.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://me.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eo.jianghongdianzi.cn

[Q33] 多列分组
来源：http://uo.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yw.asd995.cn

[Q34] 每组取第一条
来源：http://ej.wgjwhj.cn

SELECT * FROM (
来源：http://xv.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ps.szxytkj.cn

) t WHERE rn = 1;
来源：http://xy.huixinmuqiang.cn

[Q35] 内连接
来源：http://xw.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pf.nicolike.cn

[Q36] 左连接
来源：http://na.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ld.shtwfgs.cn

[Q37] 右连接
来源：http://ey.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fv.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lh.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qp.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://yi.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vw.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ik.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fy.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ls.wgjwhj.cn

[Q41] 多表连接
来源：http://rp.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pn.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://xy.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://cn.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://wo.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://bn.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vp.haigaiapp.cn

[Q43] 标量子查询
来源：http://er.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hc.hnjuh.cn

[Q44] IN 子查询
来源：http://ey.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hq.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://bm.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vi.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ea.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tr.colortex.cn

[Q47] 与平均值比较
来源：http://um.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iw.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://uz.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vk.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://yw.chemitech.net.cn

[Q49] 更新单行
来源：http://tz.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qc.asd995.cn

[Q50] 批量更新
来源：http://wo.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nb.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://zj.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fp.shtwfgs.cn

[Q52] 删除指定行
来源：http://zj.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://ut.shxzskj.cn

[Q53] 按条件删除
来源：http://dq.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pd.jctech888.com.cn

[Q54] 清空表
来源：http://us.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://kb.521024.cn

[Q55] 排名（并列占位）
来源：http://no.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ug.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://rk.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ij.colortex.cn

[Q57] 行号
来源：http://vg.hahajie.cn


<!-- 参考信息 -->