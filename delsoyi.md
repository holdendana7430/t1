代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://yj.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ix.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://uj.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qz.9csxet.cn

Go:   encoding/gob
来源：http://lq.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://xi.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hd.shxzskj.cn

================================================================================
来源：http://rp.jianghongdianzi.cn

L. 网络请求
来源：http://ni.gzmigu.cn

================================================================================
来源：http://yz.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://dq.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bq.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lv.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://eh.shtwfgs.cn

TS:   await fetch(url)
来源：http://hn.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lw.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://dg.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dh.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kf.lnxyls.cn

[L02] 发送 POST JSON
来源：http://he.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sr.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jl.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xg.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bs.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nj.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tq.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dh.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xe.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://iy.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wq.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dl.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ep.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hr.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fg.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zj.huanxung.cn

[L04] 设置超时
来源：http://ld.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://nq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://os.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xm.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xx.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lt.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xo.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rr.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://js.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://nm.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ls.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mh.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gs.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gd.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wu.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wv.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ez.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yw.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://hn.bookmarksfly.cn

Py:   resp.json()
来源：http://ha.szsharing.cn

PHP:  json_decode($body, true);
来源：http://jf.bjjhwx.cn

JS:   await resp.json()
来源：http://ib.haigaiapp.cn

TS:   await resp.json()
来源：http://bw.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nr.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ah.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://ca.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wl.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://fa.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uj.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rf.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://xj.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://ss.szsharing.cn

Java: resp.statusCode()
来源：http://nn.nicolike.cn

Go:   resp.StatusCode
来源：http://uv.colortex.cn

Ruby: resp.code.to_i
来源：http://fo.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://rf.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://cc.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zc.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://ko.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ps.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mw.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yx.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xe.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://al.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zx.haigaiapp.cn

================================================================================
来源：http://qm.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://ym.nicolike.cn

================================================================================
来源：http://np.hnjuh.cn

[M01] 读取命令行参数
来源：http://de.521024.cn

Py:   sys.argv[1:]
来源：http://qj.521024.cn

PHP:  $argv;  $argc;
来源：http://zg.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ei.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://mc.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://ul.hahajie.cn

Go:   os.Args[1:]
来源：http://jp.hnjuh.cn

Ruby: ARGV
来源：http://gh.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://qd.hahajie.cn

[M02] 读取环境变量
来源：http://ak.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://gc.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ww.shxzskj.cn

JS:   process.env.HOME
来源：http://zl.haigaiapp.cn

TS:   process.env.HOME
来源：http://ko.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://tn.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bv.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://rx.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lo.gzmigu.cn

[M03] 执行外部命令
来源：http://ng.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bz.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vt.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bi.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aj.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lh.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kw.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lw.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ky.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://np.lnxyls.cn

Py:   os.getcwd()
来源：http://fq.huixiangedu.cn

PHP:  getcwd();
来源：http://wc.colortex.cn

JS:   process.cwd()
来源：http://lo.shtwfgs.cn

TS:   process.cwd()
来源：http://ux.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://jt.nszjky.cn

Go:   os.Getwd()
来源：http://mh.nszjky.cn

Ruby: Dir.pwd
来源：http://mm.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pk.szsharing.cn

[M05] 设置退出码
来源：http://dd.huixiangedu.cn

Py:   sys.exit(1)
来源：http://va.haigaiapp.cn

PHP:  exit(1);
来源：http://dr.gzmigu.cn

JS:   process.exit(1)
来源：http://nz.nicolike.cn

TS:   process.exit(1)
来源：http://zy.hnjuh.cn

Java: System.exit(1)
来源：http://sz.9csxet.cn

Go:   os.Exit(1)
来源：http://gc.bookmarksfly.cn

Ruby: exit 1
来源：http://kk.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gf.yuexingan06.cn

[M06] 向标准错误输出
来源：http://vg.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://ty.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://if.asd995.cn

JS:   console.error("err")
来源：http://wj.shtwfgs.cn

TS:   console.error("err")
来源：http://tn.szxytkj.cn

Java: System.err.println("err")
来源：http://ge.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oc.jctech888.com.cn

Ruby: warn "err"
来源：http://qi.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://bd.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://uw.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://dn.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rv.hnjuh.cn

JS:   require.main === module
来源：http://fe.hahajie.cn

TS:   require.main === module
来源：http://rq.szsharing.cn

Java: public static void main(String[] args)
来源：http://yk.panjiajie.cn

Go:   func main()
来源：http://ao.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xk.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://ym.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://da.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://re.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yo.huanxung.cn

JS:   process.platform;  process.version
来源：http://du.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://mk.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nt.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qz.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://et.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yh.gzmigu.cn

================================================================================
来源：http://fm.jctech888.com.cn

N. 数据结构与算法
来源：http://ps.yuexingan06.cn

================================================================================
来源：http://ao.colortex.cn

[N01] 二分查找（有序数组）
来源：http://ry.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pj.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ip.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yt.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zd.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rp.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vc.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fg.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://an.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://ew.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://je.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nr.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xn.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cz.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bb.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://fp.asd995.cn

Ruby: arr.sort
来源：http://hw.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zx.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://hw.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ai.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://dz.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xs.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rh.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jq.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://va.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mx.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sv.szxytkj.cn

[N04] 斐波那契数列
来源：http://jx.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hx.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ki.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jz.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lp.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qt.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ml.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qk.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fs.szxytkj.cn

[N05] 最大公约数
来源：http://cy.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://gs.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fg.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bp.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cu.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mg.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sz.szxytkj.cn

Ruby: a.gcd(b)
来源：http://ll.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lt.yuexingan06.cn

[N06] 判断回文字符串
来源：http://gb.shxzukj.cn

Py:   s == s[::-1]
来源：http://ul.szsharing.cn

PHP:  $s === strrev($s);
来源：http://gy.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://qm.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://tv.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cv.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://mk.shtwfgs.cn

Ruby: s == s.reverse
来源：http://vl.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ii.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://gi.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ef.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wc.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ek.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://io.haigaiapp.cn

Java: // 手写 HashMap
来源：http://yj.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://il.hahajie.cn

Ruby: // 手写 Hash
来源：http://ms.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qy.huixinmuqiang.cn

[N08] 生成全排列
来源：http://zb.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://cn.gzmigu.cn

PHP:  // 手写递归交换
来源：http://me.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://vg.hahajie.cn

TS:   // 手写回溯递归
来源：http://qv.muxihuayi.cn

Java: // 手写回溯递归
来源：http://zo.nicolike.cn

Go:   // 手写回溯递归
来源：http://eb.521024.cn

Ruby: arr.permutation.to_a
来源：http://mf.huanxung.cn

C#:   // 手写回溯递归
来源：http://lt.muxihuayi.cn

[N09] 栈与队列
来源：http://tj.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mb.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wm.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hp.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sq.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xo.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jn.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ac.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://du.szsharing.cn

[N10] 链表节点定义
来源：http://ze.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://si.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bl.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fk.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nm.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://pv.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://si.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fq.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gt.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://kk.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://up.szxytkj.cn

PHP:  // 手写递归函数
来源：http://jh.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ei.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zc.yuexingan06.cn

Java: // 手写递归
来源：http://ck.521024.cn

Go:   // 手写递归
来源：http://tf.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xh.newstarts.cn

C#:   // 手写递归
来源：http://nf.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ub.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gj.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nj.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vo.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jl.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ln.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sw.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xk.jianghongdianzi.cn

================================================================================
来源：http://kc.asd995.cn

O. 并发与异步
来源：http://jp.lnxyls.cn

================================================================================
来源：http://ut.haigaiapp.cn

[O01] 启动一个线程
来源：http://hd.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jg.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zd.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ry.521024.cn

TS:   // 同 JS
来源：http://pi.521024.cn

Java: new Thread(() -> f()).start()
来源：http://se.asd995.cn

Go:   go f()
来源：http://lo.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://wc.hahajie.cn

C#:   Task.Run(() => F());
来源：http://cs.bookmarksfly.cn

[O02] 使用线程池
来源：http://mp.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pa.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dl.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://uv.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://jy.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qy.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://id.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qg.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sa.asd995.cn

[O03] 加锁保护共享数据
来源：http://yt.lnxyls.cn

Py:   with lock: shared += 1
来源：http://ty.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://ty.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pp.shxzskj.cn

TS:   // 同 JS
来源：http://vd.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://zu.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://za.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bi.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ia.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://xs.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ys.521024.cn


<!-- 参考信息 -->