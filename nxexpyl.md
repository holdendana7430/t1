代发 wailian999

Java: public static void main(String[] args)
来源：http://gm.nicolike.cn

Go:   func main()
来源：http://at.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cz.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://zp.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://lp.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://bn.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://bb.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://qh.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://mv.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jw.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zl.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hi.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mc.lnxyls.cn

================================================================================
来源：http://wv.bookmarksfly.cn

N. 数据结构与算法
来源：http://cu.jctech888.com.cn

================================================================================
来源：http://ee.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://kh.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cd.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aw.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rh.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zw.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pz.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ab.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yu.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ph.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://wr.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://he.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cx.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fw.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yr.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nz.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ef.huanxung.cn

Ruby: arr.sort
来源：http://zr.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://io.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://nn.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mq.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://zm.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ar.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mr.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dx.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lz.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vx.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ez.wgjwhj.cn

[N04] 斐波那契数列
来源：http://te.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://om.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://po.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nn.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ur.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gw.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zh.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kc.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rd.szxytkj.cn

[N05] 最大公约数
来源：http://si.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://wx.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lc.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wo.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ok.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ro.521024.cn

Ruby: a.gcd(b)
来源：http://dm.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.huanxung.cn

[N06] 判断回文字符串
来源：http://xm.shtwfgs.cn

Py:   s == s[::-1]
来源：http://zi.asd995.cn

PHP:  $s === strrev($s);
来源：http://xy.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://oa.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://pn.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mk.huanxung.cn

Go:   // 双指针从两端比较
来源：http://xk.huanxung.cn

Ruby: s == s.reverse
来源：http://fc.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zu.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://bj.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eu.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qv.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gf.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://nj.hahajie.cn

Java: // 手写 HashMap
来源：http://yc.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://ee.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://gm.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ej.panjiajie.cn

[N08] 生成全排列
来源：http://iv.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://me.hahajie.cn

PHP:  // 手写递归交换
来源：http://si.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://tn.asd995.cn

TS:   // 手写回溯递归
来源：http://xv.shxzskj.cn

Java: // 手写回溯递归
来源：http://fk.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://so.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://zk.521024.cn

C#:   // 手写回溯递归
来源：http://jo.nszjky.cn

[N09] 栈与队列
来源：http://aq.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uv.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hy.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kj.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ma.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cj.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ad.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xp.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hn.haigaiapp.cn

[N10] 链表节点定义
来源：http://ol.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bc.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://su.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jw.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://im.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://qh.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zj.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hu.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jk.szsharing.cn

[N11] 二叉树中序遍历
来源：http://no.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gt.nszjky.cn

PHP:  // 手写递归函数
来源：http://eu.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lf.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wj.yuntaijiaju.cn

Java: // 手写递归
来源：http://fw.yuntaijiaju.cn

Go:   // 手写递归
来源：http://es.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yo.lnxyls.cn

C#:   // 手写递归
来源：http://ee.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dy.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://we.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qe.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iy.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kn.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://le.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gp.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qn.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ng.colortex.cn

================================================================================
来源：http://vo.lnxyls.cn

O. 并发与异步
来源：http://mh.huixinmuqiang.cn

================================================================================
来源：http://vj.9csxet.cn

[O01] 启动一个线程
来源：http://lf.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kf.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qo.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bh.haigaiapp.cn

TS:   // 同 JS
来源：http://rl.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://ta.nszjky.cn

Go:   go f()
来源：http://gk.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://dk.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://pn.huanxung.cn

[O02] 使用线程池
来源：http://jo.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wx.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://si.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://pv.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://ep.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wg.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ym.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gs.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kh.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://ya.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://nq.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://pd.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fe.jctech888.com.cn

TS:   // 同 JS
来源：http://kg.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://sg.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pz.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iz.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://gp.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://vs.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://cy.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ku.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://kg.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ny.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ht.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ei.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ag.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://oo.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ka.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://tw.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oq.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://fe.asd995.cn

TS:   await Promise.all(tasks)
来源：http://qh.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tb.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ql.newstarts.cn

Ruby: threads.map(&:join)
来源：http://xi.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uc.muxihuayi.cn

[O06] 使用进程池
来源：http://wk.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eq.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wl.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://yt.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://tl.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kj.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://la.gzmigu.cn

Ruby: // fork 块
来源：http://as.wgjwhj.cn

C#:   Parallel.For
来源：http://ie.huixiangedu.cn

================================================================================
来源：http://fu.huixinmuqiang.cn

P. 常用工具函数
来源：http://cm.jianghongdianzi.cn

================================================================================
来源：http://yj.lnxyls.cn

[P01] 生成 UUID
来源：http://il.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://zm.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ef.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://di.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://dl.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://tg.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://eh.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://kc.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://ij.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://br.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://os.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kl.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kl.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xm.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://io.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ff.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tv.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cm.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://lr.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://un.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nu.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ml.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nv.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://en.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wp.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zi.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vy.yuntaijiaju.cn

[P04] 求长度
来源：http://je.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qv.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xb.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cd.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yq.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://tt.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://tu.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://cr.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ox.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ue.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qt.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mb.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kj.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ra.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ky.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nu.lnxyls.cn

Ruby: a == b
来源：http://lo.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wh.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xw.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ln.asd995.cn

PHP:  if (empty($x)) {}
来源：http://jd.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oz.lnxyls.cn

TS:   if (x == null) {}
来源：http://ih.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ed.huanxung.cn

Go:   if x == nil {}
来源：http://bh.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ow.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://td.panjiajie.cn

[P07] 防抖与节流
来源：http://zw.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cs.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ft.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://po.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yq.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vh.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vn.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kt.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zc.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://he.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cv.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vm.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://as.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ex.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qa.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sx.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ba.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hm.hnjuh.cn

================================================================================
来源：http://gk.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zq.szsharing.cn

================================================================================
来源：http://le.shxzukj.cn

[Q01] 创建表
来源：http://he.szsharing.cn

CREATE TABLE users (
来源：http://fw.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zu.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://fs.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://ns.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zj.nszjky.cn

);
来源：http://ls.521024.cn

[Q02] 创建带外键的表
来源：http://pq.szsharing.cn

CREATE TABLE orders (
来源：http://ej.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bt.lnxyls.cn

user_id INT NOT NULL,
来源：http://in.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://lq.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vl.wgjwhj.cn

);
来源：http://la.jianghongdianzi.cn

[Q03] 增加列
来源：http://xi.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vc.9csxet.cn

[Q04] 修改列类型
来源：http://aq.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ts.newstarts.cn

[Q05] 重命名列
来源：http://cj.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dn.shxzukj.cn

[Q06] 删除列
来源：http://ad.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ee.muxihuayi.cn

[Q07] 删除表
来源：http://fc.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://tt.shxzukj.cn

[Q08] 创建普通索引
来源：http://wk.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ci.hahajie.cn

[Q09] 创建唯一索引
来源：http://ar.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pa.hnjuh.cn

[Q10] 插入单行
来源：http://va.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eo.haigaiapp.cn

[Q11] 一次插入多行
来源：http://mx.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ok.521024.cn

[Q12] 插入后取自增 ID
来源：http://ka.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://it.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ck.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://vp.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://if.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://ak.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nr.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ag.huixinmuqiang.cn

[Q15] 查询全部
来源：http://ht.wgjwhj.cn


<!-- 参考信息 -->