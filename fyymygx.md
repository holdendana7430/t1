代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://ba.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fk.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bs.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zc.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rq.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gg.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://en.bjjhwx.cn

[N04] 斐波那契数列
来源：http://my.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jy.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tf.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ij.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://il.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wh.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lq.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://um.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tx.shxzukj.cn

[N05] 最大公约数
来源：http://ci.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://uy.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vk.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ng.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ex.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ke.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://au.9csxet.cn

Ruby: a.gcd(b)
来源：http://vt.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pp.asd995.cn

[N06] 判断回文字符串
来源：http://pw.bjjhwx.cn

Py:   s == s[::-1]
来源：http://mp.hahajie.cn

PHP:  $s === strrev($s);
来源：http://rf.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ed.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://zm.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fh.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://nd.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://it.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gk.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://yw.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hb.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://js.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bs.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://gj.nszjky.cn

Java: // 手写 HashMap
来源：http://yl.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://tl.nszjky.cn

Ruby: // 手写 Hash
来源：http://bl.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qx.gzmigu.cn

[N08] 生成全排列
来源：http://gk.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://pw.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://en.newstarts.cn

JS:   // 手写回溯递归
来源：http://ld.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://iu.gzmigu.cn

Java: // 手写回溯递归
来源：http://an.nicolike.cn

Go:   // 手写回溯递归
来源：http://bg.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://ef.gzmigu.cn

C#:   // 手写回溯递归
来源：http://kt.bookmarksfly.cn

[N09] 栈与队列
来源：http://ze.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bb.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mf.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ir.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ww.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cu.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lf.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ui.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sy.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://rl.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yx.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xb.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xe.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lo.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://rn.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ro.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ud.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xl.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://cx.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://or.asd995.cn

PHP:  // 手写递归函数
来源：http://cc.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vu.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xl.bookmarksfly.cn

Java: // 手写递归
来源：http://pl.521024.cn

Go:   // 手写递归
来源：http://im.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tv.yuntaijiaju.cn

C#:   // 手写递归
来源：http://fv.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sj.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ex.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ue.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lr.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bl.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nu.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ii.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gg.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fk.colortex.cn

================================================================================
来源：http://xx.newstarts.cn

O. 并发与异步
来源：http://jr.szxytkj.cn

================================================================================
来源：http://mo.yuexingan06.cn

[O01] 启动一个线程
来源：http://lt.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zc.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rv.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ra.lnxyls.cn

TS:   // 同 JS
来源：http://qi.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://yo.huixinmuqiang.cn

Go:   go f()
来源：http://ch.shxzskj.cn

Ruby: Thread.new { f }
来源：http://dc.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://rg.haigaiapp.cn

[O02] 使用线程池
来源：http://wa.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yh.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ug.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://bs.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://eq.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mc.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pi.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lq.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lz.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://ee.hahajie.cn

Py:   with lock: shared += 1
来源：http://bq.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://um.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hl.wgjwhj.cn

TS:   // 同 JS
来源：http://nr.521024.cn

Java: synchronized (this) { shared++; }
来源：http://ix.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rl.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gj.521024.cn

C#:   lock (gate) { shared++; }
来源：http://fd.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://gy.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://cm.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tj.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ox.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fy.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uk.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gi.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cu.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://hj.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://zn.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ir.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ru.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://zp.asd995.cn

TS:   await Promise.all(tasks)
来源：http://ca.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bq.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fx.nszjky.cn

Ruby: threads.map(&:join)
来源：http://qa.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yr.9csxet.cn

[O06] 使用进程池
来源：http://xl.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ke.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dk.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://ji.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://sx.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uc.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ae.hahajie.cn

Ruby: // fork 块
来源：http://sc.shxzskj.cn

C#:   Parallel.For
来源：http://pm.nicolike.cn

================================================================================
来源：http://lt.huixiangedu.cn

P. 常用工具函数
来源：http://gj.muxihuayi.cn

================================================================================
来源：http://fk.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://pa.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://rk.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ai.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://de.521024.cn

TS:   crypto.randomUUID()
来源：http://qc.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ar.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://az.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://zr.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://ln.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://hw.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kr.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uv.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ma.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ep.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dn.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ot.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ot.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ra.panjiajie.cn

[P03] 生成短随机字符串
来源：http://ri.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hv.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gz.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gk.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xv.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tg.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yd.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://av.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ej.yuntaijiaju.cn

[P04] 求长度
来源：http://bm.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ne.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://os.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sd.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://re.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://hi.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://xz.huanxung.cn

Ruby: x.length;  x.size
来源：http://ik.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ts.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://nz.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xc.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lc.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rv.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ik.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hb.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lx.bookmarksfly.cn

Ruby: a == b
来源：http://jh.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dn.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zm.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xz.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://eb.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wg.chemitech.net.cn

TS:   if (x == null) {}
来源：http://qz.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ow.newstarts.cn

Go:   if x == nil {}
来源：http://sk.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nl.521024.cn

C#:   if (x is null) {}
来源：http://sj.chemitech.net.cn

[P07] 防抖与节流
来源：http://hx.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cg.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://dh.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://do.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dl.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ke.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mf.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nn.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dz.newstarts.cn

[P08] 处理浮点精度问题
来源：http://il.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tx.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cq.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dz.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mc.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dy.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kj.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hc.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ii.yuexingan06.cn

================================================================================
来源：http://sx.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eo.lnxyls.cn

================================================================================
来源：http://gb.nszjky.cn

[Q01] 创建表
来源：http://mr.muxihuayi.cn

CREATE TABLE users (
来源：http://my.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zg.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://lc.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://qq.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wx.asd995.cn

);
来源：http://bl.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://lp.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ll.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ut.shtwfgs.cn

user_id INT NOT NULL,
来源：http://uv.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://vk.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://df.yuexingan06.cn

);
来源：http://oi.bookmarksfly.cn

[Q03] 增加列
来源：http://tt.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iv.asd995.cn

[Q04] 修改列类型
来源：http://xr.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qk.hnjuh.cn

[Q05] 重命名列
来源：http://py.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tq.chemitech.net.cn

[Q06] 删除列
来源：http://nt.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://je.jctech888.com.cn

[Q07] 删除表
来源：http://jt.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://sj.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://vg.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dz.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://bp.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gq.jctech888.com.cn

[Q10] 插入单行
来源：http://oo.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gp.jctech888.com.cn

[Q11] 一次插入多行
来源：http://dv.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gc.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://hb.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qx.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hw.szxytkj.cn

[Q13] 忽略重复插入
来源：http://zy.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wz.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://ev.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zv.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cx.nszjky.cn

[Q15] 查询全部
来源：http://vp.huixiangedu.cn

SELECT * FROM users;
来源：http://js.yuexingan06.cn

[Q16] 查询指定列
来源：http://ps.asd995.cn

SELECT id, name FROM users;
来源：http://ur.9csxet.cn

[Q17] 条件查询
来源：http://dh.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jn.shtwfgs.cn

[Q18] 模糊匹配
来源：http://vi.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jb.9csxet.cn

[Q19] 范围查询
来源：http://th.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sb.colortex.cn

[Q20] IN 列表
来源：http://fm.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rw.muxihuayi.cn

[Q21] 空值判断
来源：http://dj.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ln.nicolike.cn

[Q22] 排序
来源：http://jj.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ki.nszjky.cn

[Q23] 分页
来源：http://ww.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mq.newstarts.cn

[Q24] 去重
来源：http://dk.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://vv.colortex.cn

[Q25] 只取前 N 条
来源：http://mc.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jd.panjiajie.cn

[Q26] 计数
来源：http://sh.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://ju.bjjhwx.cn

[Q27] 条件计数
来源：http://il.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ll.hnjuh.cn

[Q28] 求和与平均
来源：http://ry.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qj.panjiajie.cn

[Q29] 最大最小值
来源：http://mg.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dp.wgjwhj.cn

[Q30] 分组统计
来源：http://kq.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oy.panjiajie.cn

[Q31] 分组后过滤
来源：http://jo.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vu.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://oz.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gk.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pq.huanxung.cn


<!-- 参考信息 -->