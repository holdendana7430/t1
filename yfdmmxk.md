代发 wailian999

Py:   resp.json()
来源：http://io.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://fu.gzmigu.cn

JS:   await resp.json()
来源：http://lu.szxytkj.cn

TS:   await resp.json()
来源：http://cg.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gv.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rg.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://bo.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dh.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://gq.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bo.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://um.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://fg.huixiangedu.cn

Java: resp.statusCode()
来源：http://jy.lnxyls.cn

Go:   resp.StatusCode
来源：http://oj.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://oc.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://af.lnxyls.cn

[L08] 并发请求多个地址
来源：http://vt.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gz.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://op.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rv.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yp.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xf.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hm.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vf.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zk.gzmigu.cn

================================================================================
来源：http://er.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ze.szsharing.cn

================================================================================
来源：http://ho.nicolike.cn

[M01] 读取命令行参数
来源：http://pk.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://ne.hahajie.cn

PHP:  $argv;  $argc;
来源：http://ln.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://me.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://jq.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ae.gzmigu.cn

Go:   os.Args[1:]
来源：http://jf.panjiajie.cn

Ruby: ARGV
来源：http://ax.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://pm.panjiajie.cn

[M02] 读取环境变量
来源：http://pg.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://qh.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vn.lnxyls.cn

JS:   process.env.HOME
来源：http://mu.chemitech.net.cn

TS:   process.env.HOME
来源：http://ns.panjiajie.cn

Java: System.getenv("HOME")
来源：http://et.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jk.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://fo.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qc.nicolike.cn

[M03] 执行外部命令
来源：http://si.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uv.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hq.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ds.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rh.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mh.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jw.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ml.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://dk.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ra.bookmarksfly.cn

Py:   os.getcwd()
来源：http://jf.shxzukj.cn

PHP:  getcwd();
来源：http://nj.521024.cn

JS:   process.cwd()
来源：http://px.szsharing.cn

TS:   process.cwd()
来源：http://bq.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://tz.muxihuayi.cn

Go:   os.Getwd()
来源：http://wi.huanxung.cn

Ruby: Dir.pwd
来源：http://cp.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hl.bookmarksfly.cn

[M05] 设置退出码
来源：http://oh.szsharing.cn

Py:   sys.exit(1)
来源：http://ln.nicolike.cn

PHP:  exit(1);
来源：http://xy.szxytkj.cn

JS:   process.exit(1)
来源：http://gn.hnjuh.cn

TS:   process.exit(1)
来源：http://gl.nicolike.cn

Java: System.exit(1)
来源：http://sp.newstarts.cn

Go:   os.Exit(1)
来源：http://dc.muxihuayi.cn

Ruby: exit 1
来源：http://pg.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yy.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ph.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://tj.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bo.shxzukj.cn

JS:   console.error("err")
来源：http://ql.yuntaijiaju.cn

TS:   console.error("err")
来源：http://wc.huanxung.cn

Java: System.err.println("err")
来源：http://ic.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yj.bjjhwx.cn

Ruby: warn "err"
来源：http://zh.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ar.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://ox.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://tj.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kg.gzmigu.cn

JS:   require.main === module
来源：http://bb.panjiajie.cn

TS:   require.main === module
来源：http://fb.colortex.cn

Java: public static void main(String[] args)
来源：http://ri.shxzskj.cn

Go:   func main()
来源：http://re.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rk.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://pk.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://ru.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://pd.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://wq.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://nf.panjiajie.cn

TS:   process.platform;  process.version
来源：http://vr.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ut.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://go.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xb.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fb.yuntaijiaju.cn

================================================================================
来源：http://me.shxzskj.cn

N. 数据结构与算法
来源：http://ve.colortex.cn

================================================================================
来源：http://aa.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://qz.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ke.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ih.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ma.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rz.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sq.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vq.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nw.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yb.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://fm.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jf.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nc.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bl.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bl.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ht.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://mm.nicolike.cn

Ruby: arr.sort
来源：http://ki.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gd.colortex.cn

[N03] 快速排序（分治示例）
来源：http://bt.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bf.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://dc.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pf.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wy.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jm.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lq.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rh.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gi.shxzukj.cn

[N04] 斐波那契数列
来源：http://kh.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uj.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://za.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fv.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vo.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bv.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ig.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cz.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bi.wgjwhj.cn

[N05] 最大公约数
来源：http://gz.hahajie.cn

Py:   math.gcd(a, b)
来源：http://ge.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hs.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xq.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zy.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uk.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rv.shxzukj.cn

Ruby: a.gcd(b)
来源：http://la.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://do.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://rl.shxzskj.cn

Py:   s == s[::-1]
来源：http://pr.colortex.cn

PHP:  $s === strrev($s);
来源：http://ty.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://nm.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://mq.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wv.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://wi.huanxung.cn

Ruby: s == s.reverse
来源：http://kb.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qf.asd995.cn

[N07] 两数之和（返回下标）
来源：http://tg.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kl.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gu.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dx.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://of.hnjuh.cn

Java: // 手写 HashMap
来源：http://rp.colortex.cn

Go:   // 手写 map[int]int
来源：http://zy.gzmigu.cn

Ruby: // 手写 Hash
来源：http://xr.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sj.nicolike.cn

[N08] 生成全排列
来源：http://ck.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://gt.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://cm.szxytkj.cn

JS:   // 手写回溯递归
来源：http://wr.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://nq.chemitech.net.cn

Java: // 手写回溯递归
来源：http://nq.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://hs.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://lw.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://dc.newstarts.cn

[N09] 栈与队列
来源：http://to.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pa.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bf.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://as.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rc.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://as.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zy.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ne.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wh.521024.cn

[N10] 链表节点定义
来源：http://xx.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vw.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bv.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fh.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mr.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://wv.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cb.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ga.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wh.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://xn.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qm.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://fm.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ke.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wa.shxzukj.cn

Java: // 手写递归
来源：http://tj.jianghongdianzi.cn

Go:   // 手写递归
来源：http://yo.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fd.huixinmuqiang.cn

C#:   // 手写递归
来源：http://by.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ef.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ju.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bj.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mk.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xf.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uh.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sc.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ym.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qy.nszjky.cn

================================================================================
来源：http://jq.nicolike.cn

O. 并发与异步
来源：http://no.shtwfgs.cn

================================================================================
来源：http://oy.jctech888.com.cn

[O01] 启动一个线程
来源：http://um.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ez.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qo.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nj.bookmarksfly.cn

TS:   // 同 JS
来源：http://ff.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://ok.bjjhwx.cn

Go:   go f()
来源：http://ac.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://hu.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://mc.jctech888.com.cn

[O02] 使用线程池
来源：http://be.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xv.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hp.huanxung.cn

JS:   // worker_threads 线程池
来源：http://at.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://qh.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hu.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mo.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fq.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ms.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ua.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://vg.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://bl.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ju.bookmarksfly.cn

TS:   // 同 JS
来源：http://ws.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://qs.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ld.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ck.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ar.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://zt.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://aa.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ks.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://nv.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vq.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fh.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ka.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wi.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://gl.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://ev.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://sm.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pc.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://ep.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://lf.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lb.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ar.huanxung.cn

Ruby: threads.map(&:join)
来源：http://eo.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vp.9csxet.cn

[O06] 使用进程池
来源：http://kk.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vz.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wo.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://uq.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://fr.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jo.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sm.asd995.cn

Ruby: // fork 块
来源：http://gv.haigaiapp.cn

C#:   Parallel.For
来源：http://us.szxytkj.cn

================================================================================
来源：http://ir.huixinmuqiang.cn

P. 常用工具函数
来源：http://rk.hahajie.cn

================================================================================
来源：http://cg.shxzskj.cn

[P01] 生成 UUID
来源：http://cg.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://lp.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nb.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://ni.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://za.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://dw.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://mv.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://hm.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://lz.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://yz.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uv.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://my.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://la.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://od.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fz.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://li.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mb.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ux.nszjky.cn

[P03] 生成短随机字符串
来源：http://ck.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ix.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zp.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ov.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xa.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mg.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fw.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ge.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dy.chemitech.net.cn

[P04] 求长度
来源：http://zk.gzmigu.cn


<!-- 参考信息 -->