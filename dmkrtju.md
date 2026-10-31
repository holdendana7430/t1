代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nb.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zs.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nx.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ei.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vr.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://dh.hahajie.cn

Py:   resp.json()
来源：http://lt.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://ad.panjiajie.cn

JS:   await resp.json()
来源：http://le.yuntaijiaju.cn

TS:   await resp.json()
来源：http://io.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ak.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qh.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://rv.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ri.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://uu.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rt.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mb.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ps.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://wq.shtwfgs.cn

Java: resp.statusCode()
来源：http://uq.jctech888.com.cn

Go:   resp.StatusCode
来源：http://qw.lnxyls.cn

Ruby: resp.code.to_i
来源：http://fm.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://ma.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://is.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ee.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://wk.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ch.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pw.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zg.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wp.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jt.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qy.hahajie.cn

================================================================================
来源：http://ct.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://rr.panjiajie.cn

================================================================================
来源：http://jh.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://gi.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://go.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://sr.nicolike.cn

JS:   process.argv.slice(2)
来源：http://vw.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://ea.colortex.cn

Java: args 数组（main 方法参数）
来源：http://lp.haigaiapp.cn

Go:   os.Args[1:]
来源：http://sj.9csxet.cn

Ruby: ARGV
来源：http://kh.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://id.bjjhwx.cn

[M02] 读取环境变量
来源：http://zs.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://xs.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://no.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ey.muxihuayi.cn

TS:   process.env.HOME
来源：http://mi.huanxung.cn

Java: System.getenv("HOME")
来源：http://va.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kb.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://ja.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qd.shxzskj.cn

[M03] 执行外部命令
来源：http://td.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://or.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yj.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gy.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yo.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://et.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lj.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tr.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://yi.szxytkj.cn

[M04] 获取当前工作目录
来源：http://bg.asd995.cn

Py:   os.getcwd()
来源：http://lk.chemitech.net.cn

PHP:  getcwd();
来源：http://ye.szsharing.cn

JS:   process.cwd()
来源：http://rt.haigaiapp.cn

TS:   process.cwd()
来源：http://ak.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://pp.chemitech.net.cn

Go:   os.Getwd()
来源：http://hc.nicolike.cn

Ruby: Dir.pwd
来源：http://eb.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tv.nszjky.cn

[M05] 设置退出码
来源：http://ui.hahajie.cn

Py:   sys.exit(1)
来源：http://co.yuexingan06.cn

PHP:  exit(1);
来源：http://ii.szsharing.cn

JS:   process.exit(1)
来源：http://ac.hnjuh.cn

TS:   process.exit(1)
来源：http://zd.lnxyls.cn

Java: System.exit(1)
来源：http://va.szsharing.cn

Go:   os.Exit(1)
来源：http://rx.wgjwhj.cn

Ruby: exit 1
来源：http://yv.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://um.newstarts.cn

[M06] 向标准错误输出
来源：http://gk.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://uu.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://np.bjjhwx.cn

JS:   console.error("err")
来源：http://de.newstarts.cn

TS:   console.error("err")
来源：http://qe.bjjhwx.cn

Java: System.err.println("err")
来源：http://yl.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ni.jianghongdianzi.cn

Ruby: warn "err"
来源：http://hd.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://je.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://qh.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://dh.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ca.panjiajie.cn

JS:   require.main === module
来源：http://so.gzmigu.cn

TS:   require.main === module
来源：http://jg.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://lv.wgjwhj.cn

Go:   func main()
来源：http://oc.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ru.521024.cn

C#:   static void Main(string[] args)
来源：http://ls.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://ps.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://rt.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://wc.panjiajie.cn

JS:   process.platform;  process.version
来源：http://dh.nszjky.cn

TS:   process.platform;  process.version
来源：http://xs.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wh.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://od.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uf.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kg.szxytkj.cn

================================================================================
来源：http://ha.jianghongdianzi.cn

N. 数据结构与算法
来源：http://vj.hahajie.cn

================================================================================
来源：http://dh.asd995.cn

[N01] 二分查找（有序数组）
来源：http://mf.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kt.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vl.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cx.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://mm.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sg.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://km.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://se.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://il.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ke.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ll.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yv.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://re.huanxung.cn

Ruby: arr.sort
来源：http://jn.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rl.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://mo.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sz.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://kh.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zi.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bc.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hu.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qf.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uh.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gw.521024.cn

[N04] 斐波那契数列
来源：http://cg.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hl.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hv.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rr.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://py.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jj.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mn.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oy.521024.cn

[N05] 最大公约数
来源：http://lh.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://ut.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tw.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bl.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vp.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sc.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://km.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://df.asd995.cn

[N06] 判断回文字符串
来源：http://mm.newstarts.cn

Py:   s == s[::-1]
来源：http://sl.9csxet.cn

PHP:  $s === strrev($s);
来源：http://wt.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://uz.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://uw.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://re.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://cc.hahajie.cn

Ruby: s == s.reverse
来源：http://zl.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fe.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://wd.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fd.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yw.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wf.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://cc.panjiajie.cn

Java: // 手写 HashMap
来源：http://gk.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://nl.521024.cn

Ruby: // 手写 Hash
来源：http://lx.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wp.panjiajie.cn

[N08] 生成全排列
来源：http://vq.colortex.cn

Py:   itertools.permutations(arr)
来源：http://lg.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ii.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://mn.newstarts.cn

TS:   // 手写回溯递归
来源：http://gw.newstarts.cn

Java: // 手写回溯递归
来源：http://en.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://ym.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://kv.hnjuh.cn

C#:   // 手写回溯递归
来源：http://mj.hahajie.cn

[N09] 栈与队列
来源：http://dl.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bz.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fp.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fj.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wv.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wa.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dn.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kj.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ec.szsharing.cn

[N10] 链表节点定义
来源：http://rl.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wl.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qx.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mg.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://be.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://rr.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lz.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wh.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uh.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://bb.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hk.shxzskj.cn

PHP:  // 手写递归函数
来源：http://gh.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fh.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://en.szsharing.cn

Java: // 手写递归
来源：http://fh.521024.cn

Go:   // 手写递归
来源：http://wt.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yf.muxihuayi.cn

C#:   // 手写递归
来源：http://ad.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://db.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yg.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qf.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ki.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ro.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fk.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://el.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fa.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pl.haigaiapp.cn

================================================================================
来源：http://rv.jctech888.com.cn

O. 并发与异步
来源：http://uj.huixiangedu.cn

================================================================================
来源：http://ra.yuexingan06.cn

[O01] 启动一个线程
来源：http://bp.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jt.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xc.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fk.bjjhwx.cn

TS:   // 同 JS
来源：http://nb.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://rr.shxzukj.cn

Go:   go f()
来源：http://oq.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://sn.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://ml.asd995.cn

[O02] 使用线程池
来源：http://jk.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rx.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kl.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://ok.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://ts.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zg.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mo.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xr.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zg.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://vz.nszjky.cn

Py:   with lock: shared += 1
来源：http://si.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://mo.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ca.muxihuayi.cn

TS:   // 同 JS
来源：http://hc.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://xl.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ma.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ci.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://sl.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://jw.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://ua.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lu.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://lw.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yu.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ku.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://va.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qt.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://dp.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://uk.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://yk.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://af.521024.cn

JS:   await Promise.all(tasks)
来源：http://vu.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://nl.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vd.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rr.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://fm.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hx.huixinmuqiang.cn

[O06] 使用进程池
来源：http://ca.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rm.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wa.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://nm.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://vs.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lo.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://md.lnxyls.cn

Ruby: // fork 块
来源：http://ue.colortex.cn

C#:   Parallel.For
来源：http://wa.gzmigu.cn

================================================================================
来源：http://tt.szsharing.cn

P. 常用工具函数
来源：http://ms.hahajie.cn

================================================================================
来源：http://oy.gzmigu.cn

[P01] 生成 UUID
来源：http://nk.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://vu.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ik.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ho.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://gy.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://jr.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://rb.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://an.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://bi.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://xb.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wh.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xe.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uc.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eo.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tl.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://du.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oz.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xu.szxytkj.cn

[P03] 生成短随机字符串
来源：http://fz.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cu.hahajie.cn


<!-- 参考信息 -->