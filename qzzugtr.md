代发 wailian999

TS:   process.platform;  process.version
来源：http://lk.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oc.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tv.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qy.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hf.szsharing.cn

================================================================================
来源：http://ru.wgjwhj.cn

N. 数据结构与算法
来源：http://ij.9csxet.cn

================================================================================
来源：http://jr.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://ib.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lh.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://io.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uc.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lf.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vu.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://wo.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ei.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iy.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://yi.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://qe.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zz.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nf.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fr.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sh.szsharing.cn

Go:   slices.Sort(arr)
来源：http://fg.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ne.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hm.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://qt.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ye.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://so.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tx.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sj.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cf.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qc.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vk.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pl.colortex.cn

[N04] 斐波那契数列
来源：http://vf.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jx.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sc.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://il.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wx.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://le.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qj.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nw.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bg.colortex.cn

[N05] 最大公约数
来源：http://wv.asd995.cn

Py:   math.gcd(a, b)
来源：http://qt.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ds.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fl.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xb.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vy.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jx.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ej.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xu.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://rs.haigaiapp.cn

Py:   s == s[::-1]
来源：http://hz.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://bu.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://yf.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://eb.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ir.huanxung.cn

Go:   // 双指针从两端比较
来源：http://hz.nszjky.cn

Ruby: s == s.reverse
来源：http://ip.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zi.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://en.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nz.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fp.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eu.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://za.nszjky.cn

Java: // 手写 HashMap
来源：http://rd.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://df.hahajie.cn

Ruby: // 手写 Hash
来源：http://hr.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vu.521024.cn

[N08] 生成全排列
来源：http://ox.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://fe.shxzskj.cn

PHP:  // 手写递归交换
来源：http://un.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://ro.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://xj.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://fk.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://rg.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://fu.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://pe.yuexingan06.cn

[N09] 栈与队列
来源：http://zi.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bo.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dc.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sz.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ih.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ll.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vu.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vm.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://au.gzmigu.cn

[N10] 链表节点定义
来源：http://wn.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hq.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://md.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hd.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gm.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://cy.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ja.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yy.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ik.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://gr.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bo.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://wn.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sw.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jd.hnjuh.cn

Java: // 手写递归
来源：http://fr.wgjwhj.cn

Go:   // 手写递归
来源：http://qq.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://np.bookmarksfly.cn

C#:   // 手写递归
来源：http://tn.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://el.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iz.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sd.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zr.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ah.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gz.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ua.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dg.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dj.chemitech.net.cn

================================================================================
来源：http://wk.yuexingan06.cn

O. 并发与异步
来源：http://kf.yuntaijiaju.cn

================================================================================
来源：http://xf.haigaiapp.cn

[O01] 启动一个线程
来源：http://gq.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ye.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yz.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eg.huixiangedu.cn

TS:   // 同 JS
来源：http://nb.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://fx.panjiajie.cn

Go:   go f()
来源：http://fs.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://yj.newstarts.cn

C#:   Task.Run(() => F());
来源：http://an.jctech888.com.cn

[O02] 使用线程池
来源：http://ga.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gc.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fy.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://kv.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://mf.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xa.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hv.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://np.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gq.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://rr.szsharing.cn

Py:   with lock: shared += 1
来源：http://ln.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ya.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qe.bjjhwx.cn

TS:   // 同 JS
来源：http://uv.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://bb.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yi.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mp.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ln.nszjky.cn

[O04] 定义异步函数并等待
来源：http://hq.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://hm.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xs.huanxung.cn

JS:   async function f() { await g(); }
来源：http://ms.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sz.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qf.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ol.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mu.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://nl.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://wz.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://oz.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yt.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://tb.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://jy.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xc.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iz.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://rq.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pv.hnjuh.cn

[O06] 使用进程池
来源：http://nn.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vi.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pr.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://aq.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://kf.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bh.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ja.bookmarksfly.cn

Ruby: // fork 块
来源：http://mz.huixiangedu.cn

C#:   Parallel.For
来源：http://km.asd995.cn

================================================================================
来源：http://zj.hahajie.cn

P. 常用工具函数
来源：http://cp.panjiajie.cn

================================================================================
来源：http://jj.bookmarksfly.cn

[P01] 生成 UUID
来源：http://vx.521024.cn

Py:   str(uuid.uuid4())
来源：http://wf.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tm.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://qg.hahajie.cn

TS:   crypto.randomUUID()
来源：http://or.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://pz.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://uk.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://ue.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://qi.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://ty.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nl.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hr.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xy.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fi.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oz.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xv.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ca.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://la.panjiajie.cn

[P03] 生成短随机字符串
来源：http://iw.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eu.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qb.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tw.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tu.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gz.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jv.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ex.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oi.panjiajie.cn

[P04] 求长度
来源：http://bw.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vu.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tu.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ov.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://pc.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://nc.newstarts.cn

Ruby: x.length;  x.size
来源：http://ye.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ul.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://kz.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ie.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qo.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yj.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tl.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hx.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zo.bookmarksfly.cn

Ruby: a == b
来源：http://fe.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pl.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pk.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jo.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://qn.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jd.nszjky.cn

TS:   if (x == null) {}
来源：http://re.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ih.haigaiapp.cn

Go:   if x == nil {}
来源：http://oa.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qg.huanxung.cn

C#:   if (x is null) {}
来源：http://ch.shxzukj.cn

[P07] 防抖与节流
来源：http://ww.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zh.colortex.cn

PHP:  // 手写时间戳比较
来源：http://jl.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mi.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ol.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gj.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qd.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xy.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://la.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://wc.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rg.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kd.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dt.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jv.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jj.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iv.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qx.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lj.huixinmuqiang.cn

================================================================================
来源：http://ay.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dg.colortex.cn

================================================================================
来源：http://af.muxihuayi.cn

[Q01] 创建表
来源：http://be.szxytkj.cn

CREATE TABLE users (
来源：http://cj.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zs.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://uy.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://zx.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uy.hnjuh.cn

);
来源：http://iy.nicolike.cn

[Q02] 创建带外键的表
来源：http://cs.gzmigu.cn

CREATE TABLE orders (
来源：http://bh.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wl.gzmigu.cn

user_id INT NOT NULL,
来源：http://pk.nszjky.cn

amount DECIMAL(10, 2),
来源：http://dh.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zb.9csxet.cn

);
来源：http://qs.yuntaijiaju.cn

[Q03] 增加列
来源：http://ry.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zr.shxzskj.cn

[Q04] 修改列类型
来源：http://rh.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wb.gzmigu.cn

[Q05] 重命名列
来源：http://gc.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jt.bookmarksfly.cn

[Q06] 删除列
来源：http://fu.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vz.bjjhwx.cn

[Q07] 删除表
来源：http://kr.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://ed.chemitech.net.cn

[Q08] 创建普通索引
来源：http://uo.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mc.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ek.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ul.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ay.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oh.huanxung.cn

[Q11] 一次插入多行
来源：http://fj.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sp.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://dd.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jr.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yv.lnxyls.cn

[Q13] 忽略重复插入
来源：http://vy.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ie.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://ow.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pa.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hl.asd995.cn

[Q15] 查询全部
来源：http://fp.shxzukj.cn

SELECT * FROM users;
来源：http://ex.shtwfgs.cn

[Q16] 查询指定列
来源：http://zd.szxytkj.cn

SELECT id, name FROM users;
来源：http://ma.nszjky.cn

[Q17] 条件查询
来源：http://kz.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dy.9csxet.cn

[Q18] 模糊匹配
来源：http://sx.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ai.nszjky.cn

[Q19] 范围查询
来源：http://ld.jctech888.com.cn


<!-- 参考信息 -->