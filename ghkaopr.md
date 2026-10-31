代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gn.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ux.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nn.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ti.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ds.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://wd.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ng.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://la.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yz.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kw.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gc.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yz.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zx.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://ho.newstarts.cn

Py:   resp.json()
来源：http://vb.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://sn.haigaiapp.cn

JS:   await resp.json()
来源：http://sj.huixinmuqiang.cn

TS:   await resp.json()
来源：http://jq.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yy.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zm.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://fr.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qu.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://qe.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fg.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kg.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://pm.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://my.asd995.cn

Java: resp.statusCode()
来源：http://mv.9csxet.cn

Go:   resp.StatusCode
来源：http://dr.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://lz.521024.cn

C#:   (int)resp.StatusCode
来源：http://jv.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://py.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://so.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://bb.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zc.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hd.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zb.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yw.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xn.shxzukj.cn

================================================================================
来源：http://qk.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://dm.gzmigu.cn

================================================================================
来源：http://ab.521024.cn

[M01] 读取命令行参数
来源：http://ah.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ii.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://vc.nicolike.cn

JS:   process.argv.slice(2)
来源：http://vs.newstarts.cn

TS:   process.argv.slice(2)
来源：http://sc.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://kq.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://eb.chemitech.net.cn

Ruby: ARGV
来源：http://kg.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://so.huixiangedu.cn

[M02] 读取环境变量
来源：http://qr.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://jf.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ic.521024.cn

JS:   process.env.HOME
来源：http://lm.gzmigu.cn

TS:   process.env.HOME
来源：http://tr.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ua.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dn.huanxung.cn

Ruby: ENV["HOME"]
来源：http://fd.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zq.wgjwhj.cn

[M03] 执行外部命令
来源：http://dq.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cb.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uf.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vz.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kx.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kh.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://po.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xh.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://jl.asd995.cn

[M04] 获取当前工作目录
来源：http://ma.muxihuayi.cn

Py:   os.getcwd()
来源：http://ck.panjiajie.cn

PHP:  getcwd();
来源：http://ke.shtwfgs.cn

JS:   process.cwd()
来源：http://xe.bjjhwx.cn

TS:   process.cwd()
来源：http://ia.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ln.lnxyls.cn

Go:   os.Getwd()
来源：http://xs.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://vu.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jb.muxihuayi.cn

[M05] 设置退出码
来源：http://yw.jctech888.com.cn

Py:   sys.exit(1)
来源：http://gw.bookmarksfly.cn

PHP:  exit(1);
来源：http://jt.huixiangedu.cn

JS:   process.exit(1)
来源：http://zc.521024.cn

TS:   process.exit(1)
来源：http://na.shtwfgs.cn

Java: System.exit(1)
来源：http://qe.hnjuh.cn

Go:   os.Exit(1)
来源：http://db.wgjwhj.cn

Ruby: exit 1
来源：http://el.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://es.huixiangedu.cn

[M06] 向标准错误输出
来源：http://wy.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://cc.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kn.asd995.cn

JS:   console.error("err")
来源：http://jd.yuexingan06.cn

TS:   console.error("err")
来源：http://mt.jctech888.com.cn

Java: System.err.println("err")
来源：http://vv.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rb.nicolike.cn

Ruby: warn "err"
来源：http://gv.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ol.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://np.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://kp.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sf.muxihuayi.cn

JS:   require.main === module
来源：http://xx.muxihuayi.cn

TS:   require.main === module
来源：http://ro.szsharing.cn

Java: public static void main(String[] args)
来源：http://kw.shxzukj.cn

Go:   func main()
来源：http://ky.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pv.nszjky.cn

C#:   static void Main(string[] args)
来源：http://gi.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://jh.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://hz.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://ej.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://lq.newstarts.cn

TS:   process.platform;  process.version
来源：http://nz.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tq.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qa.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sk.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fp.nicolike.cn

================================================================================
来源：http://or.huixiangedu.cn

N. 数据结构与算法
来源：http://wp.muxihuayi.cn

================================================================================
来源：http://as.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://zm.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rq.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kz.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ea.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rq.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://kd.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qp.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eq.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://ll.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://il.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xh.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mj.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mk.9csxet.cn

Go:   slices.Sort(arr)
来源：http://yp.chemitech.net.cn

Ruby: arr.sort
来源：http://np.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wl.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://zt.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xk.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://iv.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vp.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zd.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ux.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vh.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pu.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uk.yuexingan06.cn

[N04] 斐波那契数列
来源：http://vd.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://im.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ps.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sn.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zb.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pq.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tk.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ge.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jy.521024.cn

[N05] 最大公约数
来源：http://wz.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ud.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rl.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ae.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nr.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ha.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ow.nszjky.cn

Ruby: a.gcd(b)
来源：http://fs.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bs.haigaiapp.cn

[N06] 判断回文字符串
来源：http://hm.521024.cn

Py:   s == s[::-1]
来源：http://ya.huanxung.cn

PHP:  $s === strrev($s);
来源：http://oj.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ak.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ft.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uf.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://kr.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ju.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ry.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://dz.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rw.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ui.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ew.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://xh.bjjhwx.cn

Java: // 手写 HashMap
来源：http://bq.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://kk.lnxyls.cn

Ruby: // 手写 Hash
来源：http://gy.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lw.bookmarksfly.cn

[N08] 生成全排列
来源：http://db.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://nu.nicolike.cn

PHP:  // 手写递归交换
来源：http://cm.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://dl.gzmigu.cn

TS:   // 手写回溯递归
来源：http://wi.521024.cn

Java: // 手写回溯递归
来源：http://wo.szsharing.cn

Go:   // 手写回溯递归
来源：http://ok.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://rs.panjiajie.cn

C#:   // 手写回溯递归
来源：http://df.hnjuh.cn

[N09] 栈与队列
来源：http://fp.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ki.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lw.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cg.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tb.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nf.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://or.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mg.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bc.hnjuh.cn

[N10] 链表节点定义
来源：http://ti.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gz.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dx.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lo.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pb.521024.cn

Java: class Node { int v; Node next; }
来源：http://xd.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tv.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kl.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://tk.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hv.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://is.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://li.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vo.lnxyls.cn

Java: // 手写递归
来源：http://ag.521024.cn

Go:   // 手写递归
来源：http://em.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mz.muxihuayi.cn

C#:   // 手写递归
来源：http://gd.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wl.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://io.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ju.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cv.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ap.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sk.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pd.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hd.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ez.nicolike.cn

================================================================================
来源：http://bj.panjiajie.cn

O. 并发与异步
来源：http://gb.yuexingan06.cn

================================================================================
来源：http://tl.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://zy.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uk.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ra.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zk.colortex.cn

TS:   // 同 JS
来源：http://ym.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://cr.chemitech.net.cn

Go:   go f()
来源：http://mt.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://ts.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://fa.huixinmuqiang.cn

[O02] 使用线程池
来源：http://xk.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wr.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eb.521024.cn

JS:   // worker_threads 线程池
来源：http://mh.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://es.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yp.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pt.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rq.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://in.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://pv.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://jz.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://np.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://op.nszjky.cn

TS:   // 同 JS
来源：http://xw.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://tl.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tj.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iz.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://vu.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://yv.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ay.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wu.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://fa.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pv.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ol.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://we.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wy.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://te.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://lz.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://cv.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yx.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://yv.colortex.cn

TS:   await Promise.all(tasks)
来源：http://lb.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tn.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hy.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://yk.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lz.521024.cn

[O06] 使用进程池
来源：http://fc.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ry.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xo.colortex.cn

JS:   // child_process / cluster 模块
来源：http://jd.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://xl.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ft.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iu.yuntaijiaju.cn

Ruby: // fork 块
来源：http://az.muxihuayi.cn

C#:   Parallel.For
来源：http://sv.nszjky.cn

================================================================================
来源：http://wa.chemitech.net.cn

P. 常用工具函数
来源：http://ji.chemitech.net.cn

================================================================================
来源：http://er.hnjuh.cn

[P01] 生成 UUID
来源：http://my.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://zr.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wc.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ji.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://ur.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://ix.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://hv.521024.cn

Ruby: SecureRandom.uuid
来源：http://se.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://yy.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://jl.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ih.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ad.wgjwhj.cn


<!-- 参考信息 -->