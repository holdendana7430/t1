代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wg.hahajie.cn

[L04] 设置超时
来源：http://li.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://dm.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bm.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ul.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wy.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uk.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://si.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ph.asd995.cn

[L05] 上传文件（multipart）
来源：http://fi.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pb.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yi.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ix.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rv.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zx.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hr.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ix.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qn.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://kk.521024.cn

Py:   resp.json()
来源：http://xe.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://kv.nicolike.cn

JS:   await resp.json()
来源：http://wf.wgjwhj.cn

TS:   await resp.json()
来源：http://hx.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gh.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qg.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://lw.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xv.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://ig.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cy.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ia.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://kx.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://as.chemitech.net.cn

Java: resp.statusCode()
来源：http://sp.shxzukj.cn

Go:   resp.StatusCode
来源：http://fd.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://br.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://sw.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://nl.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ij.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://al.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mt.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dx.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ne.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://um.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jx.hnjuh.cn

================================================================================
来源：http://ye.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://yk.huixinmuqiang.cn

================================================================================
来源：http://mm.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://wf.shxzskj.cn

Py:   sys.argv[1:]
来源：http://qq.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://bq.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://kc.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://vv.asd995.cn

Java: args 数组（main 方法参数）
来源：http://hq.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://px.9csxet.cn

Ruby: ARGV
来源：http://ln.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://qg.nicolike.cn

[M02] 读取环境变量
来源：http://nb.colortex.cn

Py:   os.environ.get("HOME")
来源：http://rk.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xg.nicolike.cn

JS:   process.env.HOME
来源：http://co.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://xm.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ho.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sh.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://dt.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://um.asd995.cn

[M03] 执行外部命令
来源：http://qw.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zh.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wc.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ld.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ss.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dg.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pu.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uc.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://rh.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://qb.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://dx.jctech888.com.cn

PHP:  getcwd();
来源：http://fo.nicolike.cn

JS:   process.cwd()
来源：http://qx.haigaiapp.cn

TS:   process.cwd()
来源：http://yb.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ql.hahajie.cn

Go:   os.Getwd()
来源：http://ap.jctech888.com.cn

Ruby: Dir.pwd
来源：http://lf.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fm.gzmigu.cn

[M05] 设置退出码
来源：http://mf.newstarts.cn

Py:   sys.exit(1)
来源：http://me.lnxyls.cn

PHP:  exit(1);
来源：http://gc.szxytkj.cn

JS:   process.exit(1)
来源：http://id.muxihuayi.cn

TS:   process.exit(1)
来源：http://gu.chemitech.net.cn

Java: System.exit(1)
来源：http://te.huanxung.cn

Go:   os.Exit(1)
来源：http://jd.shxzskj.cn

Ruby: exit 1
来源：http://rv.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kr.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://xj.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://vk.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sw.chemitech.net.cn

JS:   console.error("err")
来源：http://rh.nicolike.cn

TS:   console.error("err")
来源：http://ba.huanxung.cn

Java: System.err.println("err")
来源：http://me.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xd.panjiajie.cn

Ruby: warn "err"
来源：http://al.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://uf.lnxyls.cn

[M07] 判断是否为主入口
来源：http://lm.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://uu.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://en.521024.cn

JS:   require.main === module
来源：http://pv.panjiajie.cn

TS:   require.main === module
来源：http://zf.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://dd.newstarts.cn

Go:   func main()
来源：http://vr.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://so.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://oa.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ph.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://oi.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://pi.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://ll.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://pj.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://do.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qw.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://id.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://on.hnjuh.cn

================================================================================
来源：http://pl.muxihuayi.cn

N. 数据结构与算法
来源：http://dt.gzmigu.cn

================================================================================
来源：http://ql.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://om.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sw.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pt.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uv.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cp.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://tm.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nu.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wk.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://zx.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ct.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dm.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yv.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xg.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ou.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://zg.gzmigu.cn

Ruby: arr.sort
来源：http://qj.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gz.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://mk.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yd.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://pi.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oh.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://al.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bg.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vs.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://do.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fo.lnxyls.cn

[N04] 斐波那契数列
来源：http://kl.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kp.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kd.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vv.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fx.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://op.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://af.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eu.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rg.nszjky.cn

[N05] 最大公约数
来源：http://ck.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://kj.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://by.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ra.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pd.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uo.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ql.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://mv.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vm.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://pr.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ml.szsharing.cn

PHP:  $s === strrev($s);
来源：http://su.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://kn.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://ux.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zd.521024.cn

Go:   // 双指针从两端比较
来源：http://os.521024.cn

Ruby: s == s.reverse
来源：http://dj.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://if.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://jm.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ff.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ao.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://al.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://bk.chemitech.net.cn

Java: // 手写 HashMap
来源：http://em.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://xx.521024.cn

Ruby: // 手写 Hash
来源：http://ma.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wd.colortex.cn

[N08] 生成全排列
来源：http://ki.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ek.9csxet.cn

PHP:  // 手写递归交换
来源：http://qx.szxytkj.cn

JS:   // 手写回溯递归
来源：http://jm.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://lp.9csxet.cn

Java: // 手写回溯递归
来源：http://mc.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ts.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ew.newstarts.cn

C#:   // 手写回溯递归
来源：http://jm.jctech888.com.cn

[N09] 栈与队列
来源：http://en.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://un.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vc.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kj.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ie.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lp.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ou.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rt.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qc.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://lw.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dc.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sq.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oe.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://je.colortex.cn

Java: class Node { int v; Node next; }
来源：http://nu.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pe.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cg.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uc.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://xo.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wv.colortex.cn

PHP:  // 手写递归函数
来源：http://ep.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://za.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sb.lnxyls.cn

Java: // 手写递归
来源：http://ig.panjiajie.cn

Go:   // 手写递归
来源：http://sl.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ut.521024.cn

C#:   // 手写递归
来源：http://bq.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://at.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ky.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vv.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ut.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qp.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qr.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ra.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yt.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://br.shtwfgs.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

O. 并发与异步
来源：http://sv.nszjky.cn

================================================================================
来源：http://zp.lnxyls.cn

[O01] 启动一个线程
来源：http://bq.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yi.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hy.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zp.hnjuh.cn

TS:   // 同 JS
来源：http://rz.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://ny.bookmarksfly.cn

Go:   go f()
来源：http://vd.lnxyls.cn

Ruby: Thread.new { f }
来源：http://bh.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://ij.lnxyls.cn

[O02] 使用线程池
来源：http://yu.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://va.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gu.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ek.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://fs.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://af.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mx.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ux.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ev.hahajie.cn

[O03] 加锁保护共享数据
来源：http://hv.521024.cn

Py:   with lock: shared += 1
来源：http://ib.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://re.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qx.nicolike.cn

TS:   // 同 JS
来源：http://zg.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://sv.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://te.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ze.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://jq.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://vo.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://wq.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jl.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://sd.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ra.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kc.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ra.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gu.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://zg.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://yh.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ar.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jo.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://xl.521024.cn

TS:   await Promise.all(tasks)
来源：http://jf.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ga.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hu.nicolike.cn

Ruby: threads.map(&:join)
来源：http://tf.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mz.hnjuh.cn

[O06] 使用进程池
来源：http://xg.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ht.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ah.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://qj.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://ux.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nj.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://su.jctech888.com.cn

Ruby: // fork 块
来源：http://la.hnjuh.cn

C#:   Parallel.For
来源：http://fz.nszjky.cn

================================================================================
来源：http://mp.9csxet.cn

P. 常用工具函数
来源：http://zf.colortex.cn

================================================================================
来源：http://pa.huanxung.cn

[P01] 生成 UUID
来源：http://xg.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://ev.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oj.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://bi.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://xt.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://ji.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://gj.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ri.gzmigu.cn


<!-- 参考信息 -->