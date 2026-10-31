代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sf.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dp.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://dx.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uj.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wt.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://zn.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ct.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hd.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cj.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fp.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xx.colortex.cn

Go:   slices.Sort(arr)
来源：http://ut.hnjuh.cn

Ruby: arr.sort
来源：http://lk.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vl.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://em.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gm.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ay.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jd.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ct.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fh.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uo.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nw.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pk.huanxung.cn

[N04] 斐波那契数列
来源：http://us.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://va.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qf.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uq.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ta.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xo.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ep.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://en.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bs.colortex.cn

[N05] 最大公约数
来源：http://kq.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://kw.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ce.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ml.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ev.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cv.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sb.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://cj.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ti.panjiajie.cn

[N06] 判断回文字符串
来源：http://bm.szsharing.cn

Py:   s == s[::-1]
来源：http://wa.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://qu.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://rz.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://zc.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yy.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://ut.newstarts.cn

Ruby: s == s.reverse
来源：http://ya.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hb.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://mw.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nt.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://au.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jz.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://zf.newstarts.cn

Java: // 手写 HashMap
来源：http://dw.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ym.panjiajie.cn

Ruby: // 手写 Hash
来源：http://pb.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wq.hnjuh.cn

[N08] 生成全排列
来源：http://gp.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://zr.newstarts.cn

PHP:  // 手写递归交换
来源：http://vb.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://zk.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://gk.lnxyls.cn

Java: // 手写回溯递归
来源：http://yt.shxzukj.cn

Go:   // 手写回溯递归
来源：http://qh.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://wu.hnjuh.cn

C#:   // 手写回溯递归
来源：http://fn.9csxet.cn

[N09] 栈与队列
来源：http://rc.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eb.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ts.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://da.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kl.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oh.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ov.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pc.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://li.wgjwhj.cn

[N10] 链表节点定义
来源：http://gz.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ci.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mn.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eg.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qo.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://np.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yd.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xx.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mn.521024.cn

[N11] 二叉树中序遍历
来源：http://uu.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kd.szxytkj.cn

PHP:  // 手写递归函数
来源：http://km.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dx.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ol.muxihuayi.cn

Java: // 手写递归
来源：http://vp.gzmigu.cn

Go:   // 手写递归
来源：http://yr.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ab.szsharing.cn

C#:   // 手写递归
来源：http://ef.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dj.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://je.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dw.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gp.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wz.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yw.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fm.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cp.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ij.yuntaijiaju.cn

================================================================================
来源：http://yo.yuexingan06.cn

O. 并发与异步
来源：http://xl.521024.cn

================================================================================
来源：http://fw.wgjwhj.cn

[O01] 启动一个线程
来源：http://da.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sm.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vk.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vy.bjjhwx.cn

TS:   // 同 JS
来源：http://fe.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://gf.huixiangedu.cn

Go:   go f()
来源：http://zk.szsharing.cn

Ruby: Thread.new { f }
来源：http://qr.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://gu.nicolike.cn

[O02] 使用线程池
来源：http://fq.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lw.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xe.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ab.9csxet.cn

TS:   // worker_threads 线程池
来源：http://oh.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vo.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sm.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oj.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ab.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://pc.nszjky.cn

Py:   with lock: shared += 1
来源：http://bi.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://di.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bh.wgjwhj.cn

TS:   // 同 JS
来源：http://bt.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://zy.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pu.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ig.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://nx.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://vd.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://eh.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fx.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://wp.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nk.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rt.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fm.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ve.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://nd.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://jg.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://tv.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lv.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://ux.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://sg.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ov.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gi.huanxung.cn

Ruby: threads.map(&:join)
来源：http://jp.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fd.shxzukj.cn

[O06] 使用进程池
来源：http://lr.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://au.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ad.asd995.cn

JS:   // child_process / cluster 模块
来源：http://kc.colortex.cn

TS:   // child_process / cluster 模块
来源：http://hk.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lg.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cv.huanxung.cn

Ruby: // fork 块
来源：http://me.yuexingan06.cn

C#:   Parallel.For
来源：http://jv.muxihuayi.cn

================================================================================
来源：http://kx.bookmarksfly.cn

P. 常用工具函数
来源：http://rz.wgjwhj.cn

================================================================================
来源：http://kx.yuexingan06.cn

[P01] 生成 UUID
来源：http://wo.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://lt.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ff.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://mn.521024.cn

TS:   crypto.randomUUID()
来源：http://ly.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://bj.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://tz.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ke.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://jl.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://uy.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vg.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dx.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ew.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eh.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ww.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://it.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ra.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wc.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://ir.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dj.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bm.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qt.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hc.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zy.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ft.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bf.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qh.szxytkj.cn

[P04] 求长度
来源：http://lv.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dp.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wu.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://no.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cz.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://xy.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://dl.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://bl.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fd.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://cu.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uf.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ir.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nv.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wi.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nh.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ol.jianghongdianzi.cn

Ruby: a == b
来源：http://xo.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mq.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tn.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dh.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://ux.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lx.nszjky.cn

TS:   if (x == null) {}
来源：http://ec.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://la.bjjhwx.cn

Go:   if x == nil {}
来源：http://ss.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wb.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://tb.nicolike.cn

[P07] 防抖与节流
来源：http://of.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cm.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://af.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ku.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cw.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://an.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bj.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vj.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ed.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://io.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wr.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ex.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hg.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hb.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jk.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://db.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ow.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qs.hahajie.cn

================================================================================
来源：http://on.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bb.jctech888.com.cn

================================================================================
来源：http://hr.shxzskj.cn

[Q01] 创建表
来源：http://ru.521024.cn

CREATE TABLE users (
来源：http://az.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kp.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://kf.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://jd.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fw.huixinmuqiang.cn

);
来源：http://xq.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://fb.521024.cn

CREATE TABLE orders (
来源：http://go.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://im.hahajie.cn

user_id INT NOT NULL,
来源：http://ac.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://lm.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wu.asd995.cn

);
来源：http://py.9csxet.cn

[Q03] 增加列
来源：http://vm.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xl.521024.cn

[Q04] 修改列类型
来源：http://nx.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oh.yuexingan06.cn

[Q05] 重命名列
来源：http://qg.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.9csxet.cn

[Q06] 删除列
来源：http://sp.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://re.newstarts.cn

[Q07] 删除表
来源：http://sx.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://up.jctech888.com.cn

[Q08] 创建普通索引
来源：http://ds.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rj.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://ai.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zm.lnxyls.cn

[Q10] 插入单行
来源：http://ig.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://or.shxzukj.cn

[Q11] 一次插入多行
来源：http://kk.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mj.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://tz.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mu.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lo.asd995.cn

[Q13] 忽略重复插入
来源：http://xj.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qu.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://xk.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ph.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oa.szsharing.cn

[Q15] 查询全部
来源：http://kv.wgjwhj.cn

SELECT * FROM users;
来源：http://cd.huanxung.cn

[Q16] 查询指定列
来源：http://wd.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://fl.jctech888.com.cn

[Q17] 条件查询
来源：http://uh.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ym.shxzskj.cn

[Q18] 模糊匹配
来源：http://kq.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kt.colortex.cn

[Q19] 范围查询
来源：http://ii.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vy.szsharing.cn

[Q20] IN 列表
来源：http://ma.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xy.lnxyls.cn

[Q21] 空值判断
来源：http://xd.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fa.bjjhwx.cn

[Q22] 排序
来源：http://fi.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ls.szsharing.cn

[Q23] 分页
来源：http://lo.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://by.newstarts.cn

[Q24] 去重
来源：http://jo.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://ka.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://lk.shtwfgs.cn


<!-- 参考信息 -->