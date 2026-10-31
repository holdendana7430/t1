代发 wailian999

Ruby: arr.sort
来源：http://qf.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ng.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://ca.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vo.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://tl.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bt.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ke.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ud.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ml.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kk.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uu.bjjhwx.cn

[N04] 斐波那契数列
来源：http://ud.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yc.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ri.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eg.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qh.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zr.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xe.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vd.haigaiapp.cn

[N05] 最大公约数
来源：http://tp.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://lm.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fc.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oy.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nj.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://no.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://av.gzmigu.cn

Ruby: a.gcd(b)
来源：http://fz.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://da.shxzskj.cn

[N06] 判断回文字符串
来源：http://ul.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ca.nicolike.cn

PHP:  $s === strrev($s);
来源：http://hr.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ci.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://yh.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rw.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://vk.newstarts.cn

Ruby: s == s.reverse
来源：http://mk.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ij.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ah.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zz.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ux.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lj.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://vm.bjjhwx.cn

Java: // 手写 HashMap
来源：http://pu.521024.cn

Go:   // 手写 map[int]int
来源：http://me.521024.cn

Ruby: // 手写 Hash
来源：http://sq.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sd.lnxyls.cn

[N08] 生成全排列
来源：http://tz.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://nr.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://mh.szsharing.cn

JS:   // 手写回溯递归
来源：http://ot.nszjky.cn

TS:   // 手写回溯递归
来源：http://fh.hnjuh.cn

Java: // 手写回溯递归
来源：http://xm.colortex.cn

Go:   // 手写回溯递归
来源：http://zx.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://uo.shxzskj.cn

C#:   // 手写回溯递归
来源：http://nu.gzmigu.cn

[N09] 栈与队列
来源：http://bz.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wa.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://to.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wg.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tz.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gz.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ci.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bi.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jv.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://fr.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wv.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xu.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bd.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ae.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://bb.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://un.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qi.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xd.szsharing.cn

[N11] 二叉树中序遍历
来源：http://no.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bh.shxzukj.cn

PHP:  // 手写递归函数
来源：http://pd.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xl.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nd.jianghongdianzi.cn

Java: // 手写递归
来源：http://nk.newstarts.cn

Go:   // 手写递归
来源：http://cb.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fl.huixiangedu.cn

C#:   // 手写递归
来源：http://pd.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jz.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jn.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fh.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xq.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pl.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iv.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sb.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ua.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ui.nicolike.cn

================================================================================
来源：http://pe.shxzukj.cn

O. 并发与异步
来源：http://bd.nicolike.cn

================================================================================
来源：http://ji.shtwfgs.cn

[O01] 启动一个线程
来源：http://nm.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oa.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wu.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vr.haigaiapp.cn

TS:   // 同 JS
来源：http://jb.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://be.nicolike.cn

Go:   go f()
来源：http://ow.shxzukj.cn

Ruby: Thread.new { f }
来源：http://ww.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://lp.szxytkj.cn

[O02] 使用线程池
来源：http://tz.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uo.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gg.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ys.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://iy.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cg.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nh.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sr.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nt.huanxung.cn

[O03] 加锁保护共享数据
来源：http://au.newstarts.cn

Py:   with lock: shared += 1
来源：http://ye.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://xs.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ol.panjiajie.cn

TS:   // 同 JS
来源：http://ai.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://jj.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aj.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mp.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://pg.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://gq.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://fk.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gm.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://fc.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ie.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jk.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ua.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bq.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://hc.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://bo.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://zd.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wv.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://bi.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://hr.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bh.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cq.szsharing.cn

Ruby: threads.map(&:join)
来源：http://kp.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xs.huixiangedu.cn

[O06] 使用进程池
来源：http://bs.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kp.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://te.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://yr.521024.cn

TS:   // child_process / cluster 模块
来源：http://fn.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wf.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kx.chemitech.net.cn

Ruby: // fork 块
来源：http://su.shxzukj.cn

C#:   Parallel.For
来源：http://bn.asd995.cn

================================================================================
来源：http://pn.yuexingan06.cn

P. 常用工具函数
来源：http://cs.gzmigu.cn

================================================================================
来源：http://nz.hnjuh.cn

[P01] 生成 UUID
来源：http://sq.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://sx.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zs.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://ae.nicolike.cn

TS:   crypto.randomUUID()
来源：http://sy.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://aq.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://jc.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://yn.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://yw.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://zp.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ns.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zb.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mk.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wp.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uz.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://al.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zw.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mw.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://qz.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zw.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vd.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vx.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cf.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fy.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ei.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zf.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qm.yuexingan06.cn

[P04] 求长度
来源：http://xk.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rp.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://va.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oo.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xf.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://je.szsharing.cn

Go:   len(arr);  len(m)
来源：http://cb.asd995.cn

Ruby: x.length;  x.size
来源：http://qr.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mz.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://iq.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cl.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tp.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yp.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jb.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://by.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gv.panjiajie.cn

Ruby: a == b
来源：http://da.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ib.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jl.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rj.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://db.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iw.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://mp.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ms.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://vf.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://by.wgjwhj.cn

C#:   if (x is null) {}
来源：http://lb.bjjhwx.cn

[P07] 防抖与节流
来源：http://sd.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sd.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://yp.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hd.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ra.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://js.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pj.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ua.newstarts.cn

[P08] 处理浮点精度问题
来源：http://hl.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tb.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hq.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jq.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jt.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vp.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ap.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://km.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mm.hnjuh.cn

================================================================================
来源：http://sh.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xb.colortex.cn

================================================================================
来源：http://yc.huanxung.cn

[Q01] 创建表
来源：http://yn.newstarts.cn

CREATE TABLE users (
来源：http://gb.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ev.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ag.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ly.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nq.wgjwhj.cn

);
来源：http://sh.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://co.9csxet.cn

CREATE TABLE orders (
来源：http://ao.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ra.shxzukj.cn

user_id INT NOT NULL,
来源：http://uv.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://gm.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sl.shxzukj.cn

);
来源：http://nj.shtwfgs.cn

[Q03] 增加列
来源：http://sz.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uc.huixiangedu.cn

[Q04] 修改列类型
来源：http://it.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gq.huixiangedu.cn

[Q05] 重命名列
来源：http://pu.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ex.huanxung.cn

[Q06] 删除列
来源：http://hs.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dt.panjiajie.cn

[Q07] 删除表
来源：http://zi.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://iv.szxytkj.cn

[Q08] 创建普通索引
来源：http://qt.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lt.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://ke.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ui.bookmarksfly.cn

[Q10] 插入单行
来源：http://hz.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://do.panjiajie.cn

[Q11] 一次插入多行
来源：http://wo.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ya.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://vn.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ep.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eb.nicolike.cn

[Q13] 忽略重复插入
来源：http://qs.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cn.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://mq.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xu.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://us.nicolike.cn

[Q15] 查询全部
来源：http://kq.haigaiapp.cn

SELECT * FROM users;
来源：http://fb.yuexingan06.cn

[Q16] 查询指定列
来源：http://qb.shxzskj.cn

SELECT id, name FROM users;
来源：http://ht.shxzskj.cn

[Q17] 条件查询
来源：http://nn.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hi.chemitech.net.cn

[Q18] 模糊匹配
来源：http://wy.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ag.huanxung.cn

[Q19] 范围查询
来源：http://db.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wn.wgjwhj.cn

[Q20] IN 列表
来源：http://pu.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gj.wgjwhj.cn

[Q21] 空值判断
来源：http://ke.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dj.lnxyls.cn

[Q22] 排序
来源：http://fq.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://td.shtwfgs.cn

[Q23] 分页
来源：http://zx.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lc.yuntaijiaju.cn

[Q24] 去重
来源：http://lo.521024.cn

SELECT DISTINCT city FROM users;
来源：http://gg.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://ji.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ri.gzmigu.cn

[Q26] 计数
来源：http://ni.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://qs.shxzskj.cn

[Q27] 条件计数
来源：http://en.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rh.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://jn.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ir.haigaiapp.cn

[Q29] 最大最小值
来源：http://lc.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jf.bookmarksfly.cn

[Q30] 分组统计
来源：http://vm.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qa.newstarts.cn

[Q31] 分组后过滤
来源：http://hx.yuntaijiaju.cn


<!-- 参考信息 -->