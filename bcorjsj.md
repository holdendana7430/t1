代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ve.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mx.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rb.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vh.521024.cn

[L03] 设置自定义请求头
来源：http://vp.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mu.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bi.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mi.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kc.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fi.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wg.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ox.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iv.bjjhwx.cn

[L04] 设置超时
来源：http://jq.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://sz.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ey.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ow.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wo.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bw.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://et.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://in.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gs.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://nn.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sy.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://he.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wl.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nn.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fd.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dw.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iy.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lj.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://wa.521024.cn

Py:   resp.json()
来源：http://ek.colortex.cn

PHP:  json_decode($body, true);
来源：http://op.nicolike.cn

JS:   await resp.json()
来源：http://jo.shxzskj.cn

TS:   await resp.json()
来源：http://tg.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yf.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gg.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://si.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kj.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://pk.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mv.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jn.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://rz.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://eo.shxzukj.cn

Java: resp.statusCode()
来源：http://wh.hnjuh.cn

Go:   resp.StatusCode
来源：http://jg.nszjky.cn

Ruby: resp.code.to_i
来源：http://vc.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://mw.nszjky.cn

[L08] 并发请求多个地址
来源：http://ye.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ri.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://vz.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tc.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ha.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ds.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ch.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vv.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://js.shxzskj.cn

================================================================================
来源：http://ts.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://mg.colortex.cn

================================================================================
来源：http://lm.panjiajie.cn

[M01] 读取命令行参数
来源：http://ce.hnjuh.cn

Py:   sys.argv[1:]
来源：http://rr.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://mp.huanxung.cn

JS:   process.argv.slice(2)
来源：http://du.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://lb.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://ko.bjjhwx.cn

Go:   os.Args[1:]
来源：http://ka.hahajie.cn

Ruby: ARGV
来源：http://fc.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://se.colortex.cn

[M02] 读取环境变量
来源：http://vm.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://md.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://so.shxzskj.cn

JS:   process.env.HOME
来源：http://eq.bjjhwx.cn

TS:   process.env.HOME
来源：http://oo.nszjky.cn

Java: System.getenv("HOME")
来源：http://ie.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qv.521024.cn

Ruby: ENV["HOME"]
来源：http://lq.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ie.shxzskj.cn

[M03] 执行外部命令
来源：http://db.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ul.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fy.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ax.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ug.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pf.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ft.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qs.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://yv.nszjky.cn

[M04] 获取当前工作目录
来源：http://ib.haigaiapp.cn

Py:   os.getcwd()
来源：http://yn.jctech888.com.cn

PHP:  getcwd();
来源：http://pv.jctech888.com.cn

JS:   process.cwd()
来源：http://zb.nszjky.cn

TS:   process.cwd()
来源：http://lt.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://fv.bjjhwx.cn

Go:   os.Getwd()
来源：http://pa.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://fd.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jk.szsharing.cn

[M05] 设置退出码
来源：http://ok.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://wc.bookmarksfly.cn

PHP:  exit(1);
来源：http://mb.nicolike.cn

JS:   process.exit(1)
来源：http://tu.shxzskj.cn

TS:   process.exit(1)
来源：http://lq.szxytkj.cn

Java: System.exit(1)
来源：http://pm.szxytkj.cn

Go:   os.Exit(1)
来源：http://nh.colortex.cn

Ruby: exit 1
来源：http://ws.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ei.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://rl.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://lk.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kq.jctech888.com.cn

JS:   console.error("err")
来源：http://ti.bookmarksfly.cn

TS:   console.error("err")
来源：http://iq.shxzukj.cn

Java: System.err.println("err")
来源：http://fx.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjjhwx.cn

Ruby: warn "err"
来源：http://aw.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://kt.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://hg.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://jj.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ep.shxzukj.cn

JS:   require.main === module
来源：http://ux.hnjuh.cn

TS:   require.main === module
来源：http://lb.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://jn.huanxung.cn

Go:   func main()
来源：http://ss.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fr.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://jq.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://fr.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://um.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ly.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://ql.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://bh.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ye.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xl.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iz.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mf.huixinmuqiang.cn

================================================================================
来源：http://je.nicolike.cn

N. 数据结构与算法
来源：http://uj.gzmigu.cn

================================================================================
来源：http://dk.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://ha.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bp.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fz.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ty.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pc.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qb.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://aj.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gq.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cy.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://ho.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://em.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vo.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kw.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sp.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fj.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ma.huanxung.cn

Ruby: arr.sort
来源：http://wv.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://em.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://md.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bg.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ag.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pf.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ww.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gq.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lb.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kj.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bn.shxzskj.cn

[N04] 斐波那契数列
来源：http://ez.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cc.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hn.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dj.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rm.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dv.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://if.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zp.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://un.jianghongdianzi.cn

[N05] 最大公约数
来源：http://zd.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://qd.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://un.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://on.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qo.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kf.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zm.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://dx.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xz.szsharing.cn

[N06] 判断回文字符串
来源：http://ki.gzmigu.cn

Py:   s == s[::-1]
来源：http://xw.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://ow.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://xn.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://mz.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ng.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ya.szxytkj.cn

Ruby: s == s.reverse
来源：http://ee.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xu.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://ji.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fo.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ak.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fa.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://tb.hahajie.cn

Java: // 手写 HashMap
来源：http://xp.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://qj.gzmigu.cn

Ruby: // 手写 Hash
来源：http://ih.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://da.colortex.cn

[N08] 生成全排列
来源：http://ds.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://wr.nszjky.cn

PHP:  // 手写递归交换
来源：http://cb.gzmigu.cn

JS:   // 手写回溯递归
来源：http://cc.colortex.cn

TS:   // 手写回溯递归
来源：http://gb.hnjuh.cn

Java: // 手写回溯递归
来源：http://mu.asd995.cn

Go:   // 手写回溯递归
来源：http://me.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://yl.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://sm.521024.cn

[N09] 栈与队列
来源：http://to.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xo.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mw.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xd.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cn.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bx.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fk.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qg.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wl.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://xh.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qv.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yl.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vb.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wy.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://hb.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pr.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ur.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nt.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://kc.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xk.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://zh.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ly.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hq.asd995.cn

Java: // 手写递归
来源：http://pn.colortex.cn

Go:   // 手写递归
来源：http://ts.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sa.colortex.cn

C#:   // 手写递归
来源：http://wz.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vk.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qt.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ha.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://og.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ci.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bo.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oo.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zx.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fo.newstarts.cn

================================================================================
来源：http://kz.bookmarksfly.cn

O. 并发与异步
来源：http://sz.lnxyls.cn

================================================================================
来源：http://dn.shtwfgs.cn

[O01] 启动一个线程
来源：http://gp.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://et.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://as.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ev.shtwfgs.cn

TS:   // 同 JS
来源：http://ie.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://fb.9csxet.cn

Go:   go f()
来源：http://uw.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://se.colortex.cn

C#:   Task.Run(() => F());
来源：http://do.jianghongdianzi.cn

[O02] 使用线程池
来源：http://er.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bt.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xb.asd995.cn

JS:   // worker_threads 线程池
来源：http://jh.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://sm.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tn.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xx.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yd.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sm.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://jf.hnjuh.cn

Py:   with lock: shared += 1
来源：http://ta.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://jt.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mj.huixinmuqiang.cn

TS:   // 同 JS
来源：http://qn.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://cu.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ve.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rg.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://qc.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://uj.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://wh.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ia.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://fu.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tt.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jg.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://or.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dg.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://kr.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://yf.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://bm.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zv.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://iw.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://dk.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hd.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wt.hahajie.cn

Ruby: threads.map(&:join)
来源：http://si.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qa.haigaiapp.cn

[O06] 使用进程池
来源：http://ha.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sh.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hm.colortex.cn

JS:   // child_process / cluster 模块
来源：http://mt.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://be.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zn.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://im.shxzskj.cn

Ruby: // fork 块
来源：http://vw.shxzskj.cn


<!-- 参考信息 -->