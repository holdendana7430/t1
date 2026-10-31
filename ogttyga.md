代发 wailian999

Go:   encoding/gob
来源：http://cw.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://zn.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pm.bookmarksfly.cn

================================================================================
来源：http://ug.newstarts.cn

L. 网络请求
来源：http://nh.521024.cn

================================================================================
来源：http://zr.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://xy.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dm.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rq.szsharing.cn

JS:   await fetch(url)
来源：http://da.muxihuayi.cn

TS:   await fetch(url)
来源：http://jn.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cc.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ou.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zk.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qo.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://sw.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hj.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hd.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gh.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ih.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rn.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cj.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xf.shxzskj.cn

[L03] 设置自定义请求头
来源：http://on.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ao.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jz.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sn.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nq.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kz.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://el.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ww.lnxyls.cn

[L04] 设置超时
来源：http://as.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://iw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ie.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kv.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://db.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sb.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ek.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ve.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ok.hahajie.cn

[L05] 上传文件（multipart）
来源：http://sp.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ub.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pc.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://us.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hv.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sv.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vm.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://of.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bj.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://wa.huixinmuqiang.cn

Py:   resp.json()
来源：http://eh.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://fr.chemitech.net.cn

JS:   await resp.json()
来源：http://ro.hnjuh.cn

TS:   await resp.json()
来源：http://fn.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jv.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bc.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://ae.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pj.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://po.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vh.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dw.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://kf.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://fb.9csxet.cn

Java: resp.statusCode()
来源：http://fo.huanxung.cn

Go:   resp.StatusCode
来源：http://qt.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://uk.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://vb.nicolike.cn

[L08] 并发请求多个地址
来源：http://vh.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oa.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://kf.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bk.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wr.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wg.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hi.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kq.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ij.huixiangedu.cn

================================================================================
来源：http://nc.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://gd.chemitech.net.cn

================================================================================
来源：http://pv.huanxung.cn

[M01] 读取命令行参数
来源：http://wa.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://sa.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://pz.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://gq.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://wg.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://nq.nszjky.cn

Go:   os.Args[1:]
来源：http://qm.asd995.cn

Ruby: ARGV
来源：http://oe.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://gu.asd995.cn

[M02] 读取环境变量
来源：http://ke.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://yt.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pf.9csxet.cn

JS:   process.env.HOME
来源：http://kn.jctech888.com.cn

TS:   process.env.HOME
来源：http://cp.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://fl.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jq.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ii.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://me.yuexingan06.cn

[M03] 执行外部命令
来源：http://bc.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qi.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zp.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wu.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uf.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bl.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ap.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fc.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://tb.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://xu.521024.cn

Py:   os.getcwd()
来源：http://fl.nszjky.cn

PHP:  getcwd();
来源：http://yl.jianghongdianzi.cn

JS:   process.cwd()
来源：http://fo.newstarts.cn

TS:   process.cwd()
来源：http://qj.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://jb.jctech888.com.cn

Go:   os.Getwd()
来源：http://vf.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ur.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dq.9csxet.cn

[M05] 设置退出码
来源：http://ls.colortex.cn

Py:   sys.exit(1)
来源：http://qu.szsharing.cn

PHP:  exit(1);
来源：http://jy.nszjky.cn

JS:   process.exit(1)
来源：http://pi.chemitech.net.cn

TS:   process.exit(1)
来源：http://gb.muxihuayi.cn

Java: System.exit(1)
来源：http://xc.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://ig.wgjwhj.cn

Ruby: exit 1
来源：http://in.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ej.521024.cn

[M06] 向标准错误输出
来源：http://cm.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ze.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hy.newstarts.cn

JS:   console.error("err")
来源：http://ky.colortex.cn

TS:   console.error("err")
来源：http://vr.newstarts.cn

Java: System.err.println("err")
来源：http://eo.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kp.hnjuh.cn

Ruby: warn "err"
来源：http://hz.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://uq.lnxyls.cn

[M07] 判断是否为主入口
来源：http://uq.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://lq.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.9csxet.cn

JS:   require.main === module
来源：http://bt.521024.cn

TS:   require.main === module
来源：http://fg.nicolike.cn

Java: public static void main(String[] args)
来源：http://iz.nicolike.cn

Go:   func main()
来源：http://mi.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ke.hahajie.cn

C#:   static void Main(string[] args)
来源：http://bb.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://wz.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ww.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://bq.asd995.cn

JS:   process.platform;  process.version
来源：http://zd.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://lc.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rt.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vw.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uw.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sj.szsharing.cn

================================================================================
来源：http://fz.huanxung.cn

N. 数据结构与算法
来源：http://jw.gzmigu.cn

================================================================================
来源：http://ra.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://ag.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lj.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fm.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://js.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ds.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lw.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://oj.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ws.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ms.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://an.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zj.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xy.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vs.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zu.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ej.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://kt.asd995.cn

Ruby: arr.sort
来源：http://my.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://if.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://tj.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wf.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://dd.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tq.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wm.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eq.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mm.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qs.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tl.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://lw.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sl.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ed.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uc.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bn.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ft.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qk.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cy.huixinmuqiang.cn

[N05] 最大公约数
来源：http://nm.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://es.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xd.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vx.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sv.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dq.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://kl.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vz.shxzskj.cn

[N06] 判断回文字符串
来源：http://fj.huixiangedu.cn

Py:   s == s[::-1]
来源：http://yb.nicolike.cn

PHP:  $s === strrev($s);
来源：http://zj.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ng.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://fo.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kn.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://do.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://hk.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lr.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://wm.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qs.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bn.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://if.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://vd.muxihuayi.cn

Java: // 手写 HashMap
来源：http://cq.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ri.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ko.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kv.bookmarksfly.cn

[N08] 生成全排列
来源：http://vy.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://xj.nicolike.cn

PHP:  // 手写递归交换
来源：http://cd.szxytkj.cn

JS:   // 手写回溯递归
来源：http://dt.nicolike.cn

TS:   // 手写回溯递归
来源：http://cm.hahajie.cn

Java: // 手写回溯递归
来源：http://hp.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://qp.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://eg.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://gr.521024.cn

[N09] 栈与队列
来源：http://cb.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fi.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kk.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ht.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vm.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fr.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://di.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yd.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ep.asd995.cn

[N10] 链表节点定义
来源：http://wi.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cb.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://os.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cs.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xq.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ks.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hf.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ob.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yk.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://qy.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rx.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://jj.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://re.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xo.bookmarksfly.cn

Java: // 手写递归
来源：http://wb.huixinmuqiang.cn

Go:   // 手写递归
来源：http://xt.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ru.gzmigu.cn

C#:   // 手写递归
来源：http://cx.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://md.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ar.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uv.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gw.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zl.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qm.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ij.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://if.lnxyls.cn

================================================================================
来源：http://ci.shtwfgs.cn

O. 并发与异步
来源：http://hm.shxzukj.cn

================================================================================
来源：http://ei.yuexingan06.cn

[O01] 启动一个线程
来源：http://ew.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pd.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nu.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sz.hnjuh.cn

TS:   // 同 JS
来源：http://db.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://uw.shxzskj.cn

Go:   go f()
来源：http://fm.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://fz.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://bt.nicolike.cn

[O02] 使用线程池
来源：http://ld.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://er.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wd.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://hn.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://wt.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://je.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ry.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sn.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ov.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://tn.521024.cn

Py:   with lock: shared += 1
来源：http://yl.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://zt.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qs.szsharing.cn

TS:   // 同 JS
来源：http://tj.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://tu.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hc.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://da.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://wo.newstarts.cn

[O04] 定义异步函数并等待
来源：http://jn.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://kq.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ao.asd995.cn

JS:   async function f() { await g(); }
来源：http://xx.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zi.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zs.wgjwhj.cn


<!-- 参考信息 -->