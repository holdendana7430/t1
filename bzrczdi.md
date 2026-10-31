代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://tj.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://fv.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://wy.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ov.hahajie.cn

Go:   encoding/gob
来源：http://mo.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://xn.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://md.yuntaijiaju.cn

================================================================================
来源：http://ta.huanxung.cn

L. 网络请求
来源：http://ts.huixinmuqiang.cn

================================================================================
来源：http://mh.szsharing.cn

[L01] 发送 GET 请求
来源：http://el.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jm.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bg.nicolike.cn

JS:   await fetch(url)
来源：http://ij.gzmigu.cn

TS:   await fetch(url)
来源：http://qq.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jk.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://vb.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sj.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fv.shxzskj.cn

[L02] 发送 POST JSON
来源：http://zx.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://px.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nt.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uu.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zp.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://he.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ht.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ha.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ou.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://fc.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://if.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lb.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yu.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://as.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ax.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gi.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wv.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qt.shtwfgs.cn

[L04] 设置超时
来源：http://le.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://zi.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yq.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qv.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xo.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qi.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cv.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gk.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jv.colortex.cn

[L05] 上传文件（multipart）
来源：http://hn.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ig.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yy.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cm.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eu.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nz.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tq.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gp.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rd.asd995.cn

[L06] 解析响应为 JSON
来源：http://ar.521024.cn

Py:   resp.json()
来源：http://ei.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://dd.panjiajie.cn

JS:   await resp.json()
来源：http://on.muxihuayi.cn

TS:   await resp.json()
来源：http://wu.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dl.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tb.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://lo.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vg.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://iq.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rk.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bm.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://vx.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://sv.szxytkj.cn

Java: resp.statusCode()
来源：http://br.gzmigu.cn

Go:   resp.StatusCode
来源：http://wk.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ns.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://ly.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://br.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xc.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://fg.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lo.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pa.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gf.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qh.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cy.newstarts.cn

================================================================================
来源：http://xp.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://sx.chemitech.net.cn

================================================================================
来源：http://yn.shxzskj.cn

[M01] 读取命令行参数
来源：http://rd.szxytkj.cn

Py:   sys.argv[1:]
来源：http://sq.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://uc.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://kv.521024.cn

TS:   process.argv.slice(2)
来源：http://nv.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://eg.bjjhwx.cn

Go:   os.Args[1:]
来源：http://uq.newstarts.cn

Ruby: ARGV
来源：http://il.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://yq.szsharing.cn

[M02] 读取环境变量
来源：http://gb.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://tj.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sg.haigaiapp.cn

JS:   process.env.HOME
来源：http://gr.nicolike.cn

TS:   process.env.HOME
来源：http://ou.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://uu.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xj.nicolike.cn

Ruby: ENV["HOME"]
来源：http://gh.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gv.huixiangedu.cn

[M03] 执行外部命令
来源：http://bg.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rq.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jg.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bw.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ge.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://th.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cd.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://st.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://gn.lnxyls.cn

[M04] 获取当前工作目录
来源：http://gq.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://td.haigaiapp.cn

PHP:  getcwd();
来源：http://ag.9csxet.cn

JS:   process.cwd()
来源：http://kc.bookmarksfly.cn

TS:   process.cwd()
来源：http://lb.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://qp.9csxet.cn

Go:   os.Getwd()
来源：http://jt.newstarts.cn

Ruby: Dir.pwd
来源：http://gl.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bn.nszjky.cn

[M05] 设置退出码
来源：http://xx.shxzukj.cn

Py:   sys.exit(1)
来源：http://bx.panjiajie.cn

PHP:  exit(1);
来源：http://vj.hahajie.cn

JS:   process.exit(1)
来源：http://to.haigaiapp.cn

TS:   process.exit(1)
来源：http://rm.wgjwhj.cn

Java: System.exit(1)
来源：http://hr.nszjky.cn

Go:   os.Exit(1)
来源：http://ia.nszjky.cn

Ruby: exit 1
来源：http://ub.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lh.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ck.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://mu.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yv.nszjky.cn

JS:   console.error("err")
来源：http://zg.jctech888.com.cn

TS:   console.error("err")
来源：http://vd.nszjky.cn

Java: System.err.println("err")
来源：http://ml.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ry.521024.cn

Ruby: warn "err"
来源：http://hv.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://hp.szxytkj.cn

[M07] 判断是否为主入口
来源：http://kt.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://wi.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fh.bjjhwx.cn

JS:   require.main === module
来源：http://mk.bookmarksfly.cn

TS:   require.main === module
来源：http://mq.shxzskj.cn

Java: public static void main(String[] args)
来源：http://vf.hahajie.cn

Go:   func main()
来源：http://xn.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qr.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://yg.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://ga.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://jd.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://mm.colortex.cn

JS:   process.platform;  process.version
来源：http://tr.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://gm.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gq.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ve.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nd.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xy.hahajie.cn

================================================================================
来源：http://ll.haigaiapp.cn

N. 数据结构与算法
来源：http://am.nicolike.cn

================================================================================
来源：http://th.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://dy.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kj.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qa.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://va.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ds.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ik.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hh.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zt.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pk.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://wk.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sh.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jv.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://um.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sb.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://vp.521024.cn

Ruby: arr.sort
来源：http://xm.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xs.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://be.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nt.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://hg.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ho.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mx.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hb.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://di.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pi.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cf.jctech888.com.cn

[N04] 斐波那契数列
来源：http://at.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gy.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qe.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ty.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://po.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rd.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pn.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ti.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xh.lnxyls.cn

[N05] 最大公约数
来源：http://cv.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://vd.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xj.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://do.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uy.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ov.szsharing.cn

Ruby: a.gcd(b)
来源：http://rd.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mb.newstarts.cn

[N06] 判断回文字符串
来源：http://kx.nicolike.cn

Py:   s == s[::-1]
来源：http://dt.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://oa.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://xb.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://sx.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://to.hahajie.cn

Go:   // 双指针从两端比较
来源：http://ha.shxzukj.cn

Ruby: s == s.reverse
来源：http://xc.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ly.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://as.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ci.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pg.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hi.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://gn.9csxet.cn

Java: // 手写 HashMap
来源：http://da.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://fd.szxytkj.cn

Ruby: // 手写 Hash
来源：http://yz.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aw.panjiajie.cn

[N08] 生成全排列
来源：http://of.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://gb.newstarts.cn

PHP:  // 手写递归交换
来源：http://zn.lnxyls.cn

JS:   // 手写回溯递归
来源：http://mg.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://be.hnjuh.cn

Java: // 手写回溯递归
来源：http://jb.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://oa.521024.cn

Ruby: arr.permutation.to_a
来源：http://st.gzmigu.cn

C#:   // 手写回溯递归
来源：http://tj.haigaiapp.cn

[N09] 栈与队列
来源：http://dk.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sl.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lo.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xp.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://au.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ub.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mg.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vg.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mb.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://lo.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qu.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lb.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tv.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gm.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://vg.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mc.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://io.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lk.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://aj.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qu.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ti.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ja.shtwfgs.cn

Java: // 手写递归
来源：http://rf.szxytkj.cn

Go:   // 手写递归
来源：http://pj.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rn.huixinmuqiang.cn

C#:   // 手写递归
来源：http://ul.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kz.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ha.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ov.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://do.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lf.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vs.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iw.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rk.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pt.huanxung.cn

================================================================================
来源：http://zz.gzmigu.cn

O. 并发与异步
来源：http://mm.szsharing.cn

================================================================================
来源：http://cw.lnxyls.cn

[O01] 启动一个线程
来源：http://bm.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zm.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cj.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ds.shxzukj.cn

TS:   // 同 JS
来源：http://ct.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://jr.yuntaijiaju.cn

Go:   go f()
来源：http://tq.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://sz.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://ca.panjiajie.cn

[O02] 使用线程池
来源：http://dz.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ec.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pr.nszjky.cn

JS:   // worker_threads 线程池
来源：http://pl.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://kj.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ct.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lv.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dd.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ms.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://ol.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://qo.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://ul.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ek.shxzskj.cn

TS:   // 同 JS
来源：http://bd.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://wk.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gs.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ut.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://qx.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://xi.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://av.yuexingan06.cn


<!-- 参考信息 -->