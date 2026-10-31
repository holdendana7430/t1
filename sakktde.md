代发 wailian999

Go:   // 手写 map[int]int
来源：http://mq.hnjuh.cn

Ruby: // 手写 Hash
来源：http://qt.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zo.huixiangedu.cn

[N08] 生成全排列
来源：http://nh.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://fn.gzmigu.cn

PHP:  // 手写递归交换
来源：http://oj.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://fh.521024.cn

TS:   // 手写回溯递归
来源：http://pn.gzmigu.cn

Java: // 手写回溯递归
来源：http://fs.huanxung.cn

Go:   // 手写回溯递归
来源：http://ke.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://do.hnjuh.cn

C#:   // 手写回溯递归
来源：http://jf.bjjhwx.cn

[N09] 栈与队列
来源：http://oe.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mt.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ua.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wm.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xp.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hk.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qc.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://se.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ln.shxzskj.cn

[N10] 链表节点定义
来源：http://en.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lw.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ee.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qt.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iv.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ef.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xx.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gd.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pd.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://lo.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xc.lnxyls.cn

PHP:  // 手写递归函数
来源：http://dp.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mc.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lb.9csxet.cn

Java: // 手写递归
来源：http://di.asd995.cn

Go:   // 手写递归
来源：http://sn.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pj.wgjwhj.cn

C#:   // 手写递归
来源：http://mr.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ab.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vl.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mr.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oy.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uy.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gy.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yw.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iy.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vd.huanxung.cn

================================================================================
来源：http://le.chemitech.net.cn

O. 并发与异步
来源：http://oz.bjjhwx.cn

================================================================================
来源：http://ih.9csxet.cn

[O01] 启动一个线程
来源：http://ek.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fo.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lx.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xj.nicolike.cn

TS:   // 同 JS
来源：http://tc.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://mh.bjjhwx.cn

Go:   go f()
来源：http://lo.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://td.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://hl.szsharing.cn

[O02] 使用线程池
来源：http://vb.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zq.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gp.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://gg.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ll.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pe.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jh.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tr.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ye.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://fo.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://ew.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://qe.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dt.bjjhwx.cn

TS:   // 同 JS
来源：http://jr.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://gp.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://su.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rx.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://bp.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://uq.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ck.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dn.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://rk.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sp.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ow.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ij.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://un.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ia.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://gh.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://iw.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yx.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://ut.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://kg.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vq.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zd.newstarts.cn

Ruby: threads.map(&:join)
来源：http://eb.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qk.asd995.cn

[O06] 使用进程池
来源：http://fj.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ab.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bf.521024.cn

JS:   // child_process / cluster 模块
来源：http://pk.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://au.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uw.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mb.asd995.cn

Ruby: // fork 块
来源：http://wt.huixiangedu.cn

C#:   Parallel.For
来源：http://hb.huixiangedu.cn

================================================================================
来源：http://ks.shxzukj.cn

P. 常用工具函数
来源：http://de.huanxung.cn

================================================================================
来源：http://hm.chemitech.net.cn

[P01] 生成 UUID
来源：http://ua.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://mh.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://my.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://ye.newstarts.cn

TS:   crypto.randomUUID()
来源：http://pu.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://po.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://ud.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://nd.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://qz.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://zo.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ps.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lm.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aw.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://az.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nx.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uo.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://it.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bg.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://dp.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://td.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mu.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lp.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://th.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jm.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gx.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vj.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sg.gzmigu.cn

[P04] 求长度
来源：http://zx.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zs.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://au.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qm.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yd.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://cm.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://vw.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://yx.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oj.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ab.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bj.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hf.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yl.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uy.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ym.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bt.shxzukj.cn

Ruby: a == b
来源：http://wk.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ol.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ly.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rl.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://aa.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tz.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://qu.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tv.nszjky.cn

Go:   if x == nil {}
来源：http://ms.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cq.szsharing.cn

C#:   if (x is null) {}
来源：http://zu.huixiangedu.cn

[P07] 防抖与节流
来源：http://ae.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kn.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://im.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rp.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ao.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dp.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://df.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lw.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ip.nicolike.cn

[P08] 处理浮点精度问题
来源：http://ka.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ii.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pl.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ui.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iq.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xy.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jz.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wk.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zr.huixiangedu.cn

================================================================================
来源：http://ck.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aj.jctech888.com.cn

================================================================================
来源：http://yf.panjiajie.cn

[Q01] 创建表
来源：http://lo.huixinmuqiang.cn

CREATE TABLE users (
来源：http://ee.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dg.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ya.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://mv.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vy.bookmarksfly.cn

);
来源：http://gl.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://uk.szsharing.cn

CREATE TABLE orders (
来源：http://mp.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ss.muxihuayi.cn

user_id INT NOT NULL,
来源：http://te.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://fp.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pv.szxytkj.cn

);
来源：http://nr.hahajie.cn

[Q03] 增加列
来源：http://ci.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gt.wgjwhj.cn

[Q04] 修改列类型
来源：http://er.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pm.huanxung.cn

[Q05] 重命名列
来源：http://hy.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qu.bookmarksfly.cn

[Q06] 删除列
来源：http://dj.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jf.huixiangedu.cn

[Q07] 删除表
来源：http://mc.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://id.huanxung.cn

[Q08] 创建普通索引
来源：http://hq.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dn.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://fb.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pd.wgjwhj.cn

[Q10] 插入单行
来源：http://ld.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zu.szxytkj.cn

[Q11] 一次插入多行
来源：http://xr.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gr.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://br.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://at.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pp.huanxung.cn

[Q13] 忽略重复插入
来源：http://mt.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://em.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://pz.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bs.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hd.szsharing.cn

[Q15] 查询全部
来源：http://al.hahajie.cn

SELECT * FROM users;
来源：http://op.chemitech.net.cn

[Q16] 查询指定列
来源：http://rh.szsharing.cn

SELECT id, name FROM users;
来源：http://vr.haigaiapp.cn

[Q17] 条件查询
来源：http://hg.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oj.colortex.cn

[Q18] 模糊匹配
来源：http://en.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yr.huixinmuqiang.cn

[Q19] 范围查询
来源：http://fh.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://an.asd995.cn

[Q20] IN 列表
来源：http://gq.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://af.newstarts.cn

[Q21] 空值判断
来源：http://wo.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oq.hahajie.cn

[Q22] 排序
来源：http://tp.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xr.szsharing.cn

[Q23] 分页
来源：http://ng.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gm.gzmigu.cn

[Q24] 去重
来源：http://zw.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://ny.shxzukj.cn

[Q25] 只取前 N 条
来源：http://it.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bp.yuexingan06.cn

[Q26] 计数
来源：http://af.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://wp.shxzukj.cn

[Q27] 条件计数
来源：http://yv.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ju.shtwfgs.cn

[Q28] 求和与平均
来源：http://vd.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mb.shxzskj.cn

[Q29] 最大最小值
来源：http://vh.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dz.huixiangedu.cn

[Q30] 分组统计
来源：http://em.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lx.muxihuayi.cn

[Q31] 分组后过滤
来源：http://fj.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mh.nicolike.cn

[Q32] 分组拼接字符串
来源：http://re.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gt.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ow.huixinmuqiang.cn

[Q33] 多列分组
来源：http://sb.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gi.yuexingan06.cn

[Q34] 每组取第一条
来源：http://bl.szxytkj.cn

SELECT * FROM (
来源：http://mr.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ol.huixiangedu.cn

) t WHERE rn = 1;
来源：http://my.asd995.cn

[Q35] 内连接
来源：http://ik.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ov.gzmigu.cn

[Q36] 左连接
来源：http://vz.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cr.9csxet.cn

[Q37] 右连接
来源：http://pu.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gt.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bq.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ie.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://lj.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ou.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sp.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vk.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zg.newstarts.cn

[Q41] 多表连接
来源：http://aq.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://la.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://wv.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://cg.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://sh.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://ba.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wh.newstarts.cn

[Q43] 标量子查询
来源：http://mj.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zn.shxzskj.cn

[Q44] IN 子查询
来源：http://us.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tq.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://dx.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hh.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xx.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bg.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ue.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wc.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://ko.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cv.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://kn.huixinmuqiang.cn

[Q49] 更新单行
来源：http://yq.yuexingan06.cn


<!-- 参考信息 -->