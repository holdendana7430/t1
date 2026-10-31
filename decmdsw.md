代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ou.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ic.hnjuh.cn

JS:   require.main === module
来源：http://ol.chemitech.net.cn

TS:   require.main === module
来源：http://rl.nszjky.cn

Java: public static void main(String[] args)
来源：http://xz.huixiangedu.cn

Go:   func main()
来源：http://sr.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lu.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://ss.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://cy.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://in.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://iz.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://xq.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://fj.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fv.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ve.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zx.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://od.huixinmuqiang.cn

================================================================================
来源：http://wq.gzmigu.cn

N. 数据结构与算法
来源：http://oc.panjiajie.cn

================================================================================
来源：http://dp.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://at.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://za.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pj.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xi.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wm.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sa.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ch.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ep.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kg.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://lu.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://er.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yu.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dw.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oo.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qa.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://nl.chemitech.net.cn

Ruby: arr.sort
来源：http://si.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uy.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://pz.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://av.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://xr.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yc.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yr.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nw.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cp.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vc.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://or.haigaiapp.cn

[N04] 斐波那契数列
来源：http://br.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dc.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wd.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://an.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kz.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gf.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pb.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pd.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qr.panjiajie.cn

[N05] 最大公约数
来源：http://he.szsharing.cn

Py:   math.gcd(a, b)
来源：http://gy.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ei.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pl.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ck.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nz.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ek.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://jr.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fd.colortex.cn

[N06] 判断回文字符串
来源：http://wx.muxihuayi.cn

Py:   s == s[::-1]
来源：http://nj.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://pn.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://mj.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://zn.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gn.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://bf.521024.cn

Ruby: s == s.reverse
来源：http://ip.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kc.521024.cn

[N07] 两数之和（返回下标）
来源：http://ic.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://db.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jt.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sy.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://ei.panjiajie.cn

Java: // 手写 HashMap
来源：http://sq.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://pk.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://vm.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ho.huixiangedu.cn

[N08] 生成全排列
来源：http://wv.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://zy.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ic.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://hg.shxzskj.cn

TS:   // 手写回溯递归
来源：http://rk.colortex.cn

Java: // 手写回溯递归
来源：http://eg.hnjuh.cn

Go:   // 手写回溯递归
来源：http://io.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://tq.panjiajie.cn

C#:   // 手写回溯递归
来源：http://me.shtwfgs.cn

[N09] 栈与队列
来源：http://xi.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kg.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oe.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yu.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pr.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://os.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jt.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pw.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oi.shxzskj.cn

[N10] 链表节点定义
来源：http://kd.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jh.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jh.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://of.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qs.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://la.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hj.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qb.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lc.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://cn.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fa.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://gq.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hr.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gw.yuntaijiaju.cn

Java: // 手写递归
来源：http://kp.9csxet.cn

Go:   // 手写递归
来源：http://pw.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eg.colortex.cn

C#:   // 手写递归
来源：http://ir.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pu.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zy.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zf.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zz.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jc.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yw.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vn.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fq.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vf.colortex.cn

================================================================================
来源：http://ev.shtwfgs.cn

O. 并发与异步
来源：http://jz.hahajie.cn

================================================================================
来源：http://yc.9csxet.cn

[O01] 启动一个线程
来源：http://ax.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lt.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hc.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mg.huixinmuqiang.cn

TS:   // 同 JS
来源：http://oq.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://vs.hnjuh.cn

Go:   go f()
来源：http://sr.newstarts.cn

Ruby: Thread.new { f }
来源：http://wb.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://eh.lnxyls.cn

[O02] 使用线程池
来源：http://ze.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gc.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rc.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://kk.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://at.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zu.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hi.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ma.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vi.newstarts.cn

[O03] 加锁保护共享数据
来源：http://eb.asd995.cn

Py:   with lock: shared += 1
来源：http://rz.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://fv.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lf.jctech888.com.cn

TS:   // 同 JS
来源：http://vp.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://xm.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xo.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qj.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://tz.newstarts.cn

[O04] 定义异步函数并等待
来源：http://lp.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://ov.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fy.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://it.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ws.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ee.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wq.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rw.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://hl.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://ff.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://eo.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qo.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://xx.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://wc.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lu.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sq.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://vw.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ma.hnjuh.cn

[O06] 使用进程池
来源：http://fl.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://no.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://he.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://kp.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://ob.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lp.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ke.9csxet.cn

Ruby: // fork 块
来源：http://fi.muxihuayi.cn

C#:   Parallel.For
来源：http://eo.hahajie.cn

================================================================================
来源：http://ao.asd995.cn

P. 常用工具函数
来源：http://zz.yuntaijiaju.cn

================================================================================
来源：http://lx.szsharing.cn

[P01] 生成 UUID
来源：http://zs.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://fd.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ji.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://kb.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://py.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://wc.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://wb.asd995.cn

Ruby: SecureRandom.uuid
来源：http://uk.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://oq.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://hh.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pu.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ka.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qw.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sl.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dd.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ym.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ua.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fk.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://he.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vz.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tl.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lo.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rr.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qp.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://od.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zp.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xq.szxytkj.cn

[P04] 求长度
来源：http://vc.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ao.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dz.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://if.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dh.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://ke.colortex.cn

Go:   len(arr);  len(m)
来源：http://yo.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://hf.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vu.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://mk.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ho.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oh.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rl.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jj.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mb.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uw.shxzskj.cn

Ruby: a == b
来源：http://wc.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pz.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ia.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oo.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://ji.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yz.jctech888.com.cn

TS:   if (x == null) {}
来源：http://or.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ed.shxzskj.cn

Go:   if x == nil {}
来源：http://jp.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pt.shtwfgs.cn

C#:   if (x is null) {}
来源：http://mv.muxihuayi.cn

[P07] 防抖与节流
来源：http://mg.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pe.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ru.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mx.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zh.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ap.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wm.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ei.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://af.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sm.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rv.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lt.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kf.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://af.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ct.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://il.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ty.szsharing.cn

================================================================================
来源：http://cr.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dr.9csxet.cn

================================================================================
来源：http://ce.szxytkj.cn

[Q01] 创建表
来源：http://ov.muxihuayi.cn

CREATE TABLE users (
来源：http://hv.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ii.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://tn.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://xy.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ec.bjjhwx.cn

);
来源：http://mz.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://cn.nszjky.cn

CREATE TABLE orders (
来源：http://og.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ex.chemitech.net.cn

user_id INT NOT NULL,
来源：http://qp.hahajie.cn

amount DECIMAL(10, 2),
来源：http://fb.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rh.nszjky.cn

);
来源：http://nf.szxytkj.cn

[Q03] 增加列
来源：http://pe.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://la.newstarts.cn

[Q04] 修改列类型
来源：http://br.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ch.muxihuayi.cn

[Q05] 重命名列
来源：http://me.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yj.colortex.cn

[Q06] 删除列
来源：http://nz.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nw.huixiangedu.cn

[Q07] 删除表
来源：http://vk.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://or.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://ct.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pu.panjiajie.cn

[Q09] 创建唯一索引
来源：http://vg.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ja.bjjhwx.cn

[Q10] 插入单行
来源：http://mh.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nq.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://cf.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ju.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://nn.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jo.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rf.9csxet.cn

[Q13] 忽略重复插入
来源：http://pm.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nm.wgjwhj.cn


<!-- 参考信息 -->