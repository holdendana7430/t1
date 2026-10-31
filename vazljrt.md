代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nd.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ua.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://el.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tl.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cg.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gh.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://go.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://py.nszjky.cn

[L04] 设置超时
来源：http://pi.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://wc.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qd.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ue.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kg.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zl.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bx.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ys.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://dr.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xy.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sy.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wq.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sz.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eo.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zb.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://th.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hd.nicolike.cn

[L06] 解析响应为 JSON
来源：http://rs.huixinmuqiang.cn

Py:   resp.json()
来源：http://ze.hahajie.cn

PHP:  json_decode($body, true);
来源：http://uz.asd995.cn

JS:   await resp.json()
来源：http://gk.yuexingan06.cn

TS:   await resp.json()
来源：http://hm.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qt.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ob.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://kb.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qa.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://hx.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yh.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fn.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://is.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://hh.shxzukj.cn

Java: resp.statusCode()
来源：http://ji.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://hr.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://tn.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://oe.gzmigu.cn

[L08] 并发请求多个地址
来源：http://vn.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vc.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://jh.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nt.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eg.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yd.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wj.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gt.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zb.nszjky.cn

================================================================================
来源：http://cg.521024.cn

M. 命令行 / 进程 / 环境
来源：http://de.shtwfgs.cn

================================================================================
来源：http://ua.hnjuh.cn

[M01] 读取命令行参数
来源：http://wo.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://gl.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://zu.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://wq.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://qz.521024.cn

Java: args 数组（main 方法参数）
来源：http://ga.szxytkj.cn

Go:   os.Args[1:]
来源：http://rq.gzmigu.cn

Ruby: ARGV
来源：http://ul.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://uv.jctech888.com.cn

[M02] 读取环境变量
来源：http://dd.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://ki.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eb.nicolike.cn

JS:   process.env.HOME
来源：http://an.huanxung.cn

TS:   process.env.HOME
来源：http://vz.shxzskj.cn

Java: System.getenv("HOME")
来源：http://de.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ef.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://va.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rm.szxytkj.cn

[M03] 执行外部命令
来源：http://as.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ii.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zu.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cr.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vx.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ot.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ar.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vc.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://po.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://fy.szxytkj.cn

Py:   os.getcwd()
来源：http://ca.colortex.cn

PHP:  getcwd();
来源：http://cg.szsharing.cn

JS:   process.cwd()
来源：http://of.haigaiapp.cn

TS:   process.cwd()
来源：http://gq.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://df.panjiajie.cn

Go:   os.Getwd()
来源：http://on.nszjky.cn

Ruby: Dir.pwd
来源：http://yj.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wf.nicolike.cn

[M05] 设置退出码
来源：http://wk.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://zm.yuexingan06.cn

PHP:  exit(1);
来源：http://xn.gzmigu.cn

JS:   process.exit(1)
来源：http://pw.nszjky.cn

TS:   process.exit(1)
来源：http://tp.bookmarksfly.cn

Java: System.exit(1)
来源：http://kg.haigaiapp.cn

Go:   os.Exit(1)
来源：http://kr.colortex.cn

Ruby: exit 1
来源：http://fp.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.szxytkj.cn

[M06] 向标准错误输出
来源：http://ll.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://qr.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wi.shxzukj.cn

JS:   console.error("err")
来源：http://cd.newstarts.cn

TS:   console.error("err")
来源：http://ob.chemitech.net.cn

Java: System.err.println("err")
来源：http://rc.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hi.wgjwhj.cn

Ruby: warn "err"
来源：http://sm.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.9csxet.cn

[M07] 判断是否为主入口
来源：http://ae.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://xn.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://li.colortex.cn

JS:   require.main === module
来源：http://su.huanxung.cn

TS:   require.main === module
来源：http://po.hnjuh.cn

Java: public static void main(String[] args)
来源：http://xo.shxzskj.cn

Go:   func main()
来源：http://wz.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rz.nszjky.cn

C#:   static void Main(string[] args)
来源：http://hl.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://tm.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://qg.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ab.shxzskj.cn

JS:   process.platform;  process.version
来源：http://dw.asd995.cn

TS:   process.platform;  process.version
来源：http://bm.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hr.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ge.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ze.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://si.muxihuayi.cn

================================================================================
来源：http://xj.szsharing.cn

N. 数据结构与算法
来源：http://as.huixinmuqiang.cn

================================================================================
来源：http://pa.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://rk.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xn.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nf.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gr.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://he.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xb.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://eg.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ms.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sx.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://qt.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://vj.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ia.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aj.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ti.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ne.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://ee.gzmigu.cn

Ruby: arr.sort
来源：http://aa.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mo.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://ni.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ws.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://pu.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ob.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eq.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kr.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ly.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qf.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yt.asd995.cn

[N04] 斐波那契数列
来源：http://mm.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xq.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jg.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hw.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lx.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bk.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eu.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://as.shxzskj.cn

[N05] 最大公约数
来源：http://sp.newstarts.cn

Py:   math.gcd(a, b)
来源：http://cf.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aj.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tz.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lw.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pg.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ue.szsharing.cn

Ruby: a.gcd(b)
来源：http://gd.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kw.chemitech.net.cn

[N06] 判断回文字符串
来源：http://et.nicolike.cn

Py:   s == s[::-1]
来源：http://hf.nszjky.cn

PHP:  $s === strrev($s);
来源：http://dw.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://oq.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ex.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dx.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://fc.wgjwhj.cn

Ruby: s == s.reverse
来源：http://pm.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fb.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://ih.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lq.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mv.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ar.521024.cn

TS:   // 手写 Map<string, number>
来源：http://uo.lnxyls.cn

Java: // 手写 HashMap
来源：http://bi.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://dt.nszjky.cn

Ruby: // 手写 Hash
来源：http://vm.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sx.newstarts.cn

[N08] 生成全排列
来源：http://gi.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://sp.9csxet.cn

PHP:  // 手写递归交换
来源：http://xc.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://dh.hnjuh.cn

TS:   // 手写回溯递归
来源：http://yb.colortex.cn

Java: // 手写回溯递归
来源：http://lp.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://sb.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://lr.hnjuh.cn

C#:   // 手写回溯递归
来源：http://wu.nicolike.cn

[N09] 栈与队列
来源：http://gb.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lj.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xi.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xy.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jd.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yf.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ic.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hh.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zs.muxihuayi.cn

[N10] 链表节点定义
来源：http://rs.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ap.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ii.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://df.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ia.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://ry.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ft.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iu.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bu.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://yr.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://su.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://wl.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ep.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ga.521024.cn

Java: // 手写递归
来源：http://kf.bookmarksfly.cn

Go:   // 手写递归
来源：http://dm.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xu.nszjky.cn

C#:   // 手写递归
来源：http://hm.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wj.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ut.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://af.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://um.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ot.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xh.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zn.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wy.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lp.yuntaijiaju.cn

================================================================================
来源：http://qv.wgjwhj.cn

O. 并发与异步
来源：http://cq.jctech888.com.cn

================================================================================
来源：http://ch.hnjuh.cn

[O01] 启动一个线程
来源：http://ep.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ak.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jd.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ic.nszjky.cn

TS:   // 同 JS
来源：http://gj.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://th.panjiajie.cn

Go:   go f()
来源：http://oh.asd995.cn

Ruby: Thread.new { f }
来源：http://cm.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://bi.jctech888.com.cn

[O02] 使用线程池
来源：http://ya.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lx.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sm.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://tm.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://oz.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fc.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fc.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lx.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xu.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://ww.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://ri.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://lq.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ql.haigaiapp.cn

TS:   // 同 JS
来源：http://gm.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://lo.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qo.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yp.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://ti.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://ra.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ra.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oz.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ii.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dm.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ze.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pk.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ol.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://tq.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://up.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://wd.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rl.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://se.colortex.cn

TS:   await Promise.all(tasks)
来源：http://ks.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ie.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yr.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://qu.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xv.9csxet.cn

[O06] 使用进程池
来源：http://oc.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cj.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zn.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://rg.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ck.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fk.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://za.yuexingan06.cn

Ruby: // fork 块
来源：http://bx.shxzukj.cn

C#:   Parallel.For
来源：http://id.colortex.cn

================================================================================
来源：http://kw.9csxet.cn

P. 常用工具函数
来源：http://tz.asd995.cn

================================================================================
来源：http://cg.newstarts.cn


<!-- 参考信息 -->