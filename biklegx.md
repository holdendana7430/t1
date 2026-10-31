代发 wailian999

L. 网络请求
来源：http://wv.bjjhwx.cn

================================================================================
来源：http://bx.nszjky.cn

[L01] 发送 GET 请求
来源：http://ep.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vy.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bb.shxzskj.cn

JS:   await fetch(url)
来源：http://fk.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://dt.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lq.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://fe.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pi.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tb.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://bj.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vj.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ok.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qj.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cu.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tz.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://li.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yr.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://fa.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://up.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qa.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mi.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bp.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wu.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sc.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aw.nicolike.cn

[L04] 设置超时
来源：http://vk.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://ft.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hi.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yb.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ye.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yw.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oa.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fq.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wi.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://be.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bt.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ej.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zq.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sa.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lb.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wh.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fn.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jg.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://gg.lnxyls.cn

Py:   resp.json()
来源：http://sb.szsharing.cn

PHP:  json_decode($body, true);
来源：http://uu.shxzskj.cn

JS:   await resp.json()
来源：http://zr.jctech888.com.cn

TS:   await resp.json()
来源：http://av.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jo.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kk.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://ir.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vr.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://gr.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yi.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ka.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://eb.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://eg.lnxyls.cn

Java: resp.statusCode()
来源：http://pi.jctech888.com.cn

Go:   resp.StatusCode
来源：http://xz.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://sv.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://zm.shxzukj.cn

[L08] 并发请求多个地址
来源：http://uk.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jx.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://au.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://st.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yt.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wk.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fe.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://db.newstarts.cn

================================================================================
来源：http://kg.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://ya.lnxyls.cn

================================================================================
来源：http://fa.nicolike.cn

[M01] 读取命令行参数
来源：http://ro.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ac.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://cq.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://xz.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://ze.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://go.shtwfgs.cn

Go:   os.Args[1:]
来源：http://hh.521024.cn

Ruby: ARGV
来源：http://lf.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://xh.shtwfgs.cn

[M02] 读取环境变量
来源：http://ix.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://vi.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hm.muxihuayi.cn

JS:   process.env.HOME
来源：http://pp.bookmarksfly.cn

TS:   process.env.HOME
来源：http://el.colortex.cn

Java: System.getenv("HOME")
来源：http://kk.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ul.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://mc.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hj.szsharing.cn

[M03] 执行外部命令
来源：http://lh.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cj.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ax.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qp.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hp.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://op.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sa.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gk.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://hb.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://es.muxihuayi.cn

Py:   os.getcwd()
来源：http://nq.9csxet.cn

PHP:  getcwd();
来源：http://mw.shxzskj.cn

JS:   process.cwd()
来源：http://nh.haigaiapp.cn

TS:   process.cwd()
来源：http://vs.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://gl.muxihuayi.cn

Go:   os.Getwd()
来源：http://fs.newstarts.cn

Ruby: Dir.pwd
来源：http://fl.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wh.nszjky.cn

[M05] 设置退出码
来源：http://kt.shtwfgs.cn

Py:   sys.exit(1)
来源：http://vw.colortex.cn

PHP:  exit(1);
来源：http://ze.9csxet.cn

JS:   process.exit(1)
来源：http://lg.shxzukj.cn

TS:   process.exit(1)
来源：http://tx.shtwfgs.cn

Java: System.exit(1)
来源：http://rp.huanxung.cn

Go:   os.Exit(1)
来源：http://if.lnxyls.cn

Ruby: exit 1
来源：http://zt.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xc.9csxet.cn

[M06] 向标准错误输出
来源：http://mt.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://cw.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ts.huanxung.cn

JS:   console.error("err")
来源：http://rh.nicolike.cn

TS:   console.error("err")
来源：http://ru.shtwfgs.cn

Java: System.err.println("err")
来源：http://jd.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tn.asd995.cn

Ruby: warn "err"
来源：http://kc.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://av.szsharing.cn

[M07] 判断是否为主入口
来源：http://iy.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://zd.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oc.gzmigu.cn

JS:   require.main === module
来源：http://lf.panjiajie.cn

TS:   require.main === module
来源：http://jd.gzmigu.cn

Java: public static void main(String[] args)
来源：http://me.nszjky.cn

Go:   func main()
来源：http://dt.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lc.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://wx.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://wq.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://wo.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ek.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ct.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://uc.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yj.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qc.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cb.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iu.521024.cn

================================================================================
来源：http://gy.huanxung.cn

N. 数据结构与算法
来源：http://qe.shxzukj.cn

================================================================================
来源：http://qm.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://tx.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gv.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pj.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eo.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pw.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gb.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://oc.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uv.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://og.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://xt.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jx.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yq.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rf.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cq.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jr.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ew.panjiajie.cn

Ruby: arr.sort
来源：http://vf.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vg.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://bi.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bl.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://vv.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bf.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ao.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dz.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oc.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jn.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://to.hnjuh.cn

[N04] 斐波那契数列
来源：http://js.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mo.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fe.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vn.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wl.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ra.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fe.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fr.asd995.cn

[N05] 最大公约数
来源：http://vq.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://ks.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dg.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xd.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ap.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qn.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qf.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://ja.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ky.shxzukj.cn

[N06] 判断回文字符串
来源：http://el.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://eu.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://fz.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://mp.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://kc.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sx.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://kr.nszjky.cn

Ruby: s == s.reverse
来源：http://cm.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vd.521024.cn

[N07] 两数之和（返回下标）
来源：http://uk.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zk.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cj.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ns.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://mt.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://gw.newstarts.cn

Go:   // 手写 map[int]int
来源：http://vx.gzmigu.cn

Ruby: // 手写 Hash
来源：http://zx.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fo.bjjhwx.cn

[N08] 生成全排列
来源：http://ua.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://bt.shxzukj.cn

PHP:  // 手写递归交换
来源：http://ma.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://yq.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://qi.jctech888.com.cn

Java: // 手写回溯递归
来源：http://mt.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ul.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ot.gzmigu.cn

C#:   // 手写回溯递归
来源：http://re.jctech888.com.cn

[N09] 栈与队列
来源：http://su.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://go.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ol.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hq.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hf.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ao.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gq.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://av.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mu.hahajie.cn

[N10] 链表节点定义
来源：http://qw.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://od.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eh.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://os.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ii.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://rd.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fe.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wc.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xc.521024.cn

[N11] 二叉树中序遍历
来源：http://jy.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bf.panjiajie.cn

PHP:  // 手写递归函数
来源：http://jp.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://om.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mq.521024.cn

Java: // 手写递归
来源：http://tf.chemitech.net.cn

Go:   // 手写递归
来源：http://ys.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ws.szsharing.cn

C#:   // 手写递归
来源：http://al.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ui.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bk.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oy.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kk.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cw.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ih.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ao.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qc.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://xr.gzmigu.cn

O. 并发与异步
来源：http://ju.bookmarksfly.cn

================================================================================
来源：http://op.newstarts.cn

[O01] 启动一个线程
来源：http://pl.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sk.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qi.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fl.szxytkj.cn

TS:   // 同 JS
来源：http://dm.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://xn.nszjky.cn

Go:   go f()
来源：http://hv.521024.cn

Ruby: Thread.new { f }
来源：http://dw.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://zg.colortex.cn

[O02] 使用线程池
来源：http://wi.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ui.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nx.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://qu.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://xi.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rx.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iv.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ie.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kb.szsharing.cn

[O03] 加锁保护共享数据
来源：http://mj.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://xf.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zd.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nm.521024.cn

TS:   // 同 JS
来源：http://cx.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ol.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://at.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xa.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://gg.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://ud.asd995.cn

Py:   async def f():⏎    await g()
来源：http://uv.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ks.nszjky.cn

JS:   async function f() { await g(); }
来源：http://yg.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iq.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qu.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vn.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ba.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://bn.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://rl.huixiangedu.cn


<!-- 参考信息 -->