代发 wailian999

[M08] 获取系统与运行时信息
来源：http://fk.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ae.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://qs.shxzukj.cn

JS:   process.platform;  process.version
来源：http://om.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://rc.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cg.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mw.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://me.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ph.hnjuh.cn

================================================================================
来源：http://qy.nicolike.cn

N. 数据结构与算法
来源：http://jb.huanxung.cn

================================================================================
来源：http://yi.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://va.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ue.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vd.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nt.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://he.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://md.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xl.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tp.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://uh.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://rk.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jf.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hy.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gg.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ns.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://ea.bjjhwx.cn

Ruby: arr.sort
来源：http://jq.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nj.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://oz.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kx.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://pk.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://da.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fk.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kn.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cb.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xy.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://pu.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aq.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kd.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fm.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yc.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rl.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ho.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bu.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://do.asd995.cn

[N05] 最大公约数
来源：http://gg.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://sg.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hg.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lt.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nm.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wr.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vg.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://mh.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qp.nicolike.cn

[N06] 判断回文字符串
来源：http://va.521024.cn

Py:   s == s[::-1]
来源：http://wd.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://qe.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://wt.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://os.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xu.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://gr.nicolike.cn

Ruby: s == s.reverse
来源：http://ni.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mj.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://iv.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yv.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zi.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ca.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://ht.gzmigu.cn

Java: // 手写 HashMap
来源：http://sg.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://dk.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://bg.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jk.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ro.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://sj.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://ad.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ll.panjiajie.cn

TS:   // 手写回溯递归
来源：http://yd.shxzukj.cn

Java: // 手写回溯递归
来源：http://oo.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://if.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://gb.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://hx.haigaiapp.cn

[N09] 栈与队列
来源：http://ye.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ly.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mm.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oa.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mf.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vo.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oa.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rq.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yj.shxzskj.cn

[N10] 链表节点定义
来源：http://xi.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yf.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kg.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xb.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.asd995.cn

Java: class Node { int v; Node next; }
来源：http://jy.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dp.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ti.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mq.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://tl.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qo.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://at.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rj.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nc.colortex.cn

Java: // 手写递归
来源：http://wb.hahajie.cn

Go:   // 手写递归
来源：http://vs.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sl.lnxyls.cn

C#:   // 手写递归
来源：http://ab.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ib.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fx.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jc.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qy.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://go.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iz.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lo.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qf.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://js.colortex.cn

================================================================================
来源：http://lv.lnxyls.cn

O. 并发与异步
来源：http://br.szxytkj.cn

================================================================================
来源：http://hu.shxzskj.cn

[O01] 启动一个线程
来源：http://nj.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xj.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iy.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://su.gzmigu.cn

TS:   // 同 JS
来源：http://dy.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://kf.haigaiapp.cn

Go:   go f()
来源：http://lm.szsharing.cn

Ruby: Thread.new { f }
来源：http://df.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://mn.bjjhwx.cn

[O02] 使用线程池
来源：http://uz.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wl.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mq.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://pw.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://pe.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://df.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mu.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jk.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nd.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://ok.9csxet.cn

Py:   with lock: shared += 1
来源：http://hl.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://jc.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pl.yuexingan06.cn

TS:   // 同 JS
来源：http://cp.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://yy.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fe.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cv.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://si.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ea.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://pb.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://to.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://xs.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iw.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nf.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ag.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ce.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://dy.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://dw.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://oi.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nx.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://lx.colortex.cn

TS:   await Promise.all(tasks)
来源：http://jp.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cc.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ty.huanxung.cn

Ruby: threads.map(&:join)
来源：http://yc.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tq.gzmigu.cn

[O06] 使用进程池
来源：http://tn.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ss.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dr.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://oq.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://tv.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eu.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bf.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ek.hahajie.cn

C#:   Parallel.For
来源：http://ue.newstarts.cn

================================================================================
来源：http://jh.9csxet.cn

P. 常用工具函数
来源：http://jz.nicolike.cn

================================================================================
来源：http://yo.wgjwhj.cn

[P01] 生成 UUID
来源：http://bt.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://bq.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://di.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://xk.szsharing.cn

TS:   crypto.randomUUID()
来源：http://lc.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://np.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://ld.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://tw.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://sn.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://gh.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bn.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yy.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xt.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ua.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bk.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uy.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xv.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uf.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://zn.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://co.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hm.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lf.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eb.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ko.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gu.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ru.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mq.jianghongdianzi.cn

[P04] 求长度
来源：http://fm.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ev.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oo.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ql.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lt.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://si.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://us.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://sb.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://si.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://di.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bj.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://of.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ch.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sw.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wx.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://to.9csxet.cn

Ruby: a == b
来源：http://dj.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vq.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zo.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vi.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://rw.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yg.lnxyls.cn

TS:   if (x == null) {}
来源：http://kr.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://of.huixiangedu.cn

Go:   if x == nil {}
来源：http://on.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ei.wgjwhj.cn

C#:   if (x is null) {}
来源：http://gv.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ua.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bl.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://xd.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wc.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bo.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gp.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jp.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oc.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tv.asd995.cn

[P08] 处理浮点精度问题
来源：http://zd.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ju.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qr.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://st.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lk.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iw.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kh.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lc.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ci.newstarts.cn

================================================================================
来源：http://lt.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ou.huanxung.cn

================================================================================
来源：http://dp.shtwfgs.cn

[Q01] 创建表
来源：http://ee.huixiangedu.cn

CREATE TABLE users (
来源：http://yp.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fr.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://tg.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://zb.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hu.9csxet.cn

);
来源：http://ms.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://vk.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://fo.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://on.nicolike.cn

user_id INT NOT NULL,
来源：http://ve.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://um.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tf.huixiangedu.cn

);
来源：http://ts.huixinmuqiang.cn

[Q03] 增加列
来源：http://uv.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oq.bjjhwx.cn

[Q04] 修改列类型
来源：http://bf.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fs.shtwfgs.cn

[Q05] 重命名列
来源：http://dl.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ai.shxzskj.cn

[Q06] 删除列
来源：http://lp.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gt.shtwfgs.cn

[Q07] 删除表
来源：http://wu.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://pv.szxytkj.cn

[Q08] 创建普通索引
来源：http://ss.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cx.newstarts.cn

[Q09] 创建唯一索引
来源：http://gv.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xh.lnxyls.cn

[Q10] 插入单行
来源：http://dd.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tq.asd995.cn

[Q11] 一次插入多行
来源：http://oh.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uz.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://wz.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sx.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ec.shxzukj.cn

[Q13] 忽略重复插入
来源：http://qq.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ev.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://ln.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rq.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://si.asd995.cn

[Q15] 查询全部
来源：http://vf.asd995.cn

SELECT * FROM users;
来源：http://jl.colortex.cn

[Q16] 查询指定列
来源：http://qy.muxihuayi.cn

SELECT id, name FROM users;
来源：http://lf.huanxung.cn

[Q17] 条件查询
来源：http://po.yuntaijiaju.cn


<!-- 参考信息 -->