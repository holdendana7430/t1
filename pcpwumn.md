代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fe.newstarts.cn

JS:   await fetch(url)
来源：http://qi.chemitech.net.cn

TS:   await fetch(url)
来源：http://fd.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nc.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://lm.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zr.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yy.panjiajie.cn

[L02] 发送 POST JSON
来源：http://jk.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qo.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oj.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ly.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ax.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ji.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mx.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wk.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://np.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://cf.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kn.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pv.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yw.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fa.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zt.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vm.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ml.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ys.jianghongdianzi.cn

[L04] 设置超时
来源：http://kz.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ma.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cj.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wn.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sp.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mv.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://so.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pu.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sx.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ki.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gk.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jd.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mr.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lp.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wy.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cc.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zu.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kr.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://bx.panjiajie.cn

Py:   resp.json()
来源：http://ks.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://nq.nszjky.cn

JS:   await resp.json()
来源：http://kd.szxytkj.cn

TS:   await resp.json()
来源：http://ou.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kg.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jk.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://fz.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ne.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://jb.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uj.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ai.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://io.colortex.cn

TS:   resp.ok;  resp.status
来源：http://oi.yuexingan06.cn

Java: resp.statusCode()
来源：http://qe.hnjuh.cn

Go:   resp.StatusCode
来源：http://de.hnjuh.cn

Ruby: resp.code.to_i
来源：http://ru.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://zp.lnxyls.cn

[L08] 并发请求多个地址
来源：http://ap.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qy.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://bf.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ce.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bd.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jh.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gz.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ej.bjjhwx.cn

================================================================================
来源：http://bs.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://kz.shtwfgs.cn

================================================================================
来源：http://wk.521024.cn

[M01] 读取命令行参数
来源：http://gt.521024.cn

Py:   sys.argv[1:]
来源：http://xm.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://nl.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://wh.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ms.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://cw.jctech888.com.cn

Go:   os.Args[1:]
来源：http://hu.panjiajie.cn

Ruby: ARGV
来源：http://fd.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://dj.huanxung.cn

[M02] 读取环境变量
来源：http://ew.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://xg.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sq.szsharing.cn

JS:   process.env.HOME
来源：http://hi.hnjuh.cn

TS:   process.env.HOME
来源：http://hj.shxzskj.cn

Java: System.getenv("HOME")
来源：http://rq.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ln.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ah.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sj.huanxung.cn

[M03] 执行外部命令
来源：http://rz.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mo.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ty.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pk.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ba.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gd.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xk.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ut.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://dv.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://kj.panjiajie.cn

Py:   os.getcwd()
来源：http://qa.shxzskj.cn

PHP:  getcwd();
来源：http://hd.huanxung.cn

JS:   process.cwd()
来源：http://ns.9csxet.cn

TS:   process.cwd()
来源：http://mb.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qo.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://xh.gzmigu.cn

Ruby: Dir.pwd
来源：http://ai.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yd.bjjhwx.cn

[M05] 设置退出码
来源：http://du.szsharing.cn

Py:   sys.exit(1)
来源：http://vz.huixiangedu.cn

PHP:  exit(1);
来源：http://tu.nicolike.cn

JS:   process.exit(1)
来源：http://ni.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://lx.yuntaijiaju.cn

Java: System.exit(1)
来源：http://zm.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ql.521024.cn

Ruby: exit 1
来源：http://sd.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kn.bjjhwx.cn

[M06] 向标准错误输出
来源：http://fv.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://zr.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hh.yuntaijiaju.cn

JS:   console.error("err")
来源：http://yr.bjjhwx.cn

TS:   console.error("err")
来源：http://if.szxytkj.cn

Java: System.err.println("err")
来源：http://yu.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ig.jctech888.com.cn

Ruby: warn "err"
来源：http://bk.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://lv.shxzukj.cn

[M07] 判断是否为主入口
来源：http://lc.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://ns.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uz.hnjuh.cn

JS:   require.main === module
来源：http://eq.lnxyls.cn

TS:   require.main === module
来源：http://bn.huanxung.cn

Java: public static void main(String[] args)
来源：http://ng.wgjwhj.cn

Go:   func main()
来源：http://tf.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ha.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://zy.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://mt.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://wo.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://hz.shxzskj.cn

JS:   process.platform;  process.version
来源：http://yi.9csxet.cn

TS:   process.platform;  process.version
来源：http://pi.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ey.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fv.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qa.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://gw.asd995.cn

N. 数据结构与算法
来源：http://vq.shtwfgs.cn

================================================================================
来源：http://mb.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://cq.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tc.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ab.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fl.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nd.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ux.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tm.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xc.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://xt.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lv.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wb.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rb.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zw.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hl.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://js.panjiajie.cn

Ruby: arr.sort
来源：http://xp.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ig.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://nc.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ay.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://rd.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nq.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oe.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lq.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sg.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bf.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aw.huixiangedu.cn

[N04] 斐波那契数列
来源：http://lw.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lx.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wz.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mk.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ql.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eb.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rx.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gb.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ve.9csxet.cn

[N05] 最大公约数
来源：http://lc.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://wa.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xm.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://af.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tz.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fe.hnjuh.cn

Ruby: a.gcd(b)
来源：http://vj.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gm.521024.cn

[N06] 判断回文字符串
来源：http://ic.newstarts.cn

Py:   s == s[::-1]
来源：http://hx.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://na.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://kn.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://ss.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://an.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://nb.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://oi.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tp.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://zg.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uh.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vv.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pc.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://up.hahajie.cn

Java: // 手写 HashMap
来源：http://rl.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://wd.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://bz.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cd.shxzukj.cn

[N08] 生成全排列
来源：http://lt.521024.cn

Py:   itertools.permutations(arr)
来源：http://uf.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://wt.521024.cn

JS:   // 手写回溯递归
来源：http://xh.hahajie.cn

TS:   // 手写回溯递归
来源：http://vs.yuexingan06.cn

Java: // 手写回溯递归
来源：http://cf.asd995.cn

Go:   // 手写回溯递归
来源：http://je.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://ct.szxytkj.cn

C#:   // 手写回溯递归
来源：http://kp.9csxet.cn

[N09] 栈与队列
来源：http://ro.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jl.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ml.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wt.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ma.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qx.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jz.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zj.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xe.nszjky.cn

[N10] 链表节点定义
来源：http://ho.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tm.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vu.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gf.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ck.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://fb.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vq.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://im.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rf.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ad.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://at.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://if.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kz.bjjhwx.cn

Java: // 手写递归
来源：http://zl.shxzukj.cn

Go:   // 手写递归
来源：http://bg.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yx.shxzskj.cn

C#:   // 手写递归
来源：http://gv.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oq.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://al.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ns.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rl.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gi.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hv.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ge.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ef.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nj.yuexingan06.cn

================================================================================
来源：http://it.hnjuh.cn

O. 并发与异步
来源：http://vc.szxytkj.cn

================================================================================
来源：http://sn.szxytkj.cn

[O01] 启动一个线程
来源：http://jy.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pd.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vx.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zc.jianghongdianzi.cn

TS:   // 同 JS
来源：http://uc.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://nf.yuntaijiaju.cn

Go:   go f()
来源：http://dk.asd995.cn

Ruby: Thread.new { f }
来源：http://ef.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://lk.szsharing.cn

[O02] 使用线程池
来源：http://jx.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vn.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fx.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://bf.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://sx.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://py.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bg.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hc.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mx.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://di.nicolike.cn

Py:   with lock: shared += 1
来源：http://lp.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://kz.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pq.szsharing.cn

TS:   // 同 JS
来源：http://rv.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://kv.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tc.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oc.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://fb.nicolike.cn

[O04] 定义异步函数并等待
来源：http://tq.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://ln.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ln.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://eh.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yq.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rt.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wo.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://py.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://bf.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://el.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://wp.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kw.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://nf.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://fc.hahajie.cn


<!-- 参考信息 -->