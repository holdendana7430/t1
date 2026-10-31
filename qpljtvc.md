代发 wailian999

Go:   encoding/gob
来源：http://pq.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://gp.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xx.muxihuayi.cn

================================================================================
来源：http://ee.gzmigu.cn

L. 网络请求
来源：http://dl.huixiangedu.cn

================================================================================
来源：http://eo.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://ru.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pe.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://se.wgjwhj.cn

JS:   await fetch(url)
来源：http://fu.huixiangedu.cn

TS:   await fetch(url)
来源：http://jv.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rt.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://zk.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sm.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ns.huanxung.cn

[L02] 发送 POST JSON
来源：http://fi.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qd.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sx.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nh.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mb.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oz.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xu.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ea.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xz.nicolike.cn

[L03] 设置自定义请求头
来源：http://ea.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pn.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jx.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pu.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gl.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cn.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zf.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gn.huixiangedu.cn

[L04] 设置超时
来源：http://qv.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://ci.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://en.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gv.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ec.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eb.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rk.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pe.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iy.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://pu.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sa.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fk.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xg.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yj.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lu.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uu.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qv.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://on.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://an.haigaiapp.cn

Py:   resp.json()
来源：http://zl.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ux.chemitech.net.cn

JS:   await resp.json()
来源：http://ip.shtwfgs.cn

TS:   await resp.json()
来源：http://hn.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dw.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tu.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://fa.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mh.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://cw.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xw.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wl.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://bj.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://gn.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://uj.shtwfgs.cn

Go:   resp.StatusCode
来源：http://rp.nszjky.cn

Ruby: resp.code.to_i
来源：http://fm.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://vr.colortex.cn

[L08] 并发请求多个地址
来源：http://pq.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wr.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://eh.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qs.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iw.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sv.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://do.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sz.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bk.nszjky.cn

================================================================================
来源：http://wr.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://wi.521024.cn

================================================================================
来源：http://gs.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://zs.colortex.cn

Py:   sys.argv[1:]
来源：http://ms.newstarts.cn

PHP:  $argv;  $argc;
来源：http://zb.hahajie.cn

JS:   process.argv.slice(2)
来源：http://wm.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://em.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://pa.szxytkj.cn

Go:   os.Args[1:]
来源：http://ze.panjiajie.cn

Ruby: ARGV
来源：http://ad.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://qd.haigaiapp.cn

[M02] 读取环境变量
来源：http://ou.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://dg.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ot.gzmigu.cn

JS:   process.env.HOME
来源：http://nt.huanxung.cn

TS:   process.env.HOME
来源：http://ri.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://qk.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ci.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://pe.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rk.wgjwhj.cn

[M03] 执行外部命令
来源：http://wk.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://co.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nq.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pb.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gy.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wh.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dy.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ej.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://qd.9csxet.cn

[M04] 获取当前工作目录
来源：http://ta.shxzskj.cn

Py:   os.getcwd()
来源：http://vr.hahajie.cn

PHP:  getcwd();
来源：http://oz.521024.cn

JS:   process.cwd()
来源：http://bz.shxzukj.cn

TS:   process.cwd()
来源：http://fu.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ne.lnxyls.cn

Go:   os.Getwd()
来源：http://ip.huixiangedu.cn

Ruby: Dir.pwd
来源：http://hj.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kb.huanxung.cn

[M05] 设置退出码
来源：http://tl.huixiangedu.cn

Py:   sys.exit(1)
来源：http://vn.asd995.cn

PHP:  exit(1);
来源：http://qa.muxihuayi.cn

JS:   process.exit(1)
来源：http://sh.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://el.szsharing.cn

Java: System.exit(1)
来源：http://zh.lnxyls.cn

Go:   os.Exit(1)
来源：http://bx.bookmarksfly.cn

Ruby: exit 1
来源：http://rc.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lk.chemitech.net.cn

[M06] 向标准错误输出
来源：http://bb.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://rv.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://on.colortex.cn

JS:   console.error("err")
来源：http://vv.yuexingan06.cn

TS:   console.error("err")
来源：http://gf.nszjky.cn

Java: System.err.println("err")
来源：http://nb.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pm.shxzukj.cn

Ruby: warn "err"
来源：http://nx.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://du.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://yo.colortex.cn

Py:   if __name__ == "__main__":
来源：http://ga.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dl.nicolike.cn

JS:   require.main === module
来源：http://fv.yuntaijiaju.cn

TS:   require.main === module
来源：http://ei.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://cj.hahajie.cn

Go:   func main()
来源：http://wq.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sy.colortex.cn

C#:   static void Main(string[] args)
来源：http://ev.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://gg.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://cs.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://fc.asd995.cn

JS:   process.platform;  process.version
来源：http://ot.lnxyls.cn

TS:   process.platform;  process.version
来源：http://mr.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nr.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gi.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://au.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://br.nicolike.cn

================================================================================
来源：http://li.muxihuayi.cn

N. 数据结构与算法
来源：http://my.panjiajie.cn

================================================================================
来源：http://ma.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://xv.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://el.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vs.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mo.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qz.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wa.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://dv.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://db.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ma.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://hp.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://jt.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qz.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://se.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kr.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wt.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://gc.yuntaijiaju.cn

Ruby: arr.sort
来源：http://yq.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qf.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://yu.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cr.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://kr.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ph.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bc.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xa.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cu.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gy.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ka.huanxung.cn

[N04] 斐波那契数列
来源：http://zd.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://le.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jr.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nv.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pw.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mk.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fw.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://li.gzmigu.cn

[N05] 最大公约数
来源：http://kx.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://tk.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://up.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vv.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ov.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gq.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ds.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://kw.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dl.shtwfgs.cn

[N06] 判断回文字符串
来源：http://ib.hahajie.cn

Py:   s == s[::-1]
来源：http://su.hahajie.cn

PHP:  $s === strrev($s);
来源：http://cz.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ub.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ao.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hx.szsharing.cn

Go:   // 双指针从两端比较
来源：http://sd.shtwfgs.cn

Ruby: s == s.reverse
来源：http://hm.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qe.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://ig.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nj.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gd.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ro.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://yk.shxzukj.cn

Java: // 手写 HashMap
来源：http://oh.newstarts.cn

Go:   // 手写 map[int]int
来源：http://gu.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://vq.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iz.newstarts.cn

[N08] 生成全排列
来源：http://kb.asd995.cn

Py:   itertools.permutations(arr)
来源：http://ut.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://kl.panjiajie.cn

JS:   // 手写回溯递归
来源：http://jv.9csxet.cn

TS:   // 手写回溯递归
来源：http://pj.chemitech.net.cn

Java: // 手写回溯递归
来源：http://ay.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://ps.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://py.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://jp.521024.cn

[N09] 栈与队列
来源：http://hi.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://th.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bg.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pr.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iu.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ch.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sc.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pf.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://je.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://lg.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gs.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gw.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pe.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iy.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://bw.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nl.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lo.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rh.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://fz.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ue.shxzukj.cn

PHP:  // 手写递归函数
来源：http://uq.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kr.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eg.szsharing.cn

Java: // 手写递归
来源：http://ep.szxytkj.cn

Go:   // 手写递归
来源：http://rl.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bm.jctech888.com.cn

C#:   // 手写递归
来源：http://ma.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gs.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://od.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lw.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lz.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wl.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ip.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kg.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wu.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.yuntaijiaju.cn

================================================================================
来源：http://uw.muxihuayi.cn

O. 并发与异步
来源：http://kh.szxytkj.cn

================================================================================
来源：http://uy.hahajie.cn

[O01] 启动一个线程
来源：http://or.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jp.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ay.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xl.huanxung.cn

TS:   // 同 JS
来源：http://vk.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ed.gzmigu.cn

Go:   go f()
来源：http://hz.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://py.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://sr.muxihuayi.cn

[O02] 使用线程池
来源：http://yv.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vr.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zh.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://yf.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://gf.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mz.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hc.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ep.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ui.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://jn.huanxung.cn

Py:   with lock: shared += 1
来源：http://fq.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://fv.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kt.huixiangedu.cn

TS:   // 同 JS
来源：http://ve.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://oe.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rw.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bx.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://bp.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://vn.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://iu.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zw.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://wo.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mi.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rw.huixinmuqiang.cn


<!-- 参考信息 -->