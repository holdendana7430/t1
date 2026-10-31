代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aj.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wl.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://fb.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ln.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ol.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://vi.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://cr.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vy.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zt.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bk.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nj.9csxet.cn

Go:   slices.Sort(arr)
来源：http://hf.yuntaijiaju.cn

Ruby: arr.sort
来源：http://st.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pp.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://ss.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://el.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://bg.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cv.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dr.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rk.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dt.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://go.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ba.asd995.cn

[N04] 斐波那契数列
来源：http://cd.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kx.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rh.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gg.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jt.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tc.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ss.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jh.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eg.chemitech.net.cn

[N05] 最大公约数
来源：http://wz.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://kz.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://el.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xo.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mc.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qn.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xr.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://gd.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vs.nicolike.cn

[N06] 判断回文字符串
来源：http://dt.bjjhwx.cn

Py:   s == s[::-1]
来源：http://vq.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://mc.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://xe.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://ar.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://up.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://fb.nszjky.cn

Ruby: s == s.reverse
来源：http://vs.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://il.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://xv.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vk.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ig.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ss.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://cy.lnxyls.cn

Java: // 手写 HashMap
来源：http://uy.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://vp.shxzskj.cn

Ruby: // 手写 Hash
来源：http://dx.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gu.hnjuh.cn

[N08] 生成全排列
来源：http://se.521024.cn

Py:   itertools.permutations(arr)
来源：http://jk.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://es.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://gr.panjiajie.cn

TS:   // 手写回溯递归
来源：http://ul.shxzskj.cn

Java: // 手写回溯递归
来源：http://nw.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://gu.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ze.panjiajie.cn

C#:   // 手写回溯递归
来源：http://oo.huanxung.cn

[N09] 栈与队列
来源：http://eh.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jp.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://am.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nk.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ey.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ze.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fs.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sp.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jl.huixiangedu.cn

[N10] 链表节点定义
来源：http://ns.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dt.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dj.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://op.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ed.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://zo.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oj.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jp.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://wi.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mv.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://af.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hd.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uo.jianghongdianzi.cn

Java: // 手写递归
来源：http://iu.shxzukj.cn

Go:   // 手写递归
来源：http://ms.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vw.newstarts.cn

C#:   // 手写递归
来源：http://cy.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mz.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kl.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tr.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gz.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://as.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://df.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ga.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dn.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://re.bookmarksfly.cn

================================================================================
来源：http://xf.muxihuayi.cn

O. 并发与异步
来源：http://fv.szsharing.cn

================================================================================
来源：http://uz.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://pz.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hm.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gu.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wg.huanxung.cn

TS:   // 同 JS
来源：http://yf.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://bq.bjjhwx.cn

Go:   go f()
来源：http://ib.nszjky.cn

Ruby: Thread.new { f }
来源：http://tx.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://zj.yuexingan06.cn

[O02] 使用线程池
来源：http://lj.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ns.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kt.asd995.cn

JS:   // worker_threads 线程池
来源：http://uk.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://cp.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pc.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vm.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gc.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ro.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://eo.lnxyls.cn

Py:   with lock: shared += 1
来源：http://ia.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://cf.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cf.panjiajie.cn

TS:   // 同 JS
来源：http://rn.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://fv.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ns.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hg.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://zn.szsharing.cn

[O04] 定义异步函数并等待
来源：http://cp.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://db.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rw.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://kk.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vw.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rs.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jd.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zm.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://un.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://wi.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://mk.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rs.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://hb.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://nh.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xm.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tm.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://li.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ke.huixinmuqiang.cn

[O06] 使用进程池
来源：http://jw.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wz.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zp.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://ux.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://qh.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jw.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fw.bookmarksfly.cn

Ruby: // fork 块
来源：http://ql.bookmarksfly.cn

C#:   Parallel.For
来源：http://vp.nicolike.cn

================================================================================
来源：http://gm.bookmarksfly.cn

P. 常用工具函数
来源：http://wt.haigaiapp.cn

================================================================================
来源：http://gi.hnjuh.cn

[P01] 生成 UUID
来源：http://zg.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://yk.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tw.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://xt.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://go.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://wz.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://uu.colortex.cn

Ruby: SecureRandom.uuid
来源：http://co.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://cf.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://bu.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ao.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tb.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mw.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lx.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ij.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hk.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pp.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://an.521024.cn

[P03] 生成短随机字符串
来源：http://eh.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://de.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uz.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lw.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mp.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vr.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://un.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bi.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://el.huixinmuqiang.cn

[P04] 求长度
来源：http://nf.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kq.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gj.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kh.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ci.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://bl.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://cf.nszjky.cn

Ruby: x.length;  x.size
来源：http://lh.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aa.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://kh.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vy.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://no.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://im.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bi.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ah.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ll.colortex.cn

Ruby: a == b
来源：http://em.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ff.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xm.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wk.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://uf.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nq.hnjuh.cn

TS:   if (x == null) {}
来源：http://no.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kv.9csxet.cn

Go:   if x == nil {}
来源：http://za.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fw.nicolike.cn

C#:   if (x is null) {}
来源：http://hs.newstarts.cn

[P07] 防抖与节流
来源：http://rh.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zc.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ae.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rg.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tf.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qd.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lz.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ov.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kj.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://gb.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lk.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aq.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://we.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tp.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cb.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://go.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sl.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://da.lnxyls.cn

================================================================================
来源：http://qq.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mn.9csxet.cn

================================================================================
来源：http://ew.huanxung.cn

[Q01] 创建表
来源：http://cm.panjiajie.cn

CREATE TABLE users (
来源：http://bo.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://hp.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://sk.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yx.panjiajie.cn

);
来源：http://so.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://lr.shxzskj.cn

CREATE TABLE orders (
来源：http://pc.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oy.szsharing.cn

user_id INT NOT NULL,
来源：http://wl.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://hs.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nz.lnxyls.cn

);
来源：http://ap.hahajie.cn

[Q03] 增加列
来源：http://ir.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zy.9csxet.cn

[Q04] 修改列类型
来源：http://rp.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ug.yuexingan06.cn

[Q05] 重命名列
来源：http://sm.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vp.asd995.cn

[Q06] 删除列
来源：http://tz.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fr.huixinmuqiang.cn

[Q07] 删除表
来源：http://ag.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://db.shtwfgs.cn

[Q08] 创建普通索引
来源：http://nw.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rx.nicolike.cn

[Q09] 创建唯一索引
来源：http://cv.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yn.newstarts.cn

[Q10] 插入单行
来源：http://vw.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jb.lnxyls.cn

[Q11] 一次插入多行
来源：http://uk.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jw.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://cp.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xn.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://co.lnxyls.cn

[Q13] 忽略重复插入
来源：http://tg.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sa.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ud.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vh.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.colortex.cn

[Q15] 查询全部
来源：http://ty.szsharing.cn

SELECT * FROM users;
来源：http://ik.wgjwhj.cn

[Q16] 查询指定列
来源：http://jd.hahajie.cn

SELECT id, name FROM users;
来源：http://ba.colortex.cn

[Q17] 条件查询
来源：http://ct.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dn.jctech888.com.cn

[Q18] 模糊匹配
来源：http://mz.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hd.nszjky.cn

[Q19] 范围查询
来源：http://sr.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ji.bookmarksfly.cn

[Q20] IN 列表
来源：http://qs.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kl.huixinmuqiang.cn

[Q21] 空值判断
来源：http://qt.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mu.panjiajie.cn

[Q22] 排序
来源：http://bd.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://td.shxzukj.cn

[Q23] 分页
来源：http://yb.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.panjiajie.cn

[Q24] 去重
来源：http://gl.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://lm.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://gt.szsharing.cn


<!-- 参考信息 -->