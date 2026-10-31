代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://os.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ge.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://xe.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iw.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://in.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pp.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ns.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://de.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://ux.szsharing.cn

Java: resp.statusCode()
来源：http://tr.lnxyls.cn

Go:   resp.StatusCode
来源：http://ns.nszjky.cn

Ruby: resp.code.to_i
来源：http://dy.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://wo.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://dk.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nb.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://jx.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://up.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sh.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bd.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zr.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ty.nicolike.cn

================================================================================
来源：http://wd.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://az.huixinmuqiang.cn

================================================================================
来源：http://dj.newstarts.cn

[M01] 读取命令行参数
来源：http://yu.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://vr.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ee.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://km.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://vk.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://bz.yuexingan06.cn

Go:   os.Args[1:]
来源：http://pu.lnxyls.cn

Ruby: ARGV
来源：http://tw.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://td.hnjuh.cn

[M02] 读取环境变量
来源：http://mo.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://cr.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uj.newstarts.cn

JS:   process.env.HOME
来源：http://ke.nicolike.cn

TS:   process.env.HOME
来源：http://qd.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://yy.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bo.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://vw.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://et.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://zt.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ia.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xz.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kf.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xf.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wq.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xd.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fq.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://nk.521024.cn

[M04] 获取当前工作目录
来源：http://zg.521024.cn

Py:   os.getcwd()
来源：http://na.huanxung.cn

PHP:  getcwd();
来源：http://lz.jianghongdianzi.cn

JS:   process.cwd()
来源：http://lz.huanxung.cn

TS:   process.cwd()
来源：http://ln.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://vz.szxytkj.cn

Go:   os.Getwd()
来源：http://rt.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ix.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bj.shxzukj.cn

[M05] 设置退出码
来源：http://ph.9csxet.cn

Py:   sys.exit(1)
来源：http://aj.bjjhwx.cn

PHP:  exit(1);
来源：http://sz.newstarts.cn

JS:   process.exit(1)
来源：http://bv.bookmarksfly.cn

TS:   process.exit(1)
来源：http://dk.hahajie.cn

Java: System.exit(1)
来源：http://dd.chemitech.net.cn

Go:   os.Exit(1)
来源：http://cc.bjjhwx.cn

Ruby: exit 1
来源：http://fj.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vw.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://cx.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://dj.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rh.jianghongdianzi.cn

JS:   console.error("err")
来源：http://fg.haigaiapp.cn

TS:   console.error("err")
来源：http://kw.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ex.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mm.huanxung.cn

Ruby: warn "err"
来源：http://po.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://vq.shxzskj.cn

[M07] 判断是否为主入口
来源：http://pc.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://cw.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wv.jianghongdianzi.cn

JS:   require.main === module
来源：http://mv.shxzskj.cn

TS:   require.main === module
来源：http://sk.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://uo.szsharing.cn

Go:   func main()
来源：http://yl.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oq.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://rp.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ff.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://tq.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://og.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://cx.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://kv.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ct.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://um.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tw.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kn.haigaiapp.cn

================================================================================
来源：http://bg.hnjuh.cn

N. 数据结构与算法
来源：http://ch.nicolike.cn

================================================================================
来源：http://kg.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://lt.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iw.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xs.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uh.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pu.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qd.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://mr.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rq.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tk.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ix.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://zg.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wa.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ml.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sb.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bj.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://jp.bjjhwx.cn

Ruby: arr.sort
来源：http://tt.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ew.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://vq.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fo.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://gr.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fj.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ao.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://do.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yr.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xg.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ge.bjjhwx.cn

[N04] 斐波那契数列
来源：http://iz.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cb.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oc.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ky.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mq.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uq.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dy.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aj.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eo.yuntaijiaju.cn

[N05] 最大公约数
来源：http://xa.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://vr.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://my.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mp.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hf.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pr.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mw.lnxyls.cn

Ruby: a.gcd(b)
来源：http://km.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pc.bjjhwx.cn

[N06] 判断回文字符串
来源：http://xt.huanxung.cn

Py:   s == s[::-1]
来源：http://wu.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://vv.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://yr.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://uo.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ms.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://xh.jctech888.com.cn

Ruby: s == s.reverse
来源：http://ge.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dw.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://jw.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kl.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uk.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vj.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://oo.wgjwhj.cn

Java: // 手写 HashMap
来源：http://mb.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://bm.gzmigu.cn

Ruby: // 手写 Hash
来源：http://sa.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ml.jctech888.com.cn

[N08] 生成全排列
来源：http://wd.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://ad.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://rr.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://ib.521024.cn

TS:   // 手写回溯递归
来源：http://tr.nicolike.cn

Java: // 手写回溯递归
来源：http://sv.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://kj.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://ni.lnxyls.cn

C#:   // 手写回溯递归
来源：http://vs.newstarts.cn

[N09] 栈与队列
来源：http://oo.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dk.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wl.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yl.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ni.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jc.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vi.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://or.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nb.yuexingan06.cn

[N10] 链表节点定义
来源：http://mp.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wj.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tu.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mk.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sb.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://kh.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zs.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wi.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jp.huanxung.cn

[N11] 二叉树中序遍历
来源：http://mr.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lk.colortex.cn

PHP:  // 手写递归函数
来源：http://no.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kv.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://th.huanxung.cn

Java: // 手写递归
来源：http://gu.newstarts.cn

Go:   // 手写递归
来源：http://bq.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uu.yuntaijiaju.cn

C#:   // 手写递归
来源：http://sx.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eu.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wm.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rv.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zk.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mh.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vk.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gs.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xr.bjjhwx.cn

================================================================================
来源：http://zd.yuexingan06.cn

O. 并发与异步
来源：http://pa.gzmigu.cn

================================================================================
来源：http://bw.521024.cn

[O01] 启动一个线程
来源：http://fl.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nh.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lz.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ha.colortex.cn

TS:   // 同 JS
来源：http://tm.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://pd.szxytkj.cn

Go:   go f()
来源：http://og.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://wv.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://bb.muxihuayi.cn

[O02] 使用线程池
来源：http://so.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rl.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mn.colortex.cn

JS:   // worker_threads 线程池
来源：http://tb.huanxung.cn

TS:   // worker_threads 线程池
来源：http://kz.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nf.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zm.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lh.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tx.hahajie.cn

[O03] 加锁保护共享数据
来源：http://ml.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://ig.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://vo.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hi.asd995.cn

TS:   // 同 JS
来源：http://us.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://nh.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ma.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://na.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://oj.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ks.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://id.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yk.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://jz.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ts.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hn.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ci.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mu.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://ow.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://sk.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://vw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zx.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://of.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://yc.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cn.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hk.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://ya.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vt.lnxyls.cn

[O06] 使用进程池
来源：http://se.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gp.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mc.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://gk.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://lh.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rp.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bj.wgjwhj.cn

Ruby: // fork 块
来源：http://fn.newstarts.cn

C#:   Parallel.For
来源：http://ny.colortex.cn

================================================================================
来源：http://xw.hahajie.cn

P. 常用工具函数
来源：http://al.521024.cn

================================================================================
来源：http://wo.huanxung.cn

[P01] 生成 UUID
来源：http://lj.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://hg.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ja.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://um.huanxung.cn

TS:   crypto.randomUUID()
来源：http://jy.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://yh.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://sh.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://su.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://cz.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://om.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rq.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hw.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mk.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dv.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ly.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ne.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hv.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gn.521024.cn

[P03] 生成短随机字符串
来源：http://aa.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fu.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bs.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ty.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pi.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ym.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://id.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jl.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kg.jctech888.com.cn

[P04] 求长度
来源：http://cz.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jd.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fk.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mm.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tm.panjiajie.cn


<!-- 参考信息 -->