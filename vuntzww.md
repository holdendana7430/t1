代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zn.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://na.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qw.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gj.yuexingan06.cn

[N05] 最大公约数
来源：http://yh.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://zc.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vp.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kr.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yd.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fr.521024.cn

Ruby: a.gcd(b)
来源：http://gg.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fk.szsharing.cn

[N06] 判断回文字符串
来源：http://er.nicolike.cn

Py:   s == s[::-1]
来源：http://or.szsharing.cn

PHP:  $s === strrev($s);
来源：http://yg.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://lc.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://gy.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uy.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://zf.muxihuayi.cn

Ruby: s == s.reverse
来源：http://rz.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ac.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://za.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://si.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://td.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://np.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://va.jctech888.com.cn

Java: // 手写 HashMap
来源：http://db.9csxet.cn

Go:   // 手写 map[int]int
来源：http://vj.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://wv.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zg.lnxyls.cn

[N08] 生成全排列
来源：http://nl.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://vt.panjiajie.cn

PHP:  // 手写递归交换
来源：http://ic.9csxet.cn

JS:   // 手写回溯递归
来源：http://gc.panjiajie.cn

TS:   // 手写回溯递归
来源：http://qi.newstarts.cn

Java: // 手写回溯递归
来源：http://ee.szxytkj.cn

Go:   // 手写回溯递归
来源：http://zf.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://dy.shxzukj.cn

C#:   // 手写回溯递归
来源：http://tf.lnxyls.cn

[N09] 栈与队列
来源：http://qq.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rx.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pt.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gz.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xr.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ad.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pr.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hu.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ad.lnxyls.cn

[N10] 链表节点定义
来源：http://gj.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nd.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ks.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jy.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bs.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://lr.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hg.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://my.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oc.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ky.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ki.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://wz.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ty.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tn.nicolike.cn

Java: // 手写递归
来源：http://ia.hnjuh.cn

Go:   // 手写递归
来源：http://rf.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yv.huixinmuqiang.cn

C#:   // 手写递归
来源：http://jx.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://to.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bt.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ak.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ig.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iq.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kq.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://un.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vq.bookmarksfly.cn

================================================================================
来源：http://qg.bookmarksfly.cn

O. 并发与异步
来源：http://sq.haigaiapp.cn

================================================================================
来源：http://nt.nszjky.cn

[O01] 启动一个线程
来源：http://zo.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uu.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cc.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pq.jctech888.com.cn

TS:   // 同 JS
来源：http://ag.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://ir.huanxung.cn

Go:   go f()
来源：http://xl.shxzukj.cn

Ruby: Thread.new { f }
来源：http://al.newstarts.cn

C#:   Task.Run(() => F());
来源：http://bv.hahajie.cn

[O02] 使用线程池
来源：http://zi.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hc.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ka.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://tw.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://pm.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ql.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gj.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://id.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cm.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://vf.nszjky.cn

Py:   with lock: shared += 1
来源：http://va.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://wc.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mq.jctech888.com.cn

TS:   // 同 JS
来源：http://ij.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://ax.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cc.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jt.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://gf.nicolike.cn

[O04] 定义异步函数并等待
来源：http://tf.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://rl.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vh.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://me.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lk.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://td.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ob.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ll.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://yg.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://zc.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://ig.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ce.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://ah.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://es.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xw.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ot.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://dr.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kb.huanxung.cn

[O06] 使用进程池
来源：http://lg.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://it.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://do.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://er.521024.cn

TS:   // child_process / cluster 模块
来源：http://la.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gj.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zq.9csxet.cn

Ruby: // fork 块
来源：http://ee.szsharing.cn

C#:   Parallel.For
来源：http://ol.bookmarksfly.cn

================================================================================
来源：http://sn.wgjwhj.cn

P. 常用工具函数
来源：http://iq.huanxung.cn

================================================================================
来源：http://va.lnxyls.cn

[P01] 生成 UUID
来源：http://ih.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://wj.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pi.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://qy.521024.cn

TS:   crypto.randomUUID()
来源：http://dh.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://xo.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://zg.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://qr.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://uh.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://rq.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xb.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zs.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lz.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fw.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xr.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kr.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xa.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ju.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://ik.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kv.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zn.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lk.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bs.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ai.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pz.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ri.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gg.nszjky.cn

[P04] 求长度
来源：http://au.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qp.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pr.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sv.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ax.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://gr.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://pg.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://lo.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rr.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://mr.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kq.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zx.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ru.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ay.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ue.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vy.shxzukj.cn

Ruby: a == b
来源：http://dj.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mz.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iu.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wo.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://nv.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lq.gzmigu.cn

TS:   if (x == null) {}
来源：http://vh.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gw.hahajie.cn

Go:   if x == nil {}
来源：http://tv.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wt.521024.cn

C#:   if (x is null) {}
来源：http://fz.asd995.cn

[P07] 防抖与节流
来源：http://wu.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lt.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://zv.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://me.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gc.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dp.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cs.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hc.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rp.9csxet.cn

[P08] 处理浮点精度问题
来源：http://fy.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pb.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yg.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uk.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qs.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uc.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xx.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tt.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nt.hnjuh.cn

================================================================================
来源：http://ok.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wt.jctech888.com.cn

================================================================================
来源：http://to.yuexingan06.cn

[Q01] 创建表
来源：http://wp.shxzukj.cn

CREATE TABLE users (
来源：http://fs.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://di.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://or.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://da.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://no.huixiangedu.cn

);
来源：http://cn.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://va.asd995.cn

CREATE TABLE orders (
来源：http://nw.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tl.yuexingan06.cn

user_id INT NOT NULL,
来源：http://qu.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://iv.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://md.yuexingan06.cn

);
来源：http://tz.huixiangedu.cn

[Q03] 增加列
来源：http://mn.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tm.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://te.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qr.huixiangedu.cn

[Q05] 重命名列
来源：http://dm.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kt.hnjuh.cn

[Q06] 删除列
来源：http://yd.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://np.newstarts.cn

[Q07] 删除表
来源：http://ay.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://ni.jctech888.com.cn

[Q08] 创建普通索引
来源：http://oz.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ro.asd995.cn

[Q09] 创建唯一索引
来源：http://qb.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xn.yuntaijiaju.cn

[Q10] 插入单行
来源：http://nc.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uh.wgjwhj.cn

[Q11] 一次插入多行
来源：http://cc.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cw.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://oa.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vz.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yc.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://tp.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xb.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://cx.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://it.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hi.wgjwhj.cn

[Q15] 查询全部
来源：http://ex.9csxet.cn

SELECT * FROM users;
来源：http://ic.chemitech.net.cn

[Q16] 查询指定列
来源：http://af.huanxung.cn

SELECT id, name FROM users;
来源：http://le.colortex.cn

[Q17] 条件查询
来源：http://jp.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ou.gzmigu.cn

[Q18] 模糊匹配
来源：http://yf.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sq.jianghongdianzi.cn

[Q19] 范围查询
来源：http://vl.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ts.szsharing.cn

[Q20] IN 列表
来源：http://cw.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zv.panjiajie.cn

[Q21] 空值判断
来源：http://zk.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kx.lnxyls.cn

[Q22] 排序
来源：http://ef.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vj.bjjhwx.cn

[Q23] 分页
来源：http://rc.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qk.szsharing.cn

[Q24] 去重
来源：http://fp.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://te.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://mw.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ao.nicolike.cn

[Q26] 计数
来源：http://fs.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://kk.huixiangedu.cn

[Q27] 条件计数
来源：http://hm.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xd.colortex.cn

[Q28] 求和与平均
来源：http://pl.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ip.jctech888.com.cn

[Q29] 最大最小值
来源：http://ba.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ut.haigaiapp.cn

[Q30] 分组统计
来源：http://ob.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pj.newstarts.cn

[Q31] 分组后过滤
来源：http://ic.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bb.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ed.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ec.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ty.jianghongdianzi.cn

[Q33] 多列分组
来源：http://si.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tr.nszjky.cn

[Q34] 每组取第一条
来源：http://lx.muxihuayi.cn

SELECT * FROM (
来源：http://zd.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zj.521024.cn

) t WHERE rn = 1;
来源：http://km.shxzukj.cn

[Q35] 内连接
来源：http://yy.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ee.colortex.cn

[Q36] 左连接
来源：http://ci.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iu.shxzukj.cn

[Q37] 右连接
来源：http://ah.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hn.nicolike.cn


<!-- 参考信息 -->