代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ah.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cb.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jw.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ee.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wt.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rt.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://co.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wz.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sh.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wn.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xy.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ja.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cf.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ga.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://fp.jctech888.com.cn

Py:   resp.json()
来源：http://bi.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://mq.yuexingan06.cn

JS:   await resp.json()
来源：http://nx.haigaiapp.cn

TS:   await resp.json()
来源：http://qa.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bm.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ec.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://wm.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ns.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://op.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ja.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://do.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://ba.521024.cn

Java: resp.statusCode()
来源：http://hr.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ki.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://ox.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://px.asd995.cn

[L08] 并发请求多个地址
来源：http://mn.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kt.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://aq.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xf.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wk.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vs.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ly.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rd.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iv.muxihuayi.cn

================================================================================
来源：http://tk.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://vg.panjiajie.cn

================================================================================
来源：http://nx.szsharing.cn

[M01] 读取命令行参数
来源：http://mo.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://dd.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://tf.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://vt.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://hg.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yf.szxytkj.cn

Go:   os.Args[1:]
来源：http://ni.gzmigu.cn

Ruby: ARGV
来源：http://ys.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://zs.nszjky.cn

[M02] 读取环境变量
来源：http://or.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://in.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mj.bookmarksfly.cn

JS:   process.env.HOME
来源：http://tg.huanxung.cn

TS:   process.env.HOME
来源：http://fr.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://xc.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ha.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://gn.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vr.panjiajie.cn

[M03] 执行外部命令
来源：http://um.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kl.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rk.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vc.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iq.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ng.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jh.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zt.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://gp.hnjuh.cn

[M04] 获取当前工作目录
来源：http://he.bjjhwx.cn

Py:   os.getcwd()
来源：http://og.nszjky.cn

PHP:  getcwd();
来源：http://af.huixiangedu.cn

JS:   process.cwd()
来源：http://no.nszjky.cn

TS:   process.cwd()
来源：http://ap.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://hl.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://jy.wgjwhj.cn

Ruby: Dir.pwd
来源：http://wz.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xx.gzmigu.cn

[M05] 设置退出码
来源：http://sj.panjiajie.cn

Py:   sys.exit(1)
来源：http://uy.asd995.cn

PHP:  exit(1);
来源：http://va.nicolike.cn

JS:   process.exit(1)
来源：http://np.szsharing.cn

TS:   process.exit(1)
来源：http://ne.wgjwhj.cn

Java: System.exit(1)
来源：http://bp.nicolike.cn

Go:   os.Exit(1)
来源：http://cz.haigaiapp.cn

Ruby: exit 1
来源：http://jc.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ey.asd995.cn

[M06] 向标准错误输出
来源：http://ay.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://cm.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://us.9csxet.cn

JS:   console.error("err")
来源：http://bx.jctech888.com.cn

TS:   console.error("err")
来源：http://qb.panjiajie.cn

Java: System.err.println("err")
来源：http://hb.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lc.yuntaijiaju.cn

Ruby: warn "err"
来源：http://aj.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://tp.nszjky.cn

[M07] 判断是否为主入口
来源：http://mj.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://rt.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tb.lnxyls.cn

JS:   require.main === module
来源：http://pe.9csxet.cn

TS:   require.main === module
来源：http://fa.asd995.cn

Java: public static void main(String[] args)
来源：http://in.szxytkj.cn

Go:   func main()
来源：http://le.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://my.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://kj.521024.cn

[M08] 获取系统与运行时信息
来源：http://yp.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://mf.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://xh.9csxet.cn

JS:   process.platform;  process.version
来源：http://pq.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://rw.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://je.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hd.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tb.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ji.huixinmuqiang.cn

================================================================================
来源：http://gx.lnxyls.cn

N. 数据结构与算法
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://zo.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://ec.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://au.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://so.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://md.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ch.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sm.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://nd.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wx.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qt.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qm.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mb.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uj.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pb.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pz.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://fj.jctech888.com.cn

Ruby: arr.sort
来源：http://li.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xy.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://wl.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wv.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://em.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rb.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rp.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rd.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pk.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sx.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ex.szsharing.cn

[N04] 斐波那契数列
来源：http://ch.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nk.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fl.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://go.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://my.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rt.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iu.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qg.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vx.huixiangedu.cn

[N05] 最大公约数
来源：http://js.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ir.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ew.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oh.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pv.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nu.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xo.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://ku.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uo.lnxyls.cn

[N06] 判断回文字符串
来源：http://pq.gzmigu.cn

Py:   s == s[::-1]
来源：http://iu.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://xi.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://fd.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://mb.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vc.newstarts.cn

Go:   // 双指针从两端比较
来源：http://zi.nicolike.cn

Ruby: s == s.reverse
来源：http://zy.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lh.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ke.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tu.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nq.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xc.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://rp.lnxyls.cn

Java: // 手写 HashMap
来源：http://nj.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://is.newstarts.cn

Ruby: // 手写 Hash
来源：http://vr.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ka.gzmigu.cn

[N08] 生成全排列
来源：http://cr.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://vq.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://lp.szsharing.cn

JS:   // 手写回溯递归
来源：http://xy.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://wd.gzmigu.cn

Java: // 手写回溯递归
来源：http://xv.shxzukj.cn

Go:   // 手写回溯递归
来源：http://qa.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://rs.huanxung.cn

C#:   // 手写回溯递归
来源：http://cf.huixinmuqiang.cn

[N09] 栈与队列
来源：http://sk.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qa.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://er.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cv.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ke.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zh.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sk.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cz.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ln.colortex.cn

[N10] 链表节点定义
来源：http://tq.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vg.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qz.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ro.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ww.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://qf.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ob.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kq.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sx.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://kk.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eq.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://nt.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jb.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iu.hnjuh.cn

Java: // 手写递归
来源：http://qq.nicolike.cn

Go:   // 手写递归
来源：http://wf.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gm.shxzskj.cn

C#:   // 手写递归
来源：http://ug.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nb.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ww.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sw.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bg.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rw.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lc.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qa.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cr.9csxet.cn

================================================================================
来源：http://qj.bookmarksfly.cn

O. 并发与异步
来源：http://ga.haigaiapp.cn

================================================================================
来源：http://ln.nszjky.cn

[O01] 启动一个线程
来源：http://zw.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tr.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fb.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qt.shxzskj.cn

TS:   // 同 JS
来源：http://hs.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://je.colortex.cn

Go:   go f()
来源：http://uq.panjiajie.cn

Ruby: Thread.new { f }
来源：http://ix.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://ji.huanxung.cn

[O02] 使用线程池
来源：http://qf.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fh.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zc.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://rn.521024.cn

TS:   // worker_threads 线程池
来源：http://az.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dv.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mf.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kv.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cj.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://ew.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://hh.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://se.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cj.szxytkj.cn

TS:   // 同 JS
来源：http://et.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://zc.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zx.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ld.521024.cn

C#:   lock (gate) { shared++; }
来源：http://sm.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://ty.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://dj.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://er.9csxet.cn

JS:   async function f() { await g(); }
来源：http://sf.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dk.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cw.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://is.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eq.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://xl.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ya.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://jm.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pa.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://io.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://iw.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://za.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ee.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://ie.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dc.huanxung.cn

[O06] 使用进程池
来源：http://mm.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gn.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ws.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://qe.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://wm.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ch.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hd.panjiajie.cn

Ruby: // fork 块
来源：http://lc.lnxyls.cn

C#:   Parallel.For
来源：http://mp.haigaiapp.cn

================================================================================
来源：http://qo.huanxung.cn

P. 常用工具函数
来源：http://br.nicolike.cn

================================================================================
来源：http://vt.szsharing.cn

[P01] 生成 UUID
来源：http://gt.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://yt.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mi.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://up.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://jq.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://kz.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ol.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://kl.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://kx.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://vd.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bj.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ch.lnxyls.cn


<!-- 参考信息 -->