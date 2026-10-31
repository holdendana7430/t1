代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vg.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ai.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://um.521024.cn

[M03] 执行外部命令
来源：http://kh.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jh.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tz.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gw.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yo.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pn.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fy.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fi.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://ml.gzmigu.cn

[M04] 获取当前工作目录
来源：http://hm.newstarts.cn

Py:   os.getcwd()
来源：http://ys.chemitech.net.cn

PHP:  getcwd();
来源：http://hu.hnjuh.cn

JS:   process.cwd()
来源：http://fo.bjjhwx.cn

TS:   process.cwd()
来源：http://ce.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://vm.shxzskj.cn

Go:   os.Getwd()
来源：http://fm.haigaiapp.cn

Ruby: Dir.pwd
来源：http://cc.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nt.huixinmuqiang.cn

[M05] 设置退出码
来源：http://qf.shtwfgs.cn

Py:   sys.exit(1)
来源：http://ii.yuntaijiaju.cn

PHP:  exit(1);
来源：http://as.521024.cn

JS:   process.exit(1)
来源：http://nx.9csxet.cn

TS:   process.exit(1)
来源：http://cc.muxihuayi.cn

Java: System.exit(1)
来源：http://fh.wgjwhj.cn

Go:   os.Exit(1)
来源：http://pl.shtwfgs.cn

Ruby: exit 1
来源：http://rf.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hk.huixiangedu.cn

[M06] 向标准错误输出
来源：http://xv.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://dl.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ye.haigaiapp.cn

JS:   console.error("err")
来源：http://vf.szsharing.cn

TS:   console.error("err")
来源：http://pj.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ud.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qw.huanxung.cn

Ruby: warn "err"
来源：http://by.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://km.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://nt.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://ja.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uw.huixinmuqiang.cn

JS:   require.main === module
来源：http://no.panjiajie.cn

TS:   require.main === module
来源：http://le.asd995.cn

Java: public static void main(String[] args)
来源：http://sj.huixiangedu.cn

Go:   func main()
来源：http://pc.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hl.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://kh.521024.cn

[M08] 获取系统与运行时信息
来源：http://hk.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://jx.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://ty.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://jb.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://ix.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sn.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pf.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ag.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://is.nicolike.cn

================================================================================
来源：http://lf.hnjuh.cn

N. 数据结构与算法
来源：http://rx.shxzukj.cn

================================================================================
来源：http://ck.521024.cn

[N01] 二分查找（有序数组）
来源：http://sg.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qs.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pj.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hh.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cc.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nf.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://nj.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nj.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vc.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://sw.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://xs.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ds.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xa.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iq.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dm.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://zg.szsharing.cn

Ruby: arr.sort
来源：http://hc.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lt.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://fp.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ep.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://sv.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qs.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vk.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gn.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ji.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rn.huanxung.cn

[N04] 斐波那契数列
来源：http://tl.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ma.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jo.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zu.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cn.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kb.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ne.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yo.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sx.shxzukj.cn

[N05] 最大公约数
来源：http://cb.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://oy.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://es.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gu.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ce.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rv.asd995.cn

Ruby: a.gcd(b)
来源：http://wa.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ba.nszjky.cn

[N06] 判断回文字符串
来源：http://vj.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://kr.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://ro.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://ek.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://cd.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iw.newstarts.cn

Go:   // 双指针从两端比较
来源：http://cv.yuexingan06.cn

Ruby: s == s.reverse
来源：http://zc.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hj.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://dv.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bc.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://su.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ie.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://jb.huixiangedu.cn

Java: // 手写 HashMap
来源：http://gk.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://hm.newstarts.cn

Ruby: // 手写 Hash
来源：http://bt.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://km.lnxyls.cn

[N08] 生成全排列
来源：http://bc.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://pn.shxzukj.cn

PHP:  // 手写递归交换
来源：http://uv.asd995.cn

JS:   // 手写回溯递归
来源：http://lj.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://jb.colortex.cn

Java: // 手写回溯递归
来源：http://lh.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ku.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://nz.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://lu.jianghongdianzi.cn

[N09] 栈与队列
来源：http://tf.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bu.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ts.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xk.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dk.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://en.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mb.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pb.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://er.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://sq.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tj.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zj.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fe.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eh.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://mo.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dg.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vj.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rf.hahajie.cn

[N11] 二叉树中序遍历
来源：http://si.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gp.szsharing.cn

PHP:  // 手写递归函数
来源：http://ks.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jw.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nv.hnjuh.cn

Java: // 手写递归
来源：http://zl.9csxet.cn

Go:   // 手写递归
来源：http://gn.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://og.jianghongdianzi.cn

C#:   // 手写递归
来源：http://ck.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eo.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ou.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gs.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rg.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yx.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qy.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bk.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fb.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ea.huixinmuqiang.cn

================================================================================
来源：http://yd.yuexingan06.cn

O. 并发与异步
来源：http://mq.shxzskj.cn

================================================================================
来源：http://qc.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://yc.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dz.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ho.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zy.colortex.cn

TS:   // 同 JS
来源：http://lk.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://mv.nicolike.cn

Go:   go f()
来源：http://ca.hahajie.cn

Ruby: Thread.new { f }
来源：http://lt.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ml.521024.cn

[O02] 使用线程池
来源：http://bf.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qd.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sz.nicolike.cn

JS:   // worker_threads 线程池
来源：http://qo.nicolike.cn

TS:   // worker_threads 线程池
来源：http://xj.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vr.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tu.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rt.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ay.newstarts.cn

[O03] 加锁保护共享数据
来源：http://ry.hahajie.cn

Py:   with lock: shared += 1
来源：http://as.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://wg.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mo.colortex.cn

TS:   // 同 JS
来源：http://xk.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://tj.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fx.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vg.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://ar.9csxet.cn

[O04] 定义异步函数并等待
来源：http://dk.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://wv.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xr.newstarts.cn

JS:   async function f() { await g(); }
来源：http://um.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yf.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cs.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hk.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yz.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://bt.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://es.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://mu.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xo.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://db.asd995.cn

TS:   await Promise.all(tasks)
来源：http://tm.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jy.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yz.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://sw.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dh.bjjhwx.cn

[O06] 使用进程池
来源：http://kw.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sd.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tw.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://tx.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://af.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mz.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rs.haigaiapp.cn

Ruby: // fork 块
来源：http://bv.yuexingan06.cn

C#:   Parallel.For
来源：http://lg.521024.cn

================================================================================
来源：http://yx.panjiajie.cn

P. 常用工具函数
来源：http://cs.wgjwhj.cn

================================================================================
来源：http://tm.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://yj.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://pu.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cs.huanxung.cn

JS:   crypto.randomUUID()
来源：http://bd.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://sj.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://bo.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://av.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://ki.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ak.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://jz.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bp.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ng.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://up.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gc.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kr.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vq.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pc.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dk.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://yg.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gf.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://of.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ne.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mm.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vv.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://de.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xl.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xh.wgjwhj.cn

[P04] 求长度
来源：http://rg.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://om.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mb.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pt.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ks.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://zy.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ch.521024.cn

Ruby: x.length;  x.size
来源：http://gs.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ww.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://fy.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uj.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vs.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fm.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nd.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tx.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vi.chemitech.net.cn

Ruby: a == b
来源：http://kx.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://im.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mw.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bc.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://hj.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ec.colortex.cn

TS:   if (x == null) {}
来源：http://xm.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yo.szxytkj.cn

Go:   if x == nil {}
来源：http://mn.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ks.colortex.cn

C#:   if (x is null) {}
来源：http://hu.yuexingan06.cn

[P07] 防抖与节流
来源：http://mw.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fo.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://cq.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ky.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://an.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vw.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://st.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sq.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sp.colortex.cn

[P08] 处理浮点精度问题
来源：http://du.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jz.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uz.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tq.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xy.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://po.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nm.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://th.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ux.gzmigu.cn


<!-- 参考信息 -->