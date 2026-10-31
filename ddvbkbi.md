代发 wailian999

Py:   resp.json()
来源：http://hm.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://gn.shxzskj.cn

JS:   await resp.json()
来源：http://nc.shxzskj.cn

TS:   await resp.json()
来源：http://lk.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pf.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ie.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://ml.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oy.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://sn.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ek.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yw.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://ya.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ur.shtwfgs.cn

Java: resp.statusCode()
来源：http://me.hnjuh.cn

Go:   resp.StatusCode
来源：http://jm.colortex.cn

Ruby: resp.code.to_i
来源：http://yn.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://bv.panjiajie.cn

[L08] 并发请求多个地址
来源：http://sz.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jt.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://us.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yj.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://we.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qe.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ga.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dm.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xj.muxihuayi.cn

================================================================================
来源：http://kd.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://we.panjiajie.cn

================================================================================
来源：http://sy.szxytkj.cn

[M01] 读取命令行参数
来源：http://zh.521024.cn

Py:   sys.argv[1:]
来源：http://sk.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://ia.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://fo.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://gx.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://su.haigaiapp.cn

Go:   os.Args[1:]
来源：http://sl.bjjhwx.cn

Ruby: ARGV
来源：http://ci.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://xs.9csxet.cn

[M02] 读取环境变量
来源：http://xj.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://ey.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xg.shxzukj.cn

JS:   process.env.HOME
来源：http://mq.lnxyls.cn

TS:   process.env.HOME
来源：http://ul.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://fe.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gr.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://zr.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bq.muxihuayi.cn

[M03] 执行外部命令
来源：http://js.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tx.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ef.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qs.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qi.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ez.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vj.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xb.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ix.shxzukj.cn

[M04] 获取当前工作目录
来源：http://uq.chemitech.net.cn

Py:   os.getcwd()
来源：http://uf.jctech888.com.cn

PHP:  getcwd();
来源：http://wr.wgjwhj.cn

JS:   process.cwd()
来源：http://oz.nszjky.cn

TS:   process.cwd()
来源：http://zc.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://vg.nszjky.cn

Go:   os.Getwd()
来源：http://sr.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ij.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pe.huixinmuqiang.cn

[M05] 设置退出码
来源：http://fs.hnjuh.cn

Py:   sys.exit(1)
来源：http://sv.chemitech.net.cn

PHP:  exit(1);
来源：http://aj.huanxung.cn

JS:   process.exit(1)
来源：http://kf.asd995.cn

TS:   process.exit(1)
来源：http://en.lnxyls.cn

Java: System.exit(1)
来源：http://rs.9csxet.cn

Go:   os.Exit(1)
来源：http://rx.wgjwhj.cn

Ruby: exit 1
来源：http://ys.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cm.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://yh.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://ho.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xb.yuntaijiaju.cn

JS:   console.error("err")
来源：http://np.panjiajie.cn

TS:   console.error("err")
来源：http://iv.521024.cn

Java: System.err.println("err")
来源：http://jl.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dx.huixiangedu.cn

Ruby: warn "err"
来源：http://jw.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://yt.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://rz.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://pv.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cl.huanxung.cn

JS:   require.main === module
来源：http://mk.shxzskj.cn

TS:   require.main === module
来源：http://rf.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://br.nszjky.cn

Go:   func main()
来源：http://ib.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fw.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://yt.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://ye.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://nr.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://al.panjiajie.cn

JS:   process.platform;  process.version
来源：http://mm.9csxet.cn

TS:   process.platform;  process.version
来源：http://vx.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zy.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://un.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yl.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qh.newstarts.cn

================================================================================
来源：http://re.nszjky.cn

N. 数据结构与算法
来源：http://yj.szsharing.cn

================================================================================
来源：http://dy.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://yb.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fw.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ri.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kq.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dt.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ut.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jm.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fd.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://rj.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://nn.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://po.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yd.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cv.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pt.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://rq.newstarts.cn

Ruby: arr.sort
来源：http://ig.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ht.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://zm.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xx.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://kv.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jc.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kw.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dg.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rs.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kh.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kp.wgjwhj.cn

[N04] 斐波那契数列
来源：http://tu.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zo.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vn.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zu.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cq.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sb.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ih.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kt.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sr.asd995.cn

[N05] 最大公约数
来源：http://dq.asd995.cn

Py:   math.gcd(a, b)
来源：http://iw.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ur.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hr.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mx.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rf.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://wg.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://po.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://wa.panjiajie.cn

Py:   s == s[::-1]
来源：http://jv.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ez.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://xc.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://iq.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qx.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://wf.szsharing.cn

Ruby: s == s.reverse
来源：http://ro.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fm.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://hh.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oq.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ay.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cc.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://dl.huixiangedu.cn

Java: // 手写 HashMap
来源：http://hm.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://cx.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://dy.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ai.wgjwhj.cn

[N08] 生成全排列
来源：http://bc.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://cg.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://dh.asd995.cn

JS:   // 手写回溯递归
来源：http://bd.colortex.cn

TS:   // 手写回溯递归
来源：http://av.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://wa.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://uz.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://cl.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://oe.huixiangedu.cn

[N09] 栈与队列
来源：http://js.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jg.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yz.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pp.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cb.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ij.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fv.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iu.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lu.bookmarksfly.cn

[N10] 链表节点定义
来源：http://od.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qq.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rs.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jo.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aj.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://fh.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://co.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ok.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ya.nszjky.cn

[N11] 二叉树中序遍历
来源：http://ke.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://my.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://sb.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tz.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qd.newstarts.cn

Java: // 手写递归
来源：http://rv.jctech888.com.cn

Go:   // 手写递归
来源：http://xq.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pb.wgjwhj.cn

C#:   // 手写递归
来源：http://zl.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ww.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hd.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ss.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nk.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ad.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iz.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hp.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tu.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rl.newstarts.cn

================================================================================
来源：http://ja.panjiajie.cn

O. 并发与异步
来源：http://ct.gzmigu.cn

================================================================================
来源：http://ca.hahajie.cn

[O01] 启动一个线程
来源：http://fn.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ql.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://if.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aj.hahajie.cn

TS:   // 同 JS
来源：http://tg.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://ip.shtwfgs.cn

Go:   go f()
来源：http://gk.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://sc.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://pl.9csxet.cn

[O02] 使用线程池
来源：http://xl.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eh.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kx.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://zp.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://yk.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zz.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zy.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ja.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iv.hahajie.cn

[O03] 加锁保护共享数据
来源：http://xy.colortex.cn

Py:   with lock: shared += 1
来源：http://le.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ln.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gq.huanxung.cn

TS:   // 同 JS
来源：http://em.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://db.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pu.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rg.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://ot.nicolike.cn

[O04] 定义异步函数并等待
来源：http://sz.521024.cn

Py:   async def f():⏎    await g()
来源：http://yz.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dw.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://jt.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ud.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://or.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qb.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zo.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://tx.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://ks.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://rs.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hx.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://mq.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://am.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jx.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hd.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://qk.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cp.colortex.cn

[O06] 使用进程池
来源：http://ny.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zm.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rp.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://jl.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://tp.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pw.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zd.bjjhwx.cn

Ruby: // fork 块
来源：http://xw.jctech888.com.cn

C#:   Parallel.For
来源：http://ad.huixinmuqiang.cn

================================================================================
来源：http://vf.haigaiapp.cn

P. 常用工具函数
来源：http://oy.huixiangedu.cn

================================================================================
来源：http://up.shtwfgs.cn

[P01] 生成 UUID
来源：http://el.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://rn.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rc.521024.cn

JS:   crypto.randomUUID()
来源：http://cx.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://sq.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://vf.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://wc.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://fd.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://bf.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://la.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dc.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://km.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qr.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tl.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://av.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nm.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yc.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ab.nszjky.cn

[P03] 生成短随机字符串
来源：http://td.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://at.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cw.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iu.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sx.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aa.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aq.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qx.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vd.szsharing.cn

[P04] 求长度
来源：http://po.chemitech.net.cn


<!-- 参考信息 -->