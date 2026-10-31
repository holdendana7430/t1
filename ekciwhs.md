代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bs.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ma.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://dl.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ub.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eu.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://rf.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://mg.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zg.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://by.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qx.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vh.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://my.szxytkj.cn

Ruby: arr.sort
来源：http://ot.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zy.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://xn.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jj.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ri.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fp.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sb.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yb.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kc.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jo.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qy.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://nu.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sd.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://es.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xd.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bu.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wl.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yx.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cm.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mo.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ss.asd995.cn

Py:   math.gcd(a, b)
来源：http://ey.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rk.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://az.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://un.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tr.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zp.shxzukj.cn

Ruby: a.gcd(b)
来源：http://jl.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://to.hnjuh.cn

[N06] 判断回文字符串
来源：http://al.shxzskj.cn

Py:   s == s[::-1]
来源：http://yu.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://lg.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://vo.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://cd.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ix.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://fn.hahajie.cn

Ruby: s == s.reverse
来源：http://at.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fi.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ur.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gi.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jm.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vt.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://dt.shxzskj.cn

Java: // 手写 HashMap
来源：http://rf.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ul.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://tj.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://en.nszjky.cn

[N08] 生成全排列
来源：http://id.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://yo.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://yf.lnxyls.cn

JS:   // 手写回溯递归
来源：http://vl.szxytkj.cn

TS:   // 手写回溯递归
来源：http://zf.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://tw.asd995.cn

Go:   // 手写回溯递归
来源：http://fo.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://hc.hnjuh.cn

C#:   // 手写回溯递归
来源：http://pu.chemitech.net.cn

[N09] 栈与队列
来源：http://ig.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sl.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hk.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ib.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vx.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nf.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://er.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bl.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jw.shxzskj.cn

[N10] 链表节点定义
来源：http://bp.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bv.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xp.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xf.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aq.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://lw.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lm.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mm.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ik.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://os.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sn.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://yu.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://io.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pj.jctech888.com.cn

Java: // 手写递归
来源：http://jn.nszjky.cn

Go:   // 手写递归
来源：http://tr.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ic.asd995.cn

C#:   // 手写递归
来源：http://wz.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ib.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hh.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ct.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://js.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sv.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sj.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wo.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ay.panjiajie.cn

================================================================================
来源：http://ef.hnjuh.cn

O. 并发与异步
来源：http://oj.huixinmuqiang.cn

================================================================================
来源：http://rl.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://gt.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vy.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pl.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nl.bjjhwx.cn

TS:   // 同 JS
来源：http://at.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://mu.yuexingan06.cn

Go:   go f()
来源：http://fb.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://yx.nszjky.cn

C#:   Task.Run(() => F());
来源：http://xi.huixiangedu.cn

[O02] 使用线程池
来源：http://ha.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ir.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cs.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://ou.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://ah.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uv.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qe.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bb.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uz.colortex.cn

[O03] 加锁保护共享数据
来源：http://rw.colortex.cn

Py:   with lock: shared += 1
来源：http://uh.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://wf.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ew.yuexingan06.cn

TS:   // 同 JS
来源：http://zu.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://zu.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gv.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yh.521024.cn

C#:   lock (gate) { shared++; }
来源：http://ws.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://yd.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://fb.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yq.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://sf.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fx.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aw.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wj.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jm.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://rf.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://ma.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://nd.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zi.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://xn.asd995.cn

TS:   await Promise.all(tasks)
来源：http://ln.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hx.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pb.nszjky.cn

Ruby: threads.map(&:join)
来源：http://jw.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zw.jianghongdianzi.cn

[O06] 使用进程池
来源：http://oq.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hh.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gi.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://xm.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://xy.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qa.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gi.chemitech.net.cn

Ruby: // fork 块
来源：http://xm.asd995.cn

C#:   Parallel.For
来源：http://ze.yuexingan06.cn

================================================================================
来源：http://xz.colortex.cn

P. 常用工具函数
来源：http://sg.panjiajie.cn

================================================================================
来源：http://kn.yuexingan06.cn

[P01] 生成 UUID
来源：http://dj.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://qv.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ks.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://iu.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://bt.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://jd.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://pv.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://mw.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://bb.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://la.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tw.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jn.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jb.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cn.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bw.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kt.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hx.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://si.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://kz.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://za.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ie.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mj.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dp.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nr.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vc.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wi.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qw.asd995.cn

[P04] 求长度
来源：http://uz.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ef.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://me.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uy.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ms.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://nl.nszjky.cn

Go:   len(arr);  len(m)
来源：http://hc.szxytkj.cn

Ruby: x.length;  x.size
来源：http://nv.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zj.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://la.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pr.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://za.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://th.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lk.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ia.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tp.yuexingan06.cn

Ruby: a == b
来源：http://jn.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lu.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bp.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aq.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://bj.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://al.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://ab.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yc.huixiangedu.cn

Go:   if x == nil {}
来源：http://ad.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ud.gzmigu.cn

C#:   if (x is null) {}
来源：http://di.9csxet.cn

[P07] 防抖与节流
来源：http://lh.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ge.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://pp.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bd.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ue.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dg.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zk.nszjky.cn

[P08] 处理浮点精度问题
来源：http://zp.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lz.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://va.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xp.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://np.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ah.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://me.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ww.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rk.gzmigu.cn

================================================================================
来源：http://vo.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dt.panjiajie.cn

================================================================================
来源：http://gf.yuntaijiaju.cn

[Q01] 创建表
来源：http://kc.shtwfgs.cn

CREATE TABLE users (
来源：http://wf.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vc.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://xk.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://ke.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gm.bookmarksfly.cn

);
来源：http://ly.shxzukj.cn

[Q02] 创建带外键的表
来源：http://qd.newstarts.cn

CREATE TABLE orders (
来源：http://fl.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qw.nicolike.cn

user_id INT NOT NULL,
来源：http://rl.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://bj.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lt.chemitech.net.cn

);
来源：http://ev.jianghongdianzi.cn

[Q03] 增加列
来源：http://xc.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://px.asd995.cn

[Q04] 修改列类型
来源：http://ij.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://et.shtwfgs.cn

[Q05] 重命名列
来源：http://vh.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bz.hnjuh.cn

[Q06] 删除列
来源：http://ba.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pu.wgjwhj.cn

[Q07] 删除表
来源：http://ct.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://zc.hahajie.cn

[Q08] 创建普通索引
来源：http://cw.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tp.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://xq.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ah.yuexingan06.cn

[Q10] 插入单行
来源：http://ir.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dx.haigaiapp.cn

[Q11] 一次插入多行
来源：http://wb.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pb.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://be.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mk.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ha.panjiajie.cn

[Q13] 忽略重复插入
来源：http://de.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uj.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ar.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ot.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wu.asd995.cn

[Q15] 查询全部
来源：http://um.nicolike.cn

SELECT * FROM users;
来源：http://wp.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ks.shxzukj.cn

SELECT id, name FROM users;
来源：http://ps.asd995.cn

[Q17] 条件查询
来源：http://ag.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://og.nicolike.cn

[Q18] 模糊匹配
来源：http://cw.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dv.huixinmuqiang.cn

[Q19] 范围查询
来源：http://jw.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://is.szxytkj.cn

[Q20] IN 列表
来源：http://lf.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vm.nszjky.cn

[Q21] 空值判断
来源：http://fy.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xl.huixiangedu.cn

[Q22] 排序
来源：http://pz.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rx.szsharing.cn

[Q23] 分页
来源：http://sv.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://my.chemitech.net.cn

[Q24] 去重
来源：http://pp.521024.cn

SELECT DISTINCT city FROM users;
来源：http://tq.szxytkj.cn

[Q25] 只取前 N 条
来源：http://fl.yuexingan06.cn


<!-- 参考信息 -->