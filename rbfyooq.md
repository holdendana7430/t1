代发 wailian999

Java: public static void main(String[] args)
来源：http://hk.huixiangedu.cn

Go:   func main()
来源：http://ij.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fj.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://ed.colortex.cn

[M08] 获取系统与运行时信息
来源：http://sa.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://qq.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://im.szsharing.cn

JS:   process.platform;  process.version
来源：http://ku.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ko.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lh.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xx.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ao.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vx.szsharing.cn

================================================================================
来源：http://rt.shxzskj.cn

N. 数据结构与算法
来源：http://wl.gzmigu.cn

================================================================================
来源：http://yo.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://uf.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yy.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nk.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nf.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://as.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gi.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://es.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ic.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rc.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://nc.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ct.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gg.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://si.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ae.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xx.huanxung.cn

Go:   slices.Sort(arr)
来源：http://rj.521024.cn

Ruby: arr.sort
来源：http://zt.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vo.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://zp.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mm.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://hi.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nz.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qa.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jl.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://km.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xc.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dr.jctech888.com.cn

[N04] 斐波那契数列
来源：http://tf.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ib.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ah.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bt.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qk.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pq.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tg.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qr.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rf.bjjhwx.cn

[N05] 最大公约数
来源：http://fs.colortex.cn

Py:   math.gcd(a, b)
来源：http://xp.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nn.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fx.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hv.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vq.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zz.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://hf.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hc.panjiajie.cn

[N06] 判断回文字符串
来源：http://pm.shxzskj.cn

Py:   s == s[::-1]
来源：http://cj.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://dc.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://yv.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://hk.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ze.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://nk.shxzskj.cn

Ruby: s == s.reverse
来源：http://sz.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lt.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://cn.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://og.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mz.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vm.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://lz.wgjwhj.cn

Java: // 手写 HashMap
来源：http://fz.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://on.newstarts.cn

Ruby: // 手写 Hash
来源：http://xk.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qb.muxihuayi.cn

[N08] 生成全排列
来源：http://ks.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://uq.panjiajie.cn

PHP:  // 手写递归交换
来源：http://xc.9csxet.cn

JS:   // 手写回溯递归
来源：http://nj.huanxung.cn

TS:   // 手写回溯递归
来源：http://ka.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ii.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://lv.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://sb.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ei.chemitech.net.cn

[N09] 栈与队列
来源：http://pz.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tx.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zw.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cn.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ke.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wl.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mr.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yo.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lj.bjjhwx.cn

[N10] 链表节点定义
来源：http://nl.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ff.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sc.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vl.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nv.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://kx.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mk.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fk.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lr.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://we.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uq.hnjuh.cn

PHP:  // 手写递归函数
来源：http://vb.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dk.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dn.hahajie.cn

Java: // 手写递归
来源：http://yd.hnjuh.cn

Go:   // 手写递归
来源：http://ax.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oo.nicolike.cn

C#:   // 手写递归
来源：http://qd.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hq.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uu.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mk.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ai.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oy.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pl.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hl.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qp.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sj.bookmarksfly.cn

================================================================================
来源：http://rv.newstarts.cn

O. 并发与异步
来源：http://kw.hnjuh.cn

================================================================================
来源：http://wg.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://kx.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kl.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ms.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aq.shxzskj.cn

TS:   // 同 JS
来源：http://go.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://ft.szsharing.cn

Go:   go f()
来源：http://mw.shxzskj.cn

Ruby: Thread.new { f }
来源：http://xe.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://tu.lnxyls.cn

[O02] 使用线程池
来源：http://im.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ym.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vc.521024.cn

JS:   // worker_threads 线程池
来源：http://iz.nszjky.cn

TS:   // worker_threads 线程池
来源：http://hx.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mq.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eg.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rt.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tz.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://qf.shxzskj.cn

Py:   with lock: shared += 1
来源：http://fx.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ib.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ac.jctech888.com.cn

TS:   // 同 JS
来源：http://ba.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://ky.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oo.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lf.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://sm.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://sh.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://oj.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hd.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://xg.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vx.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://le.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://on.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tf.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://um.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://yh.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://nz.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://em.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://cy.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://kt.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hh.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ye.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ch.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pu.asd995.cn

[O06] 使用进程池
来源：http://so.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nm.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eg.asd995.cn

JS:   // child_process / cluster 模块
来源：http://us.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://ss.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gt.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://po.szsharing.cn

Ruby: // fork 块
来源：http://ed.szsharing.cn

C#:   Parallel.For
来源：http://fq.lnxyls.cn

================================================================================
来源：http://go.colortex.cn

P. 常用工具函数
来源：http://cx.chemitech.net.cn

================================================================================
来源：http://jm.asd995.cn

[P01] 生成 UUID
来源：http://oc.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://br.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aa.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://it.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://ty.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://yk.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ib.521024.cn

Ruby: SecureRandom.uuid
来源：http://ji.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://sb.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ig.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lh.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ho.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qz.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ml.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bn.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pq.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nw.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bj.shxzskj.cn

[P03] 生成短随机字符串
来源：http://rk.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pc.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yr.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ze.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ak.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://my.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rd.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zx.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ae.yuntaijiaju.cn

[P04] 求长度
来源：http://vj.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oz.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ge.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ck.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kz.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://hy.nicolike.cn

Go:   len(arr);  len(m)
来源：http://pq.shxzukj.cn

Ruby: x.length;  x.size
来源：http://bt.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jp.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://fp.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ud.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ey.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://os.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cf.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rq.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jk.yuntaijiaju.cn

Ruby: a == b
来源：http://ba.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ay.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gc.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hw.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://rs.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cx.newstarts.cn

TS:   if (x == null) {}
来源：http://rt.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lh.bjjhwx.cn

Go:   if x == nil {}
来源：http://ck.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ww.yuexingan06.cn

C#:   if (x is null) {}
来源：http://nr.nicolike.cn

[P07] 防抖与节流
来源：http://uf.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zh.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://fs.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vo.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jg.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rt.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sf.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://so.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://so.asd995.cn

[P08] 处理浮点精度问题
来源：http://px.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://se.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lh.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pv.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uq.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wv.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oc.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wj.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dr.lnxyls.cn

================================================================================
来源：http://wd.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wc.panjiajie.cn

================================================================================
来源：http://ga.newstarts.cn

[Q01] 创建表
来源：http://ve.panjiajie.cn

CREATE TABLE users (
来源：http://fa.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hh.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://ao.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://vh.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ey.bookmarksfly.cn

);
来源：http://tn.shxzukj.cn

[Q02] 创建带外键的表
来源：http://pb.yuexingan06.cn

CREATE TABLE orders (
来源：http://ly.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gz.muxihuayi.cn

user_id INT NOT NULL,
来源：http://hb.9csxet.cn

amount DECIMAL(10, 2),
来源：http://mk.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oe.muxihuayi.cn

);
来源：http://fn.huixinmuqiang.cn

[Q03] 增加列
来源：http://pk.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vp.wgjwhj.cn

[Q04] 修改列类型
来源：http://re.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lc.hnjuh.cn

[Q05] 重命名列
来源：http://db.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dy.shxzskj.cn

[Q06] 删除列
来源：http://zk.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://od.yuexingan06.cn

[Q07] 删除表
来源：http://la.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ct.asd995.cn

[Q08] 创建普通索引
来源：http://iu.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://an.shxzukj.cn

[Q09] 创建唯一索引
来源：http://fy.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fa.lnxyls.cn

[Q10] 插入单行
来源：http://ha.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bu.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://cm.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://te.asd995.cn

[Q12] 插入后取自增 ID
来源：http://kv.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wq.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yr.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://uj.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qa.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://ei.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xx.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://af.yuexingan06.cn

[Q15] 查询全部
来源：http://mb.shxzskj.cn


<!-- 参考信息 -->