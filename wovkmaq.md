代发 wailian999

[M04] 获取当前工作目录
来源：http://pf.nszjky.cn

Py:   os.getcwd()
来源：http://zl.9csxet.cn

PHP:  getcwd();
来源：http://pt.bookmarksfly.cn

JS:   process.cwd()
来源：http://cc.bjjhwx.cn

TS:   process.cwd()
来源：http://jl.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://tg.huixiangedu.cn

Go:   os.Getwd()
来源：http://tp.haigaiapp.cn

Ruby: Dir.pwd
来源：http://tt.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jz.9csxet.cn

[M05] 设置退出码
来源：http://vd.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://xq.yuexingan06.cn

PHP:  exit(1);
来源：http://kp.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://ht.szsharing.cn

TS:   process.exit(1)
来源：http://eq.hahajie.cn

Java: System.exit(1)
来源：http://wr.newstarts.cn

Go:   os.Exit(1)
来源：http://fa.gzmigu.cn

Ruby: exit 1
来源：http://sp.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eh.521024.cn

[M06] 向标准错误输出
来源：http://vp.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://la.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fu.jianghongdianzi.cn

JS:   console.error("err")
来源：http://hk.szsharing.cn

TS:   console.error("err")
来源：http://zj.chemitech.net.cn

Java: System.err.println("err")
来源：http://xr.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hx.szxytkj.cn

Ruby: warn "err"
来源：http://yq.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://cq.hahajie.cn

[M07] 判断是否为主入口
来源：http://ci.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://wb.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bp.huanxung.cn

JS:   require.main === module
来源：http://gg.wgjwhj.cn

TS:   require.main === module
来源：http://uq.lnxyls.cn

Java: public static void main(String[] args)
来源：http://fw.lnxyls.cn

Go:   func main()
来源：http://vk.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gr.newstarts.cn

C#:   static void Main(string[] args)
来源：http://zo.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://nx.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://ie.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://zo.hnjuh.cn

JS:   process.platform;  process.version
来源：http://kw.521024.cn

TS:   process.platform;  process.version
来源：http://pt.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qx.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bu.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://op.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zh.jianghongdianzi.cn

================================================================================
来源：http://ee.bookmarksfly.cn

N. 数据结构与算法
来源：http://pa.jianghongdianzi.cn

================================================================================
来源：http://dx.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://ng.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eb.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://db.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cr.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://af.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fc.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://wg.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://em.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uu.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zu.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://tb.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ky.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ap.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pv.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vs.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://ne.bookmarksfly.cn

Ruby: arr.sort
来源：http://yj.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eu.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://sy.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ct.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://da.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hs.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ze.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gr.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xp.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hj.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dl.szsharing.cn

[N04] 斐波那契数列
来源：http://kf.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://na.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mo.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bu.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ad.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qr.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sl.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eo.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://en.szxytkj.cn

[N05] 最大公约数
来源：http://jo.hahajie.cn

Py:   math.gcd(a, b)
来源：http://ho.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cc.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gx.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ve.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ri.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rl.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://fb.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://re.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://rl.lnxyls.cn

Py:   s == s[::-1]
来源：http://ae.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://gk.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://ij.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://cs.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rk.521024.cn

Go:   // 双指针从两端比较
来源：http://pr.nicolike.cn

Ruby: s == s.reverse
来源：http://bt.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wy.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://ej.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sm.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gc.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hq.521024.cn

TS:   // 手写 Map<string, number>
来源：http://zo.chemitech.net.cn

Java: // 手写 HashMap
来源：http://xq.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://tq.gzmigu.cn

Ruby: // 手写 Hash
来源：http://uh.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vs.chemitech.net.cn

[N08] 生成全排列
来源：http://tr.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://vn.shxzukj.cn

PHP:  // 手写递归交换
来源：http://br.panjiajie.cn

JS:   // 手写回溯递归
来源：http://aw.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://ki.hahajie.cn

Java: // 手写回溯递归
来源：http://bu.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://ej.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://xi.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://gd.yuexingan06.cn

[N09] 栈与队列
来源：http://tl.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wr.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fj.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fi.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oa.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ep.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eh.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sh.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cn.shxzukj.cn

[N10] 链表节点定义
来源：http://od.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kf.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dk.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hg.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ew.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://es.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ns.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://on.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eb.huanxung.cn

[N11] 二叉树中序遍历
来源：http://uh.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://py.panjiajie.cn

PHP:  // 手写递归函数
来源：http://sl.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vv.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gt.huanxung.cn

Java: // 手写递归
来源：http://xl.chemitech.net.cn

Go:   // 手写递归
来源：http://zj.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kj.colortex.cn

C#:   // 手写递归
来源：http://jg.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fd.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iu.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ix.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zs.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xz.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nb.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sb.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ee.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vh.shxzukj.cn

================================================================================
来源：http://tt.yuntaijiaju.cn

O. 并发与异步
来源：http://zp.colortex.cn

================================================================================
来源：http://ll.yuexingan06.cn

[O01] 启动一个线程
来源：http://sv.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fs.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kf.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ul.wgjwhj.cn

TS:   // 同 JS
来源：http://fa.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://qi.jctech888.com.cn

Go:   go f()
来源：http://tp.newstarts.cn

Ruby: Thread.new { f }
来源：http://el.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://sm.yuntaijiaju.cn

[O02] 使用线程池
来源：http://vn.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bk.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qh.szsharing.cn

JS:   // worker_threads 线程池
来源：http://db.newstarts.cn

TS:   // worker_threads 线程池
来源：http://de.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://un.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://di.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rx.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lh.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://nj.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://sj.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://zy.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ua.nszjky.cn

TS:   // 同 JS
来源：http://fn.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://ux.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sm.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ru.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://gu.hahajie.cn

[O04] 定义异步函数并等待
来源：http://my.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://yb.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://et.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://rc.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lm.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pd.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rt.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://en.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://az.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://yo.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ja.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sm.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://mo.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://bz.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nr.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fn.huanxung.cn

Ruby: threads.map(&:join)
来源：http://zw.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://js.gzmigu.cn

[O06] 使用进程池
来源：http://sz.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lf.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://di.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://nl.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ct.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bi.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zn.yuntaijiaju.cn

Ruby: // fork 块
来源：http://eo.hnjuh.cn

C#:   Parallel.For
来源：http://so.gzmigu.cn

================================================================================
来源：http://og.panjiajie.cn

P. 常用工具函数
来源：http://xu.chemitech.net.cn

================================================================================
来源：http://ss.hahajie.cn

[P01] 生成 UUID
来源：http://ix.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://fh.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jz.colortex.cn

JS:   crypto.randomUUID()
来源：http://xt.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://ky.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://bv.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://ih.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://zq.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://cr.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ak.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zh.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qr.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://si.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qz.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vx.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pp.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bx.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ca.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://tl.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nb.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qf.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yr.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://om.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ea.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://it.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ga.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cm.yuexingan06.cn

[P04] 求长度
来源：http://be.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://op.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dt.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lr.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ij.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ff.colortex.cn

Go:   len(arr);  len(m)
来源：http://ys.9csxet.cn

Ruby: x.length;  x.size
来源：http://du.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://al.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://uk.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vn.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hr.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cb.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ed.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gt.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://la.yuexingan06.cn

Ruby: a == b
来源：http://hd.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mc.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vr.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xa.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://os.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sg.521024.cn

TS:   if (x == null) {}
来源：http://vv.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://io.nszjky.cn

Go:   if x == nil {}
来源：http://kc.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ma.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://jr.521024.cn

[P07] 防抖与节流
来源：http://jk.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dz.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://cb.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ts.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ad.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gs.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ez.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vr.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bk.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://he.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://is.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jd.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eu.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nj.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ze.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bw.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uv.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qo.chemitech.net.cn

================================================================================
来源：http://sd.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pw.521024.cn

================================================================================
来源：http://ie.wgjwhj.cn

[Q01] 创建表
来源：http://oz.yuexingan06.cn

CREATE TABLE users (
来源：http://jf.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ad.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://zv.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://yo.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://km.wgjwhj.cn

);
来源：http://ut.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://vr.shxzukj.cn

CREATE TABLE orders (
来源：http://ob.bjjhwx.cn


<!-- 参考信息 -->