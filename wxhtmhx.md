代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://il.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://he.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oh.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://bo.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kh.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qu.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fa.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://su.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ee.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bd.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nszjky.cn

[L03] 设置自定义请求头
来源：http://vd.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ye.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iz.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lv.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nr.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cg.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wu.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ob.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eu.huixinmuqiang.cn

[L04] 设置超时
来源：http://gy.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://qw.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ml.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rh.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ln.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rv.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ao.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cl.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://al.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://mi.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qp.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oq.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qj.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qm.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fw.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rw.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vj.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://je.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://kv.panjiajie.cn

Py:   resp.json()
来源：http://vf.9csxet.cn

PHP:  json_decode($body, true);
来源：http://dg.huixinmuqiang.cn

JS:   await resp.json()
来源：http://mb.muxihuayi.cn

TS:   await resp.json()
来源：http://ju.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sn.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://di.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://dr.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yj.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://wl.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rm.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hi.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ri.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://gq.colortex.cn

Java: resp.statusCode()
来源：http://ul.haigaiapp.cn

Go:   resp.StatusCode
来源：http://qa.nicolike.cn

Ruby: resp.code.to_i
来源：http://ul.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://nd.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://dj.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wa.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://ss.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://he.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yv.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zn.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://id.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tr.szxytkj.cn

================================================================================
来源：http://cp.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://rh.gzmigu.cn

================================================================================
来源：http://kw.9csxet.cn

[M01] 读取命令行参数
来源：http://uo.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ux.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://ml.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://mv.colortex.cn

TS:   process.argv.slice(2)
来源：http://gi.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ph.521024.cn

Go:   os.Args[1:]
来源：http://tv.hahajie.cn

Ruby: ARGV
来源：http://tc.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://av.bjjhwx.cn

[M02] 读取环境变量
来源：http://cf.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://cy.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yk.yuexingan06.cn

JS:   process.env.HOME
来源：http://ya.shxzukj.cn

TS:   process.env.HOME
来源：http://ud.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ji.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fx.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://ie.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://en.wgjwhj.cn

[M03] 执行外部命令
来源：http://fa.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qh.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ci.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ah.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://er.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xt.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qe.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pu.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://zc.nszjky.cn

[M04] 获取当前工作目录
来源：http://aw.hahajie.cn

Py:   os.getcwd()
来源：http://qi.panjiajie.cn

PHP:  getcwd();
来源：http://ah.chemitech.net.cn

JS:   process.cwd()
来源：http://bw.shtwfgs.cn

TS:   process.cwd()
来源：http://gx.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://zh.nszjky.cn

Go:   os.Getwd()
来源：http://li.huixiangedu.cn

Ruby: Dir.pwd
来源：http://jz.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hf.lnxyls.cn

[M05] 设置退出码
来源：http://jw.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ph.shxzskj.cn

PHP:  exit(1);
来源：http://cj.lnxyls.cn

JS:   process.exit(1)
来源：http://pz.wgjwhj.cn

TS:   process.exit(1)
来源：http://dy.shtwfgs.cn

Java: System.exit(1)
来源：http://gg.521024.cn

Go:   os.Exit(1)
来源：http://vp.szxytkj.cn

Ruby: exit 1
来源：http://ex.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ga.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ep.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://cy.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nq.hnjuh.cn

JS:   console.error("err")
来源：http://ou.bookmarksfly.cn

TS:   console.error("err")
来源：http://bc.haigaiapp.cn

Java: System.err.println("err")
来源：http://ak.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://de.muxihuayi.cn

Ruby: warn "err"
来源：http://is.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://wa.hahajie.cn

[M07] 判断是否为主入口
来源：http://cr.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ad.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nc.hahajie.cn

JS:   require.main === module
来源：http://wr.9csxet.cn

TS:   require.main === module
来源：http://ll.panjiajie.cn

Java: public static void main(String[] args)
来源：http://md.szsharing.cn

Go:   func main()
来源：http://tn.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tt.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://kb.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://pc.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://sy.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://rm.szsharing.cn

JS:   process.platform;  process.version
来源：http://mw.shxzukj.cn

TS:   process.platform;  process.version
来源：http://cv.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sc.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jc.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fu.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vp.szxytkj.cn

================================================================================
来源：http://wt.huixiangedu.cn

N. 数据结构与算法
来源：http://gr.bookmarksfly.cn

================================================================================
来源：http://fv.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://jb.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pb.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xl.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://et.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ab.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qk.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://sj.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qe.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://it.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://ij.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ku.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ce.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kf.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zo.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://gw.huanxung.cn

Ruby: arr.sort
来源：http://qp.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gn.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://ng.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ms.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://bp.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tm.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eb.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jg.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fo.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jv.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sh.szxytkj.cn

[N04] 斐波那契数列
来源：http://vu.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ek.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jq.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jd.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lx.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ml.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://je.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jt.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fh.bjjhwx.cn

[N05] 最大公约数
来源：http://ua.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://cc.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gd.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tk.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ok.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qd.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jx.huanxung.cn

Ruby: a.gcd(b)
来源：http://az.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rt.panjiajie.cn

[N06] 判断回文字符串
来源：http://lj.shtwfgs.cn

Py:   s == s[::-1]
来源：http://za.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://gu.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://cr.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://bs.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mi.nicolike.cn

Go:   // 双指针从两端比较
来源：http://em.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ak.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vd.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://fi.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yk.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xz.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gv.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://wq.szsharing.cn

Java: // 手写 HashMap
来源：http://mk.nicolike.cn

Go:   // 手写 map[int]int
来源：http://xv.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://jt.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ye.asd995.cn

[N08] 生成全排列
来源：http://fq.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ap.szxytkj.cn

PHP:  // 手写递归交换
来源：http://am.lnxyls.cn

JS:   // 手写回溯递归
来源：http://fb.nicolike.cn

TS:   // 手写回溯递归
来源：http://ki.hnjuh.cn

Java: // 手写回溯递归
来源：http://tf.newstarts.cn

Go:   // 手写回溯递归
来源：http://fq.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://ta.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://fy.hnjuh.cn

[N09] 栈与队列
来源：http://gh.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zu.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ck.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://js.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vk.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qg.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gw.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fr.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ds.hahajie.cn

[N10] 链表节点定义
来源：http://yk.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cu.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nf.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nh.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xc.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://sk.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ax.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sr.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://up.nszjky.cn

[N11] 二叉树中序遍历
来源：http://bb.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sp.nicolike.cn

PHP:  // 手写递归函数
来源：http://md.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nn.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zt.9csxet.cn

Java: // 手写递归
来源：http://qm.521024.cn

Go:   // 手写递归
来源：http://fv.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pa.shxzukj.cn

C#:   // 手写递归
来源：http://oq.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jh.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qu.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://we.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fz.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bk.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fr.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yg.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pt.wgjwhj.cn

================================================================================
来源：http://lq.colortex.cn

O. 并发与异步
来源：http://qu.chemitech.net.cn

================================================================================
来源：http://jk.nszjky.cn

[O01] 启动一个线程
来源：http://mc.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sl.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mk.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pp.huixiangedu.cn

TS:   // 同 JS
来源：http://qh.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://ag.szsharing.cn

Go:   go f()
来源：http://gw.asd995.cn

Ruby: Thread.new { f }
来源：http://hi.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://vm.colortex.cn

[O02] 使用线程池
来源：http://hz.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ri.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gy.newstarts.cn

JS:   // worker_threads 线程池
来源：http://kw.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://pa.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aa.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kz.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lg.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dk.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://xt.521024.cn

Py:   with lock: shared += 1
来源：http://im.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://zs.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gy.szsharing.cn

TS:   // 同 JS
来源：http://jo.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://jp.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ex.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yz.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://gx.huanxung.cn

[O04] 定义异步函数并等待
来源：http://by.asd995.cn

Py:   async def f():⏎    await g()
来源：http://qc.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hj.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://oj.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cs.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dv.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vo.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ia.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://ny.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://kt.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://bh.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uy.521024.cn

JS:   await Promise.all(tasks)
来源：http://pj.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://es.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ki.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nw.hahajie.cn

Ruby: threads.map(&:join)
来源：http://uw.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kb.asd995.cn


<!-- 参考信息 -->