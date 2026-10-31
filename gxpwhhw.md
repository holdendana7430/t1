代发 wailian999

Go:   encoding/gob
来源：http://mx.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://fr.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nf.521024.cn

================================================================================
来源：http://te.nszjky.cn

L. 网络请求
来源：http://zi.huanxung.cn

================================================================================
来源：http://kk.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://jp.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qp.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ua.huixiangedu.cn

JS:   await fetch(url)
来源：http://xf.huixiangedu.cn

TS:   await fetch(url)
来源：http://zu.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fq.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://wk.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tk.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qf.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://qm.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kz.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ux.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uk.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://et.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wl.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fc.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jo.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bv.hnjuh.cn

[L03] 设置自定义请求头
来源：http://fz.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hq.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oi.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hw.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yx.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mt.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qk.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vu.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://up.yuntaijiaju.cn

[L04] 设置超时
来源：http://fi.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://eu.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://un.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xq.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zy.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://er.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sl.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vj.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yk.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://km.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ym.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wr.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vb.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xo.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hw.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hu.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gj.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kf.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://hr.bookmarksfly.cn

Py:   resp.json()
来源：http://ts.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://wc.haigaiapp.cn

JS:   await resp.json()
来源：http://yi.9csxet.cn

TS:   await resp.json()
来源：http://ug.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jv.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ny.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://nn.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jg.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://dy.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ef.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://up.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://bs.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://ln.shtwfgs.cn

Java: resp.statusCode()
来源：http://tu.nszjky.cn

Go:   resp.StatusCode
来源：http://ip.lnxyls.cn

Ruby: resp.code.to_i
来源：http://zx.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ri.hnjuh.cn

[L08] 并发请求多个地址
来源：http://kl.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ec.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://sl.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ql.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jd.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://se.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ue.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sz.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sr.huixinmuqiang.cn

================================================================================
来源：http://xm.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://xw.colortex.cn

================================================================================
来源：http://uc.jctech888.com.cn

[M01] 读取命令行参数
来源：http://jb.shxzskj.cn

Py:   sys.argv[1:]
来源：http://iq.szsharing.cn

PHP:  $argv;  $argc;
来源：http://pn.colortex.cn

JS:   process.argv.slice(2)
来源：http://pw.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://bk.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://uk.panjiajie.cn

Go:   os.Args[1:]
来源：http://tt.chemitech.net.cn

Ruby: ARGV
来源：http://ja.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://yb.lnxyls.cn

[M02] 读取环境变量
来源：http://sb.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://nc.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yi.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://uc.hnjuh.cn

TS:   process.env.HOME
来源：http://ol.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://nu.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mn.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://lo.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bz.colortex.cn

[M03] 执行外部命令
来源：http://fk.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dp.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jp.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://is.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rs.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jv.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ev.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://sr.szxytkj.cn

[M04] 获取当前工作目录
来源：http://xi.szsharing.cn

Py:   os.getcwd()
来源：http://nq.9csxet.cn

PHP:  getcwd();
来源：http://fv.nszjky.cn

JS:   process.cwd()
来源：http://ic.bjjhwx.cn

TS:   process.cwd()
来源：http://rc.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://zf.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ez.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ul.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sw.shxzukj.cn

[M05] 设置退出码
来源：http://sh.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://sd.yuntaijiaju.cn

PHP:  exit(1);
来源：http://qo.huixiangedu.cn

JS:   process.exit(1)
来源：http://fy.nszjky.cn

TS:   process.exit(1)
来源：http://xv.huixinmuqiang.cn

Java: System.exit(1)
来源：http://dh.521024.cn

Go:   os.Exit(1)
来源：http://uo.shxzukj.cn

Ruby: exit 1
来源：http://md.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wg.colortex.cn

[M06] 向标准错误输出
来源：http://ho.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://vc.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cn.lnxyls.cn

JS:   console.error("err")
来源：http://ho.hahajie.cn

TS:   console.error("err")
来源：http://eb.muxihuayi.cn

Java: System.err.println("err")
来源：http://ac.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pe.chemitech.net.cn

Ruby: warn "err"
来源：http://ta.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ul.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://le.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://vq.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tc.huixinmuqiang.cn

JS:   require.main === module
来源：http://mi.gzmigu.cn

TS:   require.main === module
来源：http://kh.newstarts.cn

Java: public static void main(String[] args)
来源：http://dp.521024.cn

Go:   func main()
来源：http://gz.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ny.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://zz.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://jv.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://cp.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://tq.shxzskj.cn

JS:   process.platform;  process.version
来源：http://ir.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://fj.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ep.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rt.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cz.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://md.huixiangedu.cn

================================================================================
来源：http://mx.bookmarksfly.cn

N. 数据结构与算法
来源：http://pr.521024.cn

================================================================================
来源：http://hv.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://sa.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hb.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oc.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rj.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://je.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://mx.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pq.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://th.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://pk.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ks.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jl.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bm.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cv.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://bb.shxzukj.cn

Ruby: arr.sort
来源：http://zr.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vj.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://wf.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vf.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://fz.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bx.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iv.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ck.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mc.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qy.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zm.shtwfgs.cn

[N04] 斐波那契数列
来源：http://zj.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uy.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://to.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://in.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sv.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vz.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vb.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mr.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kc.shxzukj.cn

[N05] 最大公约数
来源：http://rl.9csxet.cn

Py:   math.gcd(a, b)
来源：http://az.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vo.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bw.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vp.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lm.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nn.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://qh.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gv.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://jj.chemitech.net.cn

Py:   s == s[::-1]
来源：http://cs.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://fj.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://zb.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://cp.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wj.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://ms.nicolike.cn

Ruby: s == s.reverse
来源：http://xg.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uz.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://iw.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tx.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mq.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xm.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://ai.huanxung.cn

Java: // 手写 HashMap
来源：http://rk.asd995.cn

Go:   // 手写 map[int]int
来源：http://ha.hahajie.cn

Ruby: // 手写 Hash
来源：http://ts.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ll.shxzskj.cn

[N08] 生成全排列
来源：http://pz.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://fs.asd995.cn

PHP:  // 手写递归交换
来源：http://vi.asd995.cn

JS:   // 手写回溯递归
来源：http://kl.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://qi.huanxung.cn

Java: // 手写回溯递归
来源：http://mq.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://ph.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://tu.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://ec.huixinmuqiang.cn

[N09] 栈与队列
来源：http://gr.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ko.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qp.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ay.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uz.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://js.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gw.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xb.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yb.huixiangedu.cn

[N10] 链表节点定义
来源：http://sn.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pi.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cc.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bk.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kd.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://nd.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tt.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mk.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ie.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://bp.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sb.asd995.cn

PHP:  // 手写递归函数
来源：http://ua.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ed.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zm.haigaiapp.cn

Java: // 手写递归
来源：http://ni.bookmarksfly.cn

Go:   // 手写递归
来源：http://rq.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vx.huixiangedu.cn

C#:   // 手写递归
来源：http://ex.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ov.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dx.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mn.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yw.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xp.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://az.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aa.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qe.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kv.bjjhwx.cn

================================================================================
来源：http://ht.newstarts.cn

O. 并发与异步
来源：http://ol.wgjwhj.cn

================================================================================
来源：http://wm.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://kw.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gt.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yv.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ed.panjiajie.cn

TS:   // 同 JS
来源：http://gf.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://ed.nicolike.cn

Go:   go f()
来源：http://ny.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://aj.nszjky.cn

C#:   Task.Run(() => F());
来源：http://qi.szsharing.cn

[O02] 使用线程池
来源：http://ul.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sj.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qf.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://hc.nicolike.cn

TS:   // worker_threads 线程池
来源：http://sy.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jl.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://in.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pf.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qt.9csxet.cn

[O03] 加锁保护共享数据
来源：http://iy.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://dg.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://pf.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cg.shtwfgs.cn

TS:   // 同 JS
来源：http://tw.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://mz.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qa.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xd.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://oo.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://ub.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://tn.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ov.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://og.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hp.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bl.szxytkj.cn


<!-- 参考信息 -->