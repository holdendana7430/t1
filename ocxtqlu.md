代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lw.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ps.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lf.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ft.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mr.shxzskj.cn

[L04] 设置超时
来源：http://of.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://wf.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://et.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ra.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ij.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cu.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sb.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pf.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dv.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://if.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ju.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lh.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eu.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xn.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://km.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fv.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://ms.wgjwhj.cn

Py:   resp.json()
来源：http://vv.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://ls.521024.cn

JS:   await resp.json()
来源：http://vz.yuntaijiaju.cn

TS:   await resp.json()
来源：http://hc.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://do.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vv.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://xx.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tj.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://dh.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vc.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gc.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://qt.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://ob.muxihuayi.cn

Java: resp.statusCode()
来源：http://yu.asd995.cn

Go:   resp.StatusCode
来源：http://xl.szxytkj.cn

Ruby: resp.code.to_i
来源：http://qn.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://bv.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://zr.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ya.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://qb.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ms.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ib.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uh.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rv.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jp.huanxung.cn

================================================================================
来源：http://ne.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://qi.yuexingan06.cn

================================================================================
来源：http://zj.chemitech.net.cn

[M01] 读取命令行参数
来源：http://de.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ka.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://vs.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://jy.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://cd.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://th.jctech888.com.cn

Go:   os.Args[1:]
来源：http://uw.yuntaijiaju.cn

Ruby: ARGV
来源：http://uy.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://kn.panjiajie.cn

[M02] 读取环境变量
来源：http://jf.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://ce.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rx.shxzukj.cn

JS:   process.env.HOME
来源：http://po.shxzskj.cn

TS:   process.env.HOME
来源：http://ep.panjiajie.cn

Java: System.getenv("HOME")
来源：http://fc.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cm.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://hr.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://am.bjjhwx.cn

[M03] 执行外部命令
来源：http://wb.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fc.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mj.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ne.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hq.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vl.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nr.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zy.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://wf.colortex.cn

[M04] 获取当前工作目录
来源：http://dg.shxzskj.cn

Py:   os.getcwd()
来源：http://zv.shxzskj.cn

PHP:  getcwd();
来源：http://by.muxihuayi.cn

JS:   process.cwd()
来源：http://tc.bjjhwx.cn

TS:   process.cwd()
来源：http://ii.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://wd.lnxyls.cn

Go:   os.Getwd()
来源：http://qw.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ue.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ro.shtwfgs.cn

[M05] 设置退出码
来源：http://md.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://pg.bookmarksfly.cn

PHP:  exit(1);
来源：http://pt.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ky.shtwfgs.cn

TS:   process.exit(1)
来源：http://ry.szsharing.cn

Java: System.exit(1)
来源：http://sd.hahajie.cn

Go:   os.Exit(1)
来源：http://mz.gzmigu.cn

Ruby: exit 1
来源：http://yo.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wn.nicolike.cn

[M06] 向标准错误输出
来源：http://no.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://tn.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vn.szxytkj.cn

JS:   console.error("err")
来源：http://wr.huixinmuqiang.cn

TS:   console.error("err")
来源：http://fi.wgjwhj.cn

Java: System.err.println("err")
来源：http://ii.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.bjjhwx.cn

Ruby: warn "err"
来源：http://vf.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://oc.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://sr.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://dm.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lh.huanxung.cn

JS:   require.main === module
来源：http://jq.lnxyls.cn

TS:   require.main === module
来源：http://ta.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://iz.szxytkj.cn

Go:   func main()
来源：http://yx.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://of.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://gv.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://vx.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://sj.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://vl.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://sx.nicolike.cn

TS:   process.platform;  process.version
来源：http://st.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://al.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ur.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://po.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ps.newstarts.cn

================================================================================
来源：http://mo.szsharing.cn

N. 数据结构与算法
来源：http://vb.wgjwhj.cn

================================================================================
来源：http://yl.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://xf.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mf.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://od.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dd.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pl.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wo.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://jf.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yb.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nj.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://fk.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://xv.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qu.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bz.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oe.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xp.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ob.haigaiapp.cn

Ruby: arr.sort
来源：http://wj.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hr.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://bu.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mt.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://uh.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nh.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lw.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kt.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tn.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bz.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eq.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://st.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qh.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://au.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kj.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rk.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zs.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fm.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gc.lnxyls.cn

[N05] 最大公约数
来源：http://rd.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://ge.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://co.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ea.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ob.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dp.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://md.colortex.cn

Ruby: a.gcd(b)
来源：http://us.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qw.shtwfgs.cn

[N06] 判断回文字符串
来源：http://vc.newstarts.cn

Py:   s == s[::-1]
来源：http://zh.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://lu.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://no.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://yd.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://so.colortex.cn

Go:   // 双指针从两端比较
来源：http://gv.bjjhwx.cn

Ruby: s == s.reverse
来源：http://qc.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zf.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://ux.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ps.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gw.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://or.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://rx.gzmigu.cn

Java: // 手写 HashMap
来源：http://zm.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://mi.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://zp.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xo.nszjky.cn

[N08] 生成全排列
来源：http://ri.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://dm.szxytkj.cn

PHP:  // 手写递归交换
来源：http://bd.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://jq.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://az.nszjky.cn

Java: // 手写回溯递归
来源：http://vi.shxzskj.cn

Go:   // 手写回溯递归
来源：http://bo.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://wi.shxzskj.cn

C#:   // 手写回溯递归
来源：http://td.huanxung.cn

[N09] 栈与队列
来源：http://io.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sz.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eg.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xn.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pf.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ea.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xi.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zs.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://av.newstarts.cn

[N10] 链表节点定义
来源：http://re.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ma.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nm.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://in.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cp.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://vj.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qt.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pk.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ra.9csxet.cn

[N11] 二叉树中序遍历
来源：http://eu.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jq.colortex.cn

PHP:  // 手写递归函数
来源：http://rm.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://id.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dv.bjjhwx.cn

Java: // 手写递归
来源：http://er.wgjwhj.cn

Go:   // 手写递归
来源：http://uo.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sm.shtwfgs.cn

C#:   // 手写递归
来源：http://qu.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kz.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://on.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yw.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fi.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lp.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nw.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qr.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lb.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://td.gzmigu.cn

================================================================================
来源：http://pw.huixinmuqiang.cn

O. 并发与异步
来源：http://gr.bjjhwx.cn

================================================================================
来源：http://xa.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://to.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://un.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tr.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wa.shxzskj.cn

TS:   // 同 JS
来源：http://fg.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://yq.wgjwhj.cn

Go:   go f()
来源：http://sj.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ps.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://wp.szxytkj.cn

[O02] 使用线程池
来源：http://zk.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dj.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mx.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ky.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://vr.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lx.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ao.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wr.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://op.huanxung.cn

[O03] 加锁保护共享数据
来源：http://gp.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://ny.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://fx.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qo.huixiangedu.cn

TS:   // 同 JS
来源：http://df.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://dh.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dh.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bv.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://ed.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://rx.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ez.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rd.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://vz.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xs.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fj.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://al.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bz.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://la.521024.cn

[O05] 并发执行并等待全部完成
来源：http://nh.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://mp.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tj.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://na.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://sv.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yy.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oj.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://hg.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kz.wgjwhj.cn

[O06] 使用进程池
来源：http://zy.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pt.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ff.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://kd.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://lh.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eb.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wb.gzmigu.cn

Ruby: // fork 块
来源：http://zq.9csxet.cn

C#:   Parallel.For
来源：http://zs.huanxung.cn

================================================================================
来源：http://jm.yuexingan06.cn

P. 常用工具函数
来源：http://ee.muxihuayi.cn

================================================================================
来源：http://hv.colortex.cn

[P01] 生成 UUID
来源：http://bi.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://jx.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://am.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://lv.szsharing.cn


<!-- 参考信息 -->