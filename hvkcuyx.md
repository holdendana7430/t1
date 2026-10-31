代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xa.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ui.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dx.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://mq.gzmigu.cn

[M04] 获取当前工作目录
来源：http://oo.hnjuh.cn

Py:   os.getcwd()
来源：http://yl.bookmarksfly.cn

PHP:  getcwd();
来源：http://bc.bookmarksfly.cn

JS:   process.cwd()
来源：http://ds.szxytkj.cn

TS:   process.cwd()
来源：http://bb.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://mz.nicolike.cn

Go:   os.Getwd()
来源：http://mb.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ms.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qm.huanxung.cn

[M05] 设置退出码
来源：http://mx.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://qs.bjjhwx.cn

PHP:  exit(1);
来源：http://az.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ek.szxytkj.cn

TS:   process.exit(1)
来源：http://qf.shxzukj.cn

Java: System.exit(1)
来源：http://mr.wgjwhj.cn

Go:   os.Exit(1)
来源：http://ah.huanxung.cn

Ruby: exit 1
来源：http://tu.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uz.chemitech.net.cn

[M06] 向标准错误输出
来源：http://vq.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://fp.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://td.chemitech.net.cn

JS:   console.error("err")
来源：http://mq.chemitech.net.cn

TS:   console.error("err")
来源：http://hb.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://bd.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ek.szsharing.cn

Ruby: warn "err"
来源：http://oi.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://wo.asd995.cn

[M07] 判断是否为主入口
来源：http://xf.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://sw.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ev.colortex.cn

JS:   require.main === module
来源：http://ba.huixiangedu.cn

TS:   require.main === module
来源：http://lz.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://ff.asd995.cn

Go:   func main()
来源：http://oj.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pf.nszjky.cn

C#:   static void Main(string[] args)
来源：http://dm.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://vo.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://kl.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://bb.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://kw.asd995.cn

TS:   process.platform;  process.version
来源：http://pi.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://le.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rf.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fe.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fl.jianghongdianzi.cn

================================================================================
来源：http://vm.wgjwhj.cn

N. 数据结构与算法
来源：http://hn.9csxet.cn

================================================================================
来源：http://wd.asd995.cn

[N01] 二分查找（有序数组）
来源：http://ai.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sh.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kt.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rh.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qm.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jz.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://oc.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fc.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://za.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://zs.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://qx.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://at.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://le.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qq.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kn.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://po.szxytkj.cn

Ruby: arr.sort
来源：http://mv.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xr.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://uw.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tt.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://qg.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eq.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ag.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pz.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zh.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://an.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rh.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://dg.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xo.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oz.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tq.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mm.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uk.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fh.asd995.cn

[N05] 最大公约数
来源：http://ml.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://fs.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pa.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ls.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uq.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lr.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fw.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://pv.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ym.asd995.cn

[N06] 判断回文字符串
来源：http://ra.521024.cn

Py:   s == s[::-1]
来源：http://cu.asd995.cn

PHP:  $s === strrev($s);
来源：http://fg.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://mc.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://tr.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kn.521024.cn

Go:   // 双指针从两端比较
来源：http://mi.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ps.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jk.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://ql.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://of.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eq.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ph.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ec.chemitech.net.cn

Java: // 手写 HashMap
来源：http://at.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://bw.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://jz.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yt.panjiajie.cn

[N08] 生成全排列
来源：http://tp.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://zi.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ym.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ye.asd995.cn

TS:   // 手写回溯递归
来源：http://sx.muxihuayi.cn

Java: // 手写回溯递归
来源：http://wn.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://hk.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://fh.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ur.huanxung.cn

[N09] 栈与队列
来源：http://tq.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cc.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lw.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pi.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hc.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jj.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qd.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ij.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cv.bjjhwx.cn

[N10] 链表节点定义
来源：http://wk.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hp.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tw.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ty.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jn.asd995.cn

Java: class Node { int v; Node next; }
来源：http://gh.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://at.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cd.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lt.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://pu.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lg.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://vl.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://im.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dz.colortex.cn

Java: // 手写递归
来源：http://ck.huixiangedu.cn

Go:   // 手写递归
来源：http://zh.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jy.colortex.cn

C#:   // 手写递归
来源：http://yc.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ac.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kz.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ue.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://in.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rr.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://it.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uc.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bo.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hl.colortex.cn

================================================================================
来源：http://uo.muxihuayi.cn

O. 并发与异步
来源：http://ku.yuexingan06.cn

================================================================================
来源：http://iz.bjjhwx.cn

[O01] 启动一个线程
来源：http://fn.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wu.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://br.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sa.9csxet.cn

TS:   // 同 JS
来源：http://si.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://bv.huixiangedu.cn

Go:   go f()
来源：http://tu.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://hi.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://hf.szxytkj.cn

[O02] 使用线程池
来源：http://vg.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zv.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cg.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://em.huanxung.cn

TS:   // worker_threads 线程池
来源：http://yv.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ys.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gt.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cu.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tn.nszjky.cn

[O03] 加锁保护共享数据
来源：http://tb.colortex.cn

Py:   with lock: shared += 1
来源：http://qz.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://nx.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sc.muxihuayi.cn

TS:   // 同 JS
来源：http://uv.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://ag.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ql.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gi.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://al.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://xs.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://kv.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uf.nszjky.cn

JS:   async function f() { await g(); }
来源：http://cs.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tp.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kq.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ea.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vc.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://ks.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://ax.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://lx.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://do.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://hr.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://aj.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ns.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ic.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://cc.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cb.9csxet.cn

[O06] 使用进程池
来源：http://lu.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kw.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kw.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://ip.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://rg.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fk.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ul.newstarts.cn

Ruby: // fork 块
来源：http://um.shxzukj.cn

C#:   Parallel.For
来源：http://ba.jctech888.com.cn

================================================================================
来源：http://aj.szxytkj.cn

P. 常用工具函数
来源：http://uu.hahajie.cn

================================================================================
来源：http://eq.nszjky.cn

[P01] 生成 UUID
来源：http://ff.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://js.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ya.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://im.szsharing.cn

TS:   crypto.randomUUID()
来源：http://fz.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://xd.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://bw.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://ac.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://nm.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://wn.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gf.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wp.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hu.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dp.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gl.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cl.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ua.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ky.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://ya.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lj.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lz.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xr.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://my.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vv.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ek.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hk.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zi.jctech888.com.cn

[P04] 求长度
来源：http://jr.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vx.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://op.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xd.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nt.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://ai.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://no.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ze.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://il.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ws.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jo.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fq.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nv.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bc.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ym.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uq.nszjky.cn

Ruby: a == b
来源：http://tx.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bf.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pz.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ud.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://hr.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://md.shtwfgs.cn

TS:   if (x == null) {}
来源：http://jt.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://df.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://le.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oj.muxihuayi.cn

C#:   if (x is null) {}
来源：http://xc.9csxet.cn

[P07] 防抖与节流
来源：http://xw.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ch.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://bp.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fi.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kn.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mw.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dk.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://go.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uu.newstarts.cn

[P08] 处理浮点精度问题
来源：http://xy.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gp.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ag.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uz.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oi.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tn.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bq.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://of.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rb.haigaiapp.cn

================================================================================
来源：http://sa.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uz.hahajie.cn

================================================================================
来源：http://wg.newstarts.cn

[Q01] 创建表
来源：http://ax.szsharing.cn

CREATE TABLE users (
来源：http://gk.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wx.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://xh.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://wh.hahajie.cn


<!-- 参考信息 -->