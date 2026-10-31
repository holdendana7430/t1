代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wk.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ey.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ua.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sd.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ad.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pc.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cd.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://ry.hahajie.cn

Ruby: arr.sort
来源：http://ef.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xa.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://sw.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pz.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://yl.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jd.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wj.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fw.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jp.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ph.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://so.lnxyls.cn

[N04] 斐波那契数列
来源：http://vx.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jd.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hl.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gc.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wb.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fm.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zd.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://je.wgjwhj.cn

[N05] 最大公约数
来源：http://ns.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://cj.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fb.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ru.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iw.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ls.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://po.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tx.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://si.shxzukj.cn

Py:   s == s[::-1]
来源：http://lj.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://gx.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://cj.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://sv.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ab.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://mw.asd995.cn

Ruby: s == s.reverse
来源：http://fi.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hk.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://jr.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uo.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ef.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fh.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://jv.gzmigu.cn

Java: // 手写 HashMap
来源：http://nz.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://qc.panjiajie.cn

Ruby: // 手写 Hash
来源：http://zn.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yr.asd995.cn

[N08] 生成全排列
来源：http://uf.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://kb.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://fl.newstarts.cn

JS:   // 手写回溯递归
来源：http://hy.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://vj.jctech888.com.cn

Java: // 手写回溯递归
来源：http://oh.hahajie.cn

Go:   // 手写回溯递归
来源：http://ui.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://qb.colortex.cn

C#:   // 手写回溯递归
来源：http://lc.nszjky.cn

[N09] 栈与队列
来源：http://wr.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vs.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ws.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uq.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gk.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yv.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hy.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://zf.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sr.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nv.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xv.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yc.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://bj.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cq.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://if.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://em.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://iq.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ko.huanxung.cn

PHP:  // 手写递归函数
来源：http://mv.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ac.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yh.hnjuh.cn

Java: // 手写递归
来源：http://iv.newstarts.cn

Go:   // 手写递归
来源：http://uj.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lm.muxihuayi.cn

C#:   // 手写递归
来源：http://ir.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lc.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wl.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zp.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yy.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ck.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wm.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xc.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qn.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://do.szxytkj.cn

O. 并发与异步
来源：http://fp.muxihuayi.cn

================================================================================
来源：http://np.wgjwhj.cn

[O01] 启动一个线程
来源：http://ic.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sd.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://il.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qh.panjiajie.cn

TS:   // 同 JS
来源：http://lb.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://ro.szsharing.cn

Go:   go f()
来源：http://sq.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://vk.asd995.cn

C#:   Task.Run(() => F());
来源：http://mv.newstarts.cn

[O02] 使用线程池
来源：http://ei.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xm.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kk.asd995.cn

JS:   // worker_threads 线程池
来源：http://km.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://dx.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://si.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ji.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mh.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rr.newstarts.cn

[O03] 加锁保护共享数据
来源：http://wt.hnjuh.cn

Py:   with lock: shared += 1
来源：http://wa.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://mw.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ku.lnxyls.cn

TS:   // 同 JS
来源：http://rr.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://ol.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yi.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rs.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ch.asd995.cn

[O04] 定义异步函数并等待
来源：http://vr.521024.cn

Py:   async def f():⏎    await g()
来源：http://oy.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dn.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://wk.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vj.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hx.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ig.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uk.asd995.cn

C#:   async Task F() { await G(); }
来源：http://nc.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://lm.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://sl.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bi.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://zo.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://ke.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sq.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xw.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://fg.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cp.9csxet.cn

[O06] 使用进程池
来源：http://nt.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cc.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jl.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://cp.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://us.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://to.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://js.huanxung.cn

Ruby: // fork 块
来源：http://qn.bookmarksfly.cn

C#:   Parallel.For
来源：http://hn.shxzskj.cn

================================================================================
来源：http://vb.newstarts.cn

P. 常用工具函数
来源：http://nv.nicolike.cn

================================================================================
来源：http://wf.szsharing.cn

[P01] 生成 UUID
来源：http://wb.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://hs.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jt.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://wp.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://vk.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://mx.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://if.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://gn.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://xg.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://hx.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ju.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pf.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ja.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ws.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uj.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ap.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ek.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pf.nicolike.cn

[P03] 生成短随机字符串
来源：http://fa.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uo.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qk.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qo.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ir.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yp.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vl.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zz.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tf.gzmigu.cn

[P04] 求长度
来源：http://qk.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tv.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rf.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bx.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bu.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://tb.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://ok.hnjuh.cn

Ruby: x.length;  x.size
来源：http://xd.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zg.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://cr.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vy.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ek.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sa.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tj.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rk.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yy.hahajie.cn

Ruby: a == b
来源：http://nn.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ja.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hf.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ou.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://td.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oy.muxihuayi.cn

TS:   if (x == null) {}
来源：http://os.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sy.yuexingan06.cn

Go:   if x == nil {}
来源：http://al.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cu.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://di.shtwfgs.cn

[P07] 防抖与节流
来源：http://se.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lo.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://rv.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dh.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://np.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vt.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ue.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fc.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sk.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://oi.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://je.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ph.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lx.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zy.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ju.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ar.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zu.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tv.asd995.cn

================================================================================
来源：http://tz.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uw.9csxet.cn

================================================================================
来源：http://hs.shxzskj.cn

[Q01] 创建表
来源：http://dp.szxytkj.cn

CREATE TABLE users (
来源：http://ry.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fy.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://pw.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://qz.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://la.muxihuayi.cn

);
来源：http://dh.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://sw.newstarts.cn

CREATE TABLE orders (
来源：http://os.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bs.huanxung.cn

user_id INT NOT NULL,
来源：http://pm.asd995.cn

amount DECIMAL(10, 2),
来源：http://bf.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://al.gzmigu.cn

);
来源：http://yx.szxytkj.cn

[Q03] 增加列
来源：http://ne.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lo.shxzskj.cn

[Q04] 修改列类型
来源：http://en.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bb.shtwfgs.cn

[Q05] 重命名列
来源：http://hc.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ym.jctech888.com.cn

[Q06] 删除列
来源：http://pa.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tj.shxzskj.cn

[Q07] 删除表
来源：http://yk.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://et.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://uf.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hn.gzmigu.cn

[Q09] 创建唯一索引
来源：http://vv.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eb.huanxung.cn

[Q10] 插入单行
来源：http://gn.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xy.muxihuayi.cn

[Q11] 一次插入多行
来源：http://ad.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rs.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://gw.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ri.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ki.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://dj.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ja.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://rc.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xd.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gy.colortex.cn

[Q15] 查询全部
来源：http://kc.bookmarksfly.cn

SELECT * FROM users;
来源：http://wx.lnxyls.cn

[Q16] 查询指定列
来源：http://qr.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://qf.shxzukj.cn

[Q17] 条件查询
来源：http://ep.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ov.jctech888.com.cn

[Q18] 模糊匹配
来源：http://lo.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://id.muxihuayi.cn

[Q19] 范围查询
来源：http://yn.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bt.huanxung.cn

[Q20] IN 列表
来源：http://hf.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ve.lnxyls.cn

[Q21] 空值判断
来源：http://wo.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vi.lnxyls.cn

[Q22] 排序
来源：http://zt.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tp.shxzukj.cn

[Q23] 分页
来源：http://cz.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ra.muxihuayi.cn

[Q24] 去重
来源：http://bq.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://dh.shxzukj.cn

[Q25] 只取前 N 条
来源：http://nx.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ms.shxzukj.cn

[Q26] 计数
来源：http://uk.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://hi.asd995.cn

[Q27] 条件计数
来源：http://wu.hnjuh.cn


<!-- 参考信息 -->