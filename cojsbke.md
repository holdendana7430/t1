代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tb.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wv.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ht.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hd.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tb.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kj.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mr.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://of.asd995.cn

[M04] 获取当前工作目录
来源：http://pu.huanxung.cn

Py:   os.getcwd()
来源：http://en.muxihuayi.cn

PHP:  getcwd();
来源：http://il.bookmarksfly.cn

JS:   process.cwd()
来源：http://ni.szxytkj.cn

TS:   process.cwd()
来源：http://zb.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ld.asd995.cn

Go:   os.Getwd()
来源：http://oc.colortex.cn

Ruby: Dir.pwd
来源：http://lp.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dc.szxytkj.cn

[M05] 设置退出码
来源：http://ev.521024.cn

Py:   sys.exit(1)
来源：http://yg.jianghongdianzi.cn

PHP:  exit(1);
来源：http://iq.nicolike.cn

JS:   process.exit(1)
来源：http://rn.shtwfgs.cn

TS:   process.exit(1)
来源：http://sp.colortex.cn

Java: System.exit(1)
来源：http://er.asd995.cn

Go:   os.Exit(1)
来源：http://zd.newstarts.cn

Ruby: exit 1
来源：http://gk.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fp.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://us.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://du.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uj.shtwfgs.cn

JS:   console.error("err")
来源：http://nb.wgjwhj.cn

TS:   console.error("err")
来源：http://dg.shxzukj.cn

Java: System.err.println("err")
来源：http://zv.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pw.shxzskj.cn

Ruby: warn "err"
来源：http://dm.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://gg.9csxet.cn

[M07] 判断是否为主入口
来源：http://od.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://ff.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wz.jctech888.com.cn

JS:   require.main === module
来源：http://uo.panjiajie.cn

TS:   require.main === module
来源：http://et.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://dv.jctech888.com.cn

Go:   func main()
来源：http://tv.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bo.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://bt.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://mw.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://yn.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://eq.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://lk.shxzukj.cn

TS:   process.platform;  process.version
来源：http://lr.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nw.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nn.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kf.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pu.shtwfgs.cn

================================================================================
来源：http://jl.muxihuayi.cn

N. 数据结构与算法
来源：http://if.muxihuayi.cn

================================================================================
来源：http://dj.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://ff.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dc.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://td.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mc.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gh.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wr.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://bb.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vr.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ts.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://rt.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://db.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xm.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wg.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://du.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nh.hahajie.cn

Go:   slices.Sort(arr)
来源：http://sf.hnjuh.cn

Ruby: arr.sort
来源：http://ra.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cb.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://kj.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://pb.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vu.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pz.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rj.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ae.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://th.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rt.nicolike.cn

[N04] 斐波那契数列
来源：http://mz.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dg.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ac.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fd.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oo.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ei.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ym.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dc.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ia.asd995.cn

[N05] 最大公约数
来源：http://jx.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://cg.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cx.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pi.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vh.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xa.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wx.colortex.cn

Ruby: a.gcd(b)
来源：http://rm.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ib.bjjhwx.cn

[N06] 判断回文字符串
来源：http://vo.chemitech.net.cn

Py:   s == s[::-1]
来源：http://am.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://vl.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://wa.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://px.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mp.colortex.cn

Go:   // 双指针从两端比较
来源：http://gv.nszjky.cn

Ruby: s == s.reverse
来源：http://oa.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oj.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://aq.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zo.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vz.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zj.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://db.nszjky.cn

Java: // 手写 HashMap
来源：http://rm.newstarts.cn

Go:   // 手写 map[int]int
来源：http://sv.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://cv.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hk.huixinmuqiang.cn

[N08] 生成全排列
来源：http://oe.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://sc.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://ki.lnxyls.cn

JS:   // 手写回溯递归
来源：http://vq.9csxet.cn

TS:   // 手写回溯递归
来源：http://pz.hahajie.cn

Java: // 手写回溯递归
来源：http://ko.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ue.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://zo.szxytkj.cn

C#:   // 手写回溯递归
来源：http://za.shxzukj.cn

[N09] 栈与队列
来源：http://lt.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mj.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yb.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aq.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uc.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://he.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ok.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fy.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xl.gzmigu.cn

[N10] 链表节点定义
来源：http://ca.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://on.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pp.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fh.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mx.521024.cn

Java: class Node { int v; Node next; }
来源：http://dn.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ti.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ub.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ee.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://qu.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rp.panjiajie.cn

PHP:  // 手写递归函数
来源：http://sr.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oa.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vm.shxzskj.cn

Java: // 手写递归
来源：http://pm.shxzukj.cn

Go:   // 手写递归
来源：http://dw.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zw.bookmarksfly.cn

C#:   // 手写递归
来源：http://od.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ka.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://en.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vv.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ce.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gx.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ty.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hl.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jy.hnjuh.cn

================================================================================
来源：http://gj.jianghongdianzi.cn

O. 并发与异步
来源：http://gx.szxytkj.cn

================================================================================
来源：http://zk.nicolike.cn

[O01] 启动一个线程
来源：http://ni.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ws.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nk.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mn.9csxet.cn

TS:   // 同 JS
来源：http://va.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://lh.521024.cn

Go:   go f()
来源：http://re.shxzskj.cn

Ruby: Thread.new { f }
来源：http://wl.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://vb.wgjwhj.cn

[O02] 使用线程池
来源：http://uo.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jy.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eu.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://go.521024.cn

TS:   // worker_threads 线程池
来源：http://ek.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uh.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jg.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qr.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uf.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ip.nszjky.cn

Py:   with lock: shared += 1
来源：http://vk.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://ct.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://do.9csxet.cn

TS:   // 同 JS
来源：http://fg.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://vl.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dc.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ec.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://ec.colortex.cn

[O04] 定义异步函数并等待
来源：http://oy.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://oi.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mf.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ek.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jn.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vr.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kl.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vu.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://gr.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://dk.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://gg.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://he.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://so.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://jj.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jk.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ns.szsharing.cn

Ruby: threads.map(&:join)
来源：http://my.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cv.muxihuayi.cn

[O06] 使用进程池
来源：http://bj.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rx.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://am.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://lw.521024.cn

TS:   // child_process / cluster 模块
来源：http://nd.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oq.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wi.asd995.cn

Ruby: // fork 块
来源：http://qg.jctech888.com.cn

C#:   Parallel.For
来源：http://wj.bjjhwx.cn

================================================================================
来源：http://mc.chemitech.net.cn

P. 常用工具函数
来源：http://od.yuntaijiaju.cn

================================================================================
来源：http://dp.bookmarksfly.cn

[P01] 生成 UUID
来源：http://ji.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://fe.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yn.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://dk.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://ue.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://my.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://xt.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://xy.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://yf.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://oe.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yo.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bs.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rs.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ak.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nk.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lm.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eh.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://un.asd995.cn

[P03] 生成短随机字符串
来源：http://ef.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yi.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ol.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xw.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ch.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zk.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tj.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xj.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cn.nszjky.cn

[P04] 求长度
来源：http://yc.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cx.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ls.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jj.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mu.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://xt.nicolike.cn

Go:   len(arr);  len(m)
来源：http://iv.colortex.cn

Ruby: x.length;  x.size
来源：http://yd.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oy.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://yd.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qh.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nj.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aq.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oq.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://is.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://re.huixiangedu.cn

Ruby: a == b
来源：http://mv.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ns.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vg.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wc.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://bi.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://on.huanxung.cn

TS:   if (x == null) {}
来源：http://ku.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uw.nicolike.cn

Go:   if x == nil {}
来源：http://hw.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kj.gzmigu.cn

C#:   if (x is null) {}
来源：http://wj.jctech888.com.cn

[P07] 防抖与节流
来源：http://vs.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wj.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://dn.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ny.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://am.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zr.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tv.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lf.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mz.asd995.cn

[P08] 处理浮点精度问题
来源：http://dd.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jm.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://go.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jr.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ju.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wi.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://av.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://go.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kt.wgjwhj.cn

================================================================================
来源：http://mx.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rl.szxytkj.cn

================================================================================
来源：http://og.asd995.cn

[Q01] 创建表
来源：http://tt.nszjky.cn


<!-- 参考信息 -->