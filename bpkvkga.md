代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://ch.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://aw.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ce.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mb.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pw.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://my.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yt.szsharing.cn

Go:   slices.Sort(arr)
来源：http://cz.yuexingan06.cn

Ruby: arr.sort
来源：http://hq.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ap.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://po.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ud.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://nn.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fu.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ta.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://io.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nv.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nv.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xv.asd995.cn

[N04] 斐波那契数列
来源：http://ej.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yn.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mv.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gy.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ix.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qn.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kq.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yy.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wp.muxihuayi.cn

[N05] 最大公约数
来源：http://dy.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://jb.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nh.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vt.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hi.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://xz.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bs.huixiangedu.cn

[N06] 判断回文字符串
来源：http://lc.szsharing.cn

Py:   s == s[::-1]
来源：http://al.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://zh.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://pj.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://hn.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ir.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://ba.wgjwhj.cn

Ruby: s == s.reverse
来源：http://ri.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iz.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://jn.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://id.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vv.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bi.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://mm.bjjhwx.cn

Java: // 手写 HashMap
来源：http://my.hahajie.cn

Go:   // 手写 map[int]int
来源：http://jv.hahajie.cn

Ruby: // 手写 Hash
来源：http://ga.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ea.lnxyls.cn

[N08] 生成全排列
来源：http://nt.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://yi.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://ka.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://al.asd995.cn

TS:   // 手写回溯递归
来源：http://fm.lnxyls.cn

Java: // 手写回溯递归
来源：http://th.szxytkj.cn

Go:   // 手写回溯递归
来源：http://ni.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://cv.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://rf.hahajie.cn

[N09] 栈与队列
来源：http://rp.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://db.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qb.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://of.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zz.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dz.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sl.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rq.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nh.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://nu.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bk.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dn.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dt.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sf.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://dy.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ke.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qo.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rc.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://wp.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ul.9csxet.cn

PHP:  // 手写递归函数
来源：http://jc.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lz.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sz.jctech888.com.cn

Java: // 手写递归
来源：http://az.bjjhwx.cn

Go:   // 手写递归
来源：http://or.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vp.szxytkj.cn

C#:   // 手写递归
来源：http://gv.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xf.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tx.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rl.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ri.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kk.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wi.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://js.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ot.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pn.hnjuh.cn

================================================================================
来源：http://hm.szxytkj.cn

O. 并发与异步
来源：http://py.szsharing.cn

================================================================================
来源：http://dr.szsharing.cn

[O01] 启动一个线程
来源：http://ab.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tr.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bs.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://il.wgjwhj.cn

TS:   // 同 JS
来源：http://jz.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://tt.nicolike.cn

Go:   go f()
来源：http://wl.lnxyls.cn

Ruby: Thread.new { f }
来源：http://qn.521024.cn

C#:   Task.Run(() => F());
来源：http://bs.muxihuayi.cn

[O02] 使用线程池
来源：http://va.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dv.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qy.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ic.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://xz.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lc.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://va.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lp.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fq.9csxet.cn

[O03] 加锁保护共享数据
来源：http://ja.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://oi.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://yt.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qv.wgjwhj.cn

TS:   // 同 JS
来源：http://rl.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://tx.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ii.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://te.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ge.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://jm.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://bx.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lz.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://ka.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pw.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mt.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rg.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xu.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://oz.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://fa.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://no.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vd.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://al.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://gs.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lt.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ij.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://xv.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://id.colortex.cn

[O06] 使用进程池
来源：http://vh.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sk.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bs.colortex.cn

JS:   // child_process / cluster 模块
来源：http://fj.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://hx.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://za.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cd.lnxyls.cn

Ruby: // fork 块
来源：http://kq.jianghongdianzi.cn

C#:   Parallel.For
来源：http://vz.colortex.cn

================================================================================
来源：http://yb.panjiajie.cn

P. 常用工具函数
来源：http://ly.nszjky.cn

================================================================================
来源：http://wp.huanxung.cn

[P01] 生成 UUID
来源：http://vh.521024.cn

Py:   str(uuid.uuid4())
来源：http://wa.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yh.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://hw.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://dh.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://or.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://kq.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://iy.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://ze.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://ni.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jz.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fo.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zu.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rf.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fw.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tb.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mi.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vq.asd995.cn

[P03] 生成短随机字符串
来源：http://um.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dv.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fe.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jl.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ns.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dy.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lj.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zf.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lp.nszjky.cn

[P04] 求长度
来源：http://sy.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://un.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lb.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fj.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ao.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ay.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://uq.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://vh.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ye.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://uj.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cl.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dh.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://at.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iw.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ed.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xf.hnjuh.cn

Ruby: a == b
来源：http://vq.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kw.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rr.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jl.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://df.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://us.yuexingan06.cn

TS:   if (x == null) {}
来源：http://az.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zv.shxzskj.cn

Go:   if x == nil {}
来源：http://sl.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xx.jctech888.com.cn

C#:   if (x is null) {}
来源：http://te.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://mx.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gm.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://na.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cu.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://el.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://un.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://la.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bb.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nx.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://hj.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pv.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ko.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sg.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jj.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jx.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ob.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ox.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ma.chemitech.net.cn

================================================================================
来源：http://qq.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ij.colortex.cn

================================================================================
来源：http://fb.nszjky.cn

[Q01] 创建表
来源：http://ga.szxytkj.cn

CREATE TABLE users (
来源：http://kz.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rx.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://jk.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://fy.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fo.huanxung.cn

);
来源：http://vy.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://vh.bookmarksfly.cn

CREATE TABLE orders (
来源：http://wm.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bx.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://uw.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://cg.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kh.yuexingan06.cn

);
来源：http://en.colortex.cn

[Q03] 增加列
来源：http://qw.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pj.asd995.cn

[Q04] 修改列类型
来源：http://wx.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ki.szsharing.cn

[Q05] 重命名列
来源：http://hv.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qc.9csxet.cn

[Q06] 删除列
来源：http://bs.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ak.lnxyls.cn

[Q07] 删除表
来源：http://qn.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://jp.shxzskj.cn

[Q08] 创建普通索引
来源：http://hp.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ch.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://qj.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xg.muxihuayi.cn

[Q10] 插入单行
来源：http://ox.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eh.bjjhwx.cn

[Q11] 一次插入多行
来源：http://av.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xl.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://sn.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dx.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qm.nicolike.cn

[Q13] 忽略重复插入
来源：http://mh.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ic.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://ez.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yc.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vy.huixinmuqiang.cn

[Q15] 查询全部
来源：http://im.shtwfgs.cn

SELECT * FROM users;
来源：http://bw.huanxung.cn

[Q16] 查询指定列
来源：http://qv.asd995.cn

SELECT id, name FROM users;
来源：http://cm.jctech888.com.cn

[Q17] 条件查询
来源：http://hf.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lq.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://ae.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ag.521024.cn

[Q19] 范围查询
来源：http://wl.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cs.wgjwhj.cn

[Q20] IN 列表
来源：http://pk.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zh.panjiajie.cn

[Q21] 空值判断
来源：http://vq.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zb.hahajie.cn

[Q22] 排序
来源：http://zl.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sc.chemitech.net.cn

[Q23] 分页
来源：http://hi.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mn.yuexingan06.cn

[Q24] 去重
来源：http://ij.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://zc.shxzukj.cn

[Q25] 只取前 N 条
来源：http://qn.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dc.szsharing.cn

[Q26] 计数
来源：http://as.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://kl.shxzukj.cn

[Q27] 条件计数
来源：http://tb.hnjuh.cn


<!-- 参考信息 -->