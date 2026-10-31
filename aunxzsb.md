代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wd.hnjuh.cn

JS:   process.env.HOME
来源：http://sb.yuexingan06.cn

TS:   process.env.HOME
来源：http://vv.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://md.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://og.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://pi.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fv.yuexingan06.cn

[M03] 执行外部命令
来源：http://bi.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hv.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fj.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ln.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cq.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qg.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jr.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nq.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://nw.hnjuh.cn

[M04] 获取当前工作目录
来源：http://tl.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://us.haigaiapp.cn

PHP:  getcwd();
来源：http://lb.chemitech.net.cn

JS:   process.cwd()
来源：http://ew.haigaiapp.cn

TS:   process.cwd()
来源：http://fv.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://tk.shxzskj.cn

Go:   os.Getwd()
来源：http://oj.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ny.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gw.bjjhwx.cn

[M05] 设置退出码
来源：http://nb.nszjky.cn

Py:   sys.exit(1)
来源：http://if.shxzskj.cn

PHP:  exit(1);
来源：http://jf.bjjhwx.cn

JS:   process.exit(1)
来源：http://ez.wgjwhj.cn

TS:   process.exit(1)
来源：http://ts.haigaiapp.cn

Java: System.exit(1)
来源：http://df.nszjky.cn

Go:   os.Exit(1)
来源：http://xg.shtwfgs.cn

Ruby: exit 1
来源：http://jw.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mo.yuexingan06.cn

[M06] 向标准错误输出
来源：http://bd.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://pn.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gj.yuexingan06.cn

JS:   console.error("err")
来源：http://zq.huanxung.cn

TS:   console.error("err")
来源：http://yl.szxytkj.cn

Java: System.err.println("err")
来源：http://uq.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ms.panjiajie.cn

Ruby: warn "err"
来源：http://mi.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://aj.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://mj.colortex.cn

Py:   if __name__ == "__main__":
来源：http://za.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wu.gzmigu.cn

JS:   require.main === module
来源：http://fg.nicolike.cn

TS:   require.main === module
来源：http://yn.nicolike.cn

Java: public static void main(String[] args)
来源：http://dx.colortex.cn

Go:   func main()
来源：http://xk.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ku.asd995.cn

C#:   static void Main(string[] args)
来源：http://ka.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://op.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://yg.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://ud.521024.cn

JS:   process.platform;  process.version
来源：http://hs.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://ps.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cr.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ch.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vj.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uk.chemitech.net.cn

================================================================================
来源：http://oj.lnxyls.cn

N. 数据结构与算法
来源：http://zx.newstarts.cn

================================================================================
来源：http://vd.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://mm.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yf.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xe.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ix.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fe.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mo.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://lu.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rv.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nc.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://rq.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ll.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ei.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tr.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zt.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bi.521024.cn

Go:   slices.Sort(arr)
来源：http://cd.szxytkj.cn

Ruby: arr.sort
来源：http://iz.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tw.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://jp.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bj.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://th.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ks.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tw.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gj.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fw.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tb.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ml.hahajie.cn

[N04] 斐波那契数列
来源：http://pq.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ue.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mi.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://os.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cu.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bt.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pk.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wt.newstarts.cn

[N05] 最大公约数
来源：http://vd.9csxet.cn

Py:   math.gcd(a, b)
来源：http://qi.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fk.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nr.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cn.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nx.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hp.nicolike.cn

Ruby: a.gcd(b)
来源：http://xb.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://np.gzmigu.cn

[N06] 判断回文字符串
来源：http://gf.szsharing.cn

Py:   s == s[::-1]
来源：http://zv.nicolike.cn

PHP:  $s === strrev($s);
来源：http://pp.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://qr.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://do.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aa.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://jn.shxzukj.cn

Ruby: s == s.reverse
来源：http://kf.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://me.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://be.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://st.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vv.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fx.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ri.yuexingan06.cn

Java: // 手写 HashMap
来源：http://xh.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://fm.lnxyls.cn

Ruby: // 手写 Hash
来源：http://wr.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://va.muxihuayi.cn

[N08] 生成全排列
来源：http://gg.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://sa.huanxung.cn

PHP:  // 手写递归交换
来源：http://az.huanxung.cn

JS:   // 手写回溯递归
来源：http://up.9csxet.cn

TS:   // 手写回溯递归
来源：http://op.szxytkj.cn

Java: // 手写回溯递归
来源：http://xv.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://cc.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://gr.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://td.huanxung.cn

[N09] 栈与队列
来源：http://ki.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ge.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pq.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bs.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hh.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lt.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yy.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bp.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ao.521024.cn

[N10] 链表节点定义
来源：http://wi.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oz.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wr.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://is.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jd.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ii.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qc.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://il.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ke.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://xj.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kr.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://av.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tg.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xh.muxihuayi.cn

Java: // 手写递归
来源：http://ik.bjjhwx.cn

Go:   // 手写递归
来源：http://dw.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bh.lnxyls.cn

C#:   // 手写递归
来源：http://pt.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uy.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gl.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tp.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sn.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pb.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dh.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ec.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yn.asd995.cn

================================================================================
来源：http://nd.szsharing.cn

O. 并发与异步
来源：http://kg.szxytkj.cn

================================================================================
来源：http://dm.szsharing.cn

[O01] 启动一个线程
来源：http://zh.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yx.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yi.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zw.bjjhwx.cn

TS:   // 同 JS
来源：http://rg.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://rx.yuexingan06.cn

Go:   go f()
来源：http://aw.szsharing.cn

Ruby: Thread.new { f }
来源：http://ns.nicolike.cn

C#:   Task.Run(() => F());
来源：http://nv.wgjwhj.cn

[O02] 使用线程池
来源：http://bv.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bu.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fx.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://af.hahajie.cn

TS:   // worker_threads 线程池
来源：http://ss.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ov.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oa.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hh.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wo.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://hl.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://fh.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://jk.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wk.asd995.cn

TS:   // 同 JS
来源：http://zp.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://vj.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ds.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://so.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://zs.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ai.521024.cn

Py:   async def f():⏎    await g()
来源：http://zn.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ke.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://li.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://io.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xh.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wd.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ig.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://bb.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://nr.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ec.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ch.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://rg.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://ml.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vd.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://to.521024.cn

Ruby: threads.map(&:join)
来源：http://tv.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://io.521024.cn

[O06] 使用进程池
来源：http://ns.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jy.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jh.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://fo.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://jv.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bo.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sd.gzmigu.cn

Ruby: // fork 块
来源：http://em.wgjwhj.cn

C#:   Parallel.For
来源：http://sb.gzmigu.cn

================================================================================
来源：http://kk.shxzskj.cn

P. 常用工具函数
来源：http://vv.hnjuh.cn

================================================================================
来源：http://yc.wgjwhj.cn

[P01] 生成 UUID
来源：http://yn.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://fr.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kb.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://pr.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://ff.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://co.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ml.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://hg.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://fz.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://gn.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hv.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hm.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pj.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://su.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jd.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wu.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gu.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://je.nszjky.cn

[P03] 生成短随机字符串
来源：http://vu.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ne.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bf.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wa.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rd.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://go.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ef.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pf.gzmigu.cn

[P04] 求长度
来源：http://gq.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ie.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xt.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eb.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sf.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://gs.nicolike.cn

Go:   len(arr);  len(m)
来源：http://xf.shxzskj.cn

Ruby: x.length;  x.size
来源：http://tp.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wg.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://sr.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://au.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gd.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vc.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gr.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uv.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://re.shxzukj.cn

Ruby: a == b
来源：http://ue.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gh.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xv.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://um.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://wt.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ct.chemitech.net.cn

TS:   if (x == null) {}
来源：http://bx.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lu.colortex.cn

Go:   if x == nil {}
来源：http://gx.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gn.wgjwhj.cn

C#:   if (x is null) {}
来源：http://to.nicolike.cn

[P07] 防抖与节流
来源：http://rl.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ph.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://xb.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wl.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fb.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rw.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ae.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tp.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://si.asd995.cn

[P08] 处理浮点精度问题
来源：http://rj.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://be.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tn.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sl.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ds.huixinmuqiang.cn


<!-- 参考信息 -->