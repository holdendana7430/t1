代发 wailian999

TS:   process.platform;  process.version
来源：http://wd.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vz.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lt.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dq.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ws.yuntaijiaju.cn

================================================================================
来源：http://pd.nszjky.cn

N. 数据结构与算法
来源：http://eh.hnjuh.cn

================================================================================
来源：http://qg.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://dt.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nm.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jd.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gu.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qw.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rz.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://jy.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iu.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ny.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://tg.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://xm.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hf.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ko.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bo.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://an.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://qx.hahajie.cn

Ruby: arr.sort
来源：http://rm.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://je.colortex.cn

[N03] 快速排序（分治示例）
来源：http://rh.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pl.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://zm.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yz.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://il.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xa.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hv.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gw.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pd.panjiajie.cn

[N04] 斐波那契数列
来源：http://qa.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gd.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zd.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jr.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aq.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qk.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pr.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xn.newstarts.cn

[N05] 最大公约数
来源：http://bv.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://pm.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lt.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eh.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rs.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tg.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pn.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://fr.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oi.huixiangedu.cn

[N06] 判断回文字符串
来源：http://cp.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://tz.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://my.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://hg.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://np.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qe.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://gc.huanxung.cn

Ruby: s == s.reverse
来源：http://tu.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lx.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://qw.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cb.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oe.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jy.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://dr.nicolike.cn

Java: // 手写 HashMap
来源：http://ca.nicolike.cn

Go:   // 手写 map[int]int
来源：http://vd.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ij.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yo.9csxet.cn

[N08] 生成全排列
来源：http://wc.521024.cn

Py:   itertools.permutations(arr)
来源：http://ia.shxzukj.cn

PHP:  // 手写递归交换
来源：http://up.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://eu.nicolike.cn

TS:   // 手写回溯递归
来源：http://iy.gzmigu.cn

Java: // 手写回溯递归
来源：http://ms.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://in.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://hw.panjiajie.cn

C#:   // 手写回溯递归
来源：http://ga.haigaiapp.cn

[N09] 栈与队列
来源：http://ac.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bt.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mq.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oa.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qd.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ck.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dc.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vo.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nd.newstarts.cn

[N10] 链表节点定义
来源：http://xb.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yq.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nq.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ki.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fd.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ht.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lo.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ok.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ql.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://hq.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ej.nicolike.cn

PHP:  // 手写递归函数
来源：http://he.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rb.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qs.shxzukj.cn

Java: // 手写递归
来源：http://yt.hnjuh.cn

Go:   // 手写递归
来源：http://gf.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lf.shxzukj.cn

C#:   // 手写递归
来源：http://vz.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ok.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qw.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ae.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kk.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qs.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://py.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zp.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ij.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.szsharing.cn

================================================================================
来源：http://et.nszjky.cn

O. 并发与异步
来源：http://dq.szsharing.cn

================================================================================
来源：http://ql.nicolike.cn

[O01] 启动一个线程
来源：http://wc.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://px.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oi.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dq.gzmigu.cn

TS:   // 同 JS
来源：http://km.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://hu.muxihuayi.cn

Go:   go f()
来源：http://eu.asd995.cn

Ruby: Thread.new { f }
来源：http://io.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://gs.yuntaijiaju.cn

[O02] 使用线程池
来源：http://fd.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kl.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cg.huanxung.cn

JS:   // worker_threads 线程池
来源：http://iu.newstarts.cn

TS:   // worker_threads 线程池
来源：http://re.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xi.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gb.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dz.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fs.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://dz.521024.cn

Py:   with lock: shared += 1
来源：http://vk.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://rq.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bz.gzmigu.cn

TS:   // 同 JS
来源：http://du.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://tf.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hp.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kl.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://vx.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://hv.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://kv.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zx.521024.cn

JS:   async function f() { await g(); }
来源：http://iv.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cn.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xk.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dm.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ek.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://md.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://kf.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://ul.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fe.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://ty.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ec.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://li.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yo.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://it.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vs.huixiangedu.cn

[O06] 使用进程池
来源：http://tk.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pu.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://us.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://yh.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://jn.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ct.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ja.haigaiapp.cn

Ruby: // fork 块
来源：http://dc.bjjhwx.cn

C#:   Parallel.For
来源：http://vd.szxytkj.cn

================================================================================
来源：http://rs.yuexingan06.cn

P. 常用工具函数
来源：http://mt.panjiajie.cn

================================================================================
来源：http://rx.bookmarksfly.cn

[P01] 生成 UUID
来源：http://nn.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://wy.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oc.hahajie.cn

JS:   crypto.randomUUID()
来源：http://ro.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://ab.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://um.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://gc.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://ni.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://bt.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://nh.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xd.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cs.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fo.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vz.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xl.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://co.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yh.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://og.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://wk.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rm.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vq.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gf.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tq.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yi.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gd.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lg.shtwfgs.cn

[P04] 求长度
来源：http://dc.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qs.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xf.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mm.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://yq.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://if.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://bq.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cq.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://bj.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://va.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nx.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gj.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qm.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mu.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wi.szxytkj.cn

Ruby: a == b
来源：http://hg.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lk.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nx.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zl.521024.cn

PHP:  if (empty($x)) {}
来源：http://hs.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ad.9csxet.cn

TS:   if (x == null) {}
来源：http://rx.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hk.szsharing.cn

Go:   if x == nil {}
来源：http://cq.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://me.shxzskj.cn

C#:   if (x is null) {}
来源：http://as.bjjhwx.cn

[P07] 防抖与节流
来源：http://pk.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nt.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://uq.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sl.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fe.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ca.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jz.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://nh.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://az.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wl.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rf.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hl.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wc.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://di.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qu.huixinmuqiang.cn

================================================================================
来源：http://gs.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://og.szsharing.cn

================================================================================
来源：http://ej.9csxet.cn

[Q01] 创建表
来源：http://ag.hnjuh.cn

CREATE TABLE users (
来源：http://wv.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ay.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://ll.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://db.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zj.yuntaijiaju.cn

);
来源：http://cf.shxzskj.cn

[Q02] 创建带外键的表
来源：http://rg.nicolike.cn

CREATE TABLE orders (
来源：http://fu.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nu.szxytkj.cn

user_id INT NOT NULL,
来源：http://qz.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://hz.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zg.yuntaijiaju.cn

);
来源：http://zc.muxihuayi.cn

[Q03] 增加列
来源：http://kd.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wn.jctech888.com.cn

[Q04] 修改列类型
来源：http://jr.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ce.lnxyls.cn

[Q05] 重命名列
来源：http://zn.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ck.jctech888.com.cn

[Q06] 删除列
来源：http://cl.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jb.huanxung.cn

[Q07] 删除表
来源：http://ns.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://ig.shxzukj.cn

[Q08] 创建普通索引
来源：http://ss.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zn.colortex.cn

[Q09] 创建唯一索引
来源：http://fd.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pe.nszjky.cn

[Q10] 插入单行
来源：http://uw.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qm.wgjwhj.cn

[Q11] 一次插入多行
来源：http://dw.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://an.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ag.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tq.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ru.nicolike.cn

[Q13] 忽略重复插入
来源：http://px.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ne.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://sc.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jz.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://om.huixinmuqiang.cn

[Q15] 查询全部
来源：http://dw.wgjwhj.cn

SELECT * FROM users;
来源：http://nt.huixiangedu.cn

[Q16] 查询指定列
来源：http://tx.lnxyls.cn

SELECT id, name FROM users;
来源：http://cb.521024.cn

[Q17] 条件查询
来源：http://ov.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nx.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://xq.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dp.nszjky.cn

[Q19] 范围查询
来源：http://up.wgjwhj.cn


<!-- 参考信息 -->