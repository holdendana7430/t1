代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ih.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://di.hahajie.cn

[L05] 上传文件（multipart）
来源：http://nd.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bc.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xm.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qj.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sa.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qx.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bw.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://id.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yk.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://tz.haigaiapp.cn

Py:   resp.json()
来源：http://jy.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://jz.gzmigu.cn

JS:   await resp.json()
来源：http://fn.haigaiapp.cn

TS:   await resp.json()
来源：http://tu.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vk.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pz.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://vv.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cc.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://fu.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zd.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nx.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://wv.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://dh.yuexingan06.cn

Java: resp.statusCode()
来源：http://wa.szxytkj.cn

Go:   resp.StatusCode
来源：http://op.huanxung.cn

Ruby: resp.code.to_i
来源：http://cf.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://lu.panjiajie.cn

[L08] 并发请求多个地址
来源：http://qq.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dr.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://lo.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mf.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kp.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ks.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mu.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pl.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uk.colortex.cn

================================================================================
来源：http://km.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://np.shxzskj.cn

================================================================================
来源：http://hx.lnxyls.cn

[M01] 读取命令行参数
来源：http://wj.colortex.cn

Py:   sys.argv[1:]
来源：http://yk.521024.cn

PHP:  $argv;  $argc;
来源：http://ws.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ev.hahajie.cn

TS:   process.argv.slice(2)
来源：http://dp.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://zg.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://ul.hnjuh.cn

Ruby: ARGV
来源：http://ut.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://yi.muxihuayi.cn

[M02] 读取环境变量
来源：http://jp.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://xg.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dh.szsharing.cn

JS:   process.env.HOME
来源：http://kg.shxzskj.cn

TS:   process.env.HOME
来源：http://st.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://jz.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ba.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://rw.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ia.jctech888.com.cn

[M03] 执行外部命令
来源：http://kj.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fv.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ib.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hc.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dt.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oc.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ky.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uf.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ew.colortex.cn

[M04] 获取当前工作目录
来源：http://al.jctech888.com.cn

Py:   os.getcwd()
来源：http://xw.huixiangedu.cn

PHP:  getcwd();
来源：http://go.panjiajie.cn

JS:   process.cwd()
来源：http://dh.szxytkj.cn

TS:   process.cwd()
来源：http://cu.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ud.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://vm.521024.cn

Ruby: Dir.pwd
来源：http://nq.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wn.yuexingan06.cn

[M05] 设置退出码
来源：http://gw.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ab.newstarts.cn

PHP:  exit(1);
来源：http://nq.hahajie.cn

JS:   process.exit(1)
来源：http://bb.shxzskj.cn

TS:   process.exit(1)
来源：http://pb.asd995.cn

Java: System.exit(1)
来源：http://fi.hahajie.cn

Go:   os.Exit(1)
来源：http://zn.521024.cn

Ruby: exit 1
来源：http://wj.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mb.szxytkj.cn

[M06] 向标准错误输出
来源：http://hw.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://et.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uv.yuexingan06.cn

JS:   console.error("err")
来源：http://ln.colortex.cn

TS:   console.error("err")
来源：http://iu.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://px.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xm.shxzukj.cn

Ruby: warn "err"
来源：http://na.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://sq.huanxung.cn

[M07] 判断是否为主入口
来源：http://uk.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://bx.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qj.huixiangedu.cn

JS:   require.main === module
来源：http://ps.szsharing.cn

TS:   require.main === module
来源：http://we.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://kg.yuntaijiaju.cn

Go:   func main()
来源：http://it.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zg.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://gi.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://dz.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://qz.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://rg.nicolike.cn

JS:   process.platform;  process.version
来源：http://jz.panjiajie.cn

TS:   process.platform;  process.version
来源：http://xa.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://he.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dc.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yf.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://et.shxzukj.cn

================================================================================
来源：http://hs.yuexingan06.cn

N. 数据结构与算法
来源：http://fe.huixinmuqiang.cn

================================================================================
来源：http://my.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://ri.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eh.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bd.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://we.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xj.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://po.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ci.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wi.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ol.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://dx.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rg.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://co.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vk.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://um.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://px.lnxyls.cn

Ruby: arr.sort
来源：http://bj.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tx.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://tp.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wf.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://fx.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mi.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ze.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://et.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ml.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ut.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vw.panjiajie.cn

[N04] 斐波那契数列
来源：http://ar.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pp.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gm.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qh.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pf.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ja.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ez.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://in.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://il.huixiangedu.cn

[N05] 最大公约数
来源：http://jm.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://kw.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ru.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pt.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mf.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dh.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hk.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://vw.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yc.9csxet.cn

[N06] 判断回文字符串
来源：http://hn.asd995.cn

Py:   s == s[::-1]
来源：http://aa.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://cb.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://rw.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://md.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://om.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://lw.shtwfgs.cn

Ruby: s == s.reverse
来源：http://uc.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kz.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://yu.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ap.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cg.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nq.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://jt.chemitech.net.cn

Java: // 手写 HashMap
来源：http://mg.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://ay.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://vm.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xx.newstarts.cn

[N08] 生成全排列
来源：http://pj.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://ce.nicolike.cn

PHP:  // 手写递归交换
来源：http://ry.nicolike.cn

JS:   // 手写回溯递归
来源：http://yx.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://lk.shxzukj.cn

Java: // 手写回溯递归
来源：http://us.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://cq.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://xe.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://us.shxzskj.cn

[N09] 栈与队列
来源：http://ry.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zh.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iq.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fu.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iu.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ew.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qj.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ta.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ti.wgjwhj.cn

[N10] 链表节点定义
来源：http://ie.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mw.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uf.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ei.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rp.asd995.cn

Java: class Node { int v; Node next; }
来源：http://hx.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lr.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jr.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wc.huanxung.cn

[N11] 二叉树中序遍历
来源：http://az.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ua.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://wa.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cn.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nm.yuexingan06.cn

Java: // 手写递归
来源：http://vn.wgjwhj.cn

Go:   // 手写递归
来源：http://yv.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gr.nszjky.cn

C#:   // 手写递归
来源：http://nw.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vn.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zq.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ar.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fc.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bj.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hu.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bq.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bn.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rv.panjiajie.cn

================================================================================
来源：http://jg.huanxung.cn

O. 并发与异步
来源：http://rd.colortex.cn

================================================================================
来源：http://wl.hahajie.cn

[O01] 启动一个线程
来源：http://ix.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ky.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jg.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tw.newstarts.cn

TS:   // 同 JS
来源：http://ns.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://ys.jianghongdianzi.cn

Go:   go f()
来源：http://ng.521024.cn

Ruby: Thread.new { f }
来源：http://uq.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://yu.nszjky.cn

[O02] 使用线程池
来源：http://sj.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vh.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hs.nszjky.cn

JS:   // worker_threads 线程池
来源：http://wa.hahajie.cn

TS:   // worker_threads 线程池
来源：http://nh.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yp.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ey.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ko.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bt.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://sa.hahajie.cn

Py:   with lock: shared += 1
来源：http://ms.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://qc.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rm.huixiangedu.cn

TS:   // 同 JS
来源：http://ez.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://ln.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pd.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://op.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://ge.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://pt.asd995.cn

Py:   async def f():⏎    await g()
来源：http://hn.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gf.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ns.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fi.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ks.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jr.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fb.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://yc.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://mc.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://bk.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sb.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://rh.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://xd.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gb.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wx.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://qe.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jf.wgjwhj.cn

[O06] 使用进程池
来源：http://fk.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ju.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oz.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://dd.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://yq.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://he.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nr.chemitech.net.cn

Ruby: // fork 块
来源：http://fr.huixinmuqiang.cn

C#:   Parallel.For
来源：http://mt.asd995.cn

================================================================================
来源：http://ue.hahajie.cn

P. 常用工具函数
来源：http://vd.shxzskj.cn

================================================================================
来源：http://le.asd995.cn

[P01] 生成 UUID
来源：http://iu.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://rq.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ni.colortex.cn

JS:   crypto.randomUUID()
来源：http://po.newstarts.cn

TS:   crypto.randomUUID()
来源：http://tf.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://rf.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://fz.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://yq.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ze.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ui.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fl.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://om.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dm.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hj.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://by.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://od.nszjky.cn


<!-- 参考信息 -->