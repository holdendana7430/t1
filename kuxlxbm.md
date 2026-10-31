代发 wailian999

Go:   encoding/gob
来源：http://rb.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://ds.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zf.521024.cn

================================================================================
来源：http://jl.szsharing.cn

L. 网络请求
来源：http://um.huanxung.cn

================================================================================
来源：http://sa.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://cp.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ox.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vc.bjjhwx.cn

JS:   await fetch(url)
来源：http://nq.gzmigu.cn

TS:   await fetch(url)
来源：http://dc.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://at.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ht.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://im.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xc.9csxet.cn

[L02] 发送 POST JSON
来源：http://wm.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mf.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fw.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dt.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tr.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oh.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rg.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ja.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kz.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://ti.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tz.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yw.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mp.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gx.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pc.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qa.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zz.newstarts.cn

[L04] 设置超时
来源：http://bm.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://dj.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ct.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ug.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qe.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ap.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ag.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rs.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ak.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://dv.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jx.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cx.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jt.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pr.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nu.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uj.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cv.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pw.9csxet.cn

[L06] 解析响应为 JSON
来源：http://hj.huixiangedu.cn

Py:   resp.json()
来源：http://br.szsharing.cn

PHP:  json_decode($body, true);
来源：http://wk.colortex.cn

JS:   await resp.json()
来源：http://ey.521024.cn

TS:   await resp.json()
来源：http://fi.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rb.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://es.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://kr.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xt.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://qz.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lr.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://km.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://rc.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://lv.shxzukj.cn

Java: resp.statusCode()
来源：http://vb.bjjhwx.cn

Go:   resp.StatusCode
来源：http://li.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://xz.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://gp.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://oa.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hb.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://wd.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yv.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qk.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cp.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fe.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vm.colortex.cn

================================================================================
来源：http://vj.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://hs.bjjhwx.cn

================================================================================
来源：http://ik.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://vb.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://rm.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://lp.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://ot.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://xm.asd995.cn

Java: args 数组（main 方法参数）
来源：http://kj.gzmigu.cn

Go:   os.Args[1:]
来源：http://lu.9csxet.cn

Ruby: ARGV
来源：http://yw.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://kj.shxzskj.cn

[M02] 读取环境变量
来源：http://nc.colortex.cn

Py:   os.environ.get("HOME")
来源：http://dz.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cs.panjiajie.cn

JS:   process.env.HOME
来源：http://ye.nicolike.cn

TS:   process.env.HOME
来源：http://mh.asd995.cn

Java: System.getenv("HOME")
来源：http://ec.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://el.nicolike.cn

Ruby: ENV["HOME"]
来源：http://hz.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pf.gzmigu.cn

[M03] 执行外部命令
来源：http://be.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://om.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://na.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://go.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ww.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cu.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ye.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wz.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://ag.hahajie.cn

[M04] 获取当前工作目录
来源：http://or.szxytkj.cn

Py:   os.getcwd()
来源：http://zd.hahajie.cn

PHP:  getcwd();
来源：http://ly.shxzskj.cn

JS:   process.cwd()
来源：http://wx.hnjuh.cn

TS:   process.cwd()
来源：http://jc.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://en.bjjhwx.cn

Go:   os.Getwd()
来源：http://gr.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ie.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://he.chemitech.net.cn

[M05] 设置退出码
来源：http://es.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ph.wgjwhj.cn

PHP:  exit(1);
来源：http://eb.huixiangedu.cn

JS:   process.exit(1)
来源：http://om.panjiajie.cn

TS:   process.exit(1)
来源：http://ca.hnjuh.cn

Java: System.exit(1)
来源：http://pj.shxzskj.cn

Go:   os.Exit(1)
来源：http://ln.colortex.cn

Ruby: exit 1
来源：http://nr.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ox.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://fl.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ip.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ch.wgjwhj.cn

JS:   console.error("err")
来源：http://ck.gzmigu.cn

TS:   console.error("err")
来源：http://zx.nicolike.cn

Java: System.err.println("err")
来源：http://xy.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fo.yuexingan06.cn

Ruby: warn "err"
来源：http://rz.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://tr.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://ek.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://zq.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yj.yuexingan06.cn

JS:   require.main === module
来源：http://rb.yuntaijiaju.cn

TS:   require.main === module
来源：http://xh.asd995.cn

Java: public static void main(String[] args)
来源：http://ze.nszjky.cn

Go:   func main()
来源：http://hu.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gm.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xf.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://aq.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://et.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ad.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ju.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://mx.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qv.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kg.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jf.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jb.shxzskj.cn

================================================================================
来源：http://zm.jctech888.com.cn

N. 数据结构与算法
来源：http://yb.hnjuh.cn

================================================================================
来源：http://qe.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ot.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jl.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zr.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bc.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bd.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hw.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://hq.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jk.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://px.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ui.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://yt.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zn.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hn.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fe.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://du.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://qc.haigaiapp.cn

Ruby: arr.sort
来源：http://sj.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yt.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://fa.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cs.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://km.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wr.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fa.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yb.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jo.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xr.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mw.nszjky.cn

[N04] 斐波那契数列
来源：http://vt.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://od.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://av.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gs.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cc.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jc.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gx.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ta.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://my.gzmigu.cn

[N05] 最大公约数
来源：http://hu.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://mp.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lb.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qb.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dc.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rb.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rm.nszjky.cn

Ruby: a.gcd(b)
来源：http://li.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oj.wgjwhj.cn

[N06] 判断回文字符串
来源：http://bb.asd995.cn

Py:   s == s[::-1]
来源：http://tc.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://jy.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://sy.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://ur.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://le.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://ai.lnxyls.cn

Ruby: s == s.reverse
来源：http://pj.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://za.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://qp.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sw.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vb.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yv.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ug.gzmigu.cn

Java: // 手写 HashMap
来源：http://wu.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ut.9csxet.cn

Ruby: // 手写 Hash
来源：http://tx.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iw.colortex.cn

[N08] 生成全排列
来源：http://ef.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://ir.521024.cn

PHP:  // 手写递归交换
来源：http://xo.colortex.cn

JS:   // 手写回溯递归
来源：http://nj.asd995.cn

TS:   // 手写回溯递归
来源：http://ag.nicolike.cn

Java: // 手写回溯递归
来源：http://jo.colortex.cn

Go:   // 手写回溯递归
来源：http://jq.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://of.nszjky.cn

C#:   // 手写回溯递归
来源：http://sg.huanxung.cn

[N09] 栈与队列
来源：http://fh.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sk.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qv.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pm.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zd.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ea.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://us.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ts.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://su.nszjky.cn

[N10] 链表节点定义
来源：http://xv.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qc.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://je.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vt.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xe.asd995.cn

Java: class Node { int v; Node next; }
来源：http://ve.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rw.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://js.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://al.colortex.cn

[N11] 二叉树中序遍历
来源：http://zw.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vj.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://kw.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ph.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fv.hnjuh.cn

Java: // 手写递归
来源：http://ke.huanxung.cn

Go:   // 手写递归
来源：http://gq.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kf.lnxyls.cn

C#:   // 手写递归
来源：http://lc.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sb.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://le.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bi.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dk.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fg.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nq.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cp.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mu.lnxyls.cn

================================================================================
来源：http://nv.bjjhwx.cn

O. 并发与异步
来源：http://yq.shxzukj.cn

================================================================================
来源：http://kr.hnjuh.cn

[O01] 启动一个线程
来源：http://nl.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://am.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nv.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eq.newstarts.cn

TS:   // 同 JS
来源：http://lh.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://py.asd995.cn

Go:   go f()
来源：http://wc.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://yz.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://mz.yuntaijiaju.cn

[O02] 使用线程池
来源：http://vt.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://au.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gp.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://mi.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://zj.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xk.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iy.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jh.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gy.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://yn.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://gs.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://od.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://od.szsharing.cn

TS:   // 同 JS
来源：http://ig.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ts.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ms.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://it.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://ph.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://dm.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://zm.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://di.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://bo.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zh.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kq.yuntaijiaju.cn


<!-- 参考信息 -->