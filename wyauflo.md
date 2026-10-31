代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://kr.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://bi.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://rn.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.shxzukj.cn

Go:   encoding/gob
来源：http://sc.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://rk.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kw.huixiangedu.cn

================================================================================
来源：http://sh.panjiajie.cn

L. 网络请求
来源：http://fu.huixiangedu.cn

================================================================================
来源：http://nf.shxzskj.cn

[L01] 发送 GET 请求
来源：http://sm.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xs.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eg.newstarts.cn

JS:   await fetch(url)
来源：http://rf.szxytkj.cn

TS:   await fetch(url)
来源：http://mk.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://si.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://au.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ig.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://us.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://yz.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ok.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rl.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ac.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tf.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nc.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ru.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sn.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pk.gzmigu.cn

[L03] 设置自定义请求头
来源：http://eb.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nw.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://km.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ng.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hj.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://no.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cx.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://un.newstarts.cn

[L04] 设置超时
来源：http://gk.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://zv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://at.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wh.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ws.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ss.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ch.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wn.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fy.colortex.cn

[L05] 上传文件（multipart）
来源：http://ig.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ho.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nh.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vm.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pq.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zh.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sm.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rn.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://hw.panjiajie.cn

Py:   resp.json()
来源：http://kk.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://ks.nszjky.cn

JS:   await resp.json()
来源：http://pg.yuexingan06.cn

TS:   await resp.json()
来源：http://on.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ih.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vn.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://yv.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zt.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://sv.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ip.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nn.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://wv.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://yz.nicolike.cn

Java: resp.statusCode()
来源：http://su.hnjuh.cn

Go:   resp.StatusCode
来源：http://hl.521024.cn

Ruby: resp.code.to_i
来源：http://wf.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://gz.szsharing.cn

[L08] 并发请求多个地址
来源：http://jd.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xq.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://qj.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nt.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ww.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ib.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://is.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ps.nszjky.cn

================================================================================
来源：http://ek.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://hg.chemitech.net.cn

================================================================================
来源：http://ej.jctech888.com.cn

[M01] 读取命令行参数
来源：http://xq.hahajie.cn

Py:   sys.argv[1:]
来源：http://wd.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://fc.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://wa.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://qx.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://yf.shxzukj.cn

Go:   os.Args[1:]
来源：http://yf.nszjky.cn

Ruby: ARGV
来源：http://ph.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://zg.bjjhwx.cn

[M02] 读取环境变量
来源：http://sx.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://iq.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zp.shxzukj.cn

JS:   process.env.HOME
来源：http://yl.szsharing.cn

TS:   process.env.HOME
来源：http://xw.gzmigu.cn

Java: System.getenv("HOME")
来源：http://jb.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ge.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ou.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jj.nicolike.cn

[M03] 执行外部命令
来源：http://ad.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vp.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eb.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://we.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://am.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tu.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ou.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ce.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://iv.nszjky.cn

[M04] 获取当前工作目录
来源：http://it.huixiangedu.cn

Py:   os.getcwd()
来源：http://yk.jctech888.com.cn

PHP:  getcwd();
来源：http://kq.9csxet.cn

JS:   process.cwd()
来源：http://pm.huixiangedu.cn

TS:   process.cwd()
来源：http://jn.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://xx.panjiajie.cn

Go:   os.Getwd()
来源：http://zr.yuexingan06.cn

Ruby: Dir.pwd
来源：http://gn.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iz.lnxyls.cn

[M05] 设置退出码
来源：http://px.shxzukj.cn

Py:   sys.exit(1)
来源：http://yr.chemitech.net.cn

PHP:  exit(1);
来源：http://zb.szxytkj.cn

JS:   process.exit(1)
来源：http://il.hnjuh.cn

TS:   process.exit(1)
来源：http://jh.szsharing.cn

Java: System.exit(1)
来源：http://it.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://lj.haigaiapp.cn

Ruby: exit 1
来源：http://zi.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yt.jctech888.com.cn

[M06] 向标准错误输出
来源：http://bl.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://sm.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sk.huixinmuqiang.cn

JS:   console.error("err")
来源：http://cd.szsharing.cn

TS:   console.error("err")
来源：http://mg.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ev.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kx.haigaiapp.cn

Ruby: warn "err"
来源：http://rw.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://qe.colortex.cn

[M07] 判断是否为主入口
来源：http://pj.colortex.cn

Py:   if __name__ == "__main__":
来源：http://yo.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hk.wgjwhj.cn

JS:   require.main === module
来源：http://ho.hahajie.cn

TS:   require.main === module
来源：http://yd.shxzskj.cn

Java: public static void main(String[] args)
来源：http://gv.shxzskj.cn

Go:   func main()
来源：http://ev.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kh.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://fx.asd995.cn

[M08] 获取系统与运行时信息
来源：http://oo.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://id.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://kq.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://wy.panjiajie.cn

TS:   process.platform;  process.version
来源：http://ah.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ky.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ku.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yf.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bh.chemitech.net.cn

================================================================================
来源：http://ek.newstarts.cn

N. 数据结构与算法
来源：http://ct.huanxung.cn

================================================================================
来源：http://uj.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://zv.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ro.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://az.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jj.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://ly.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eg.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mn.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zt.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://jw.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rv.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xv.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://el.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jf.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://mm.colortex.cn

Ruby: arr.sort
来源：http://vl.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ze.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://cn.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://np.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://rn.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ft.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ai.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ea.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rt.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wg.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://tr.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sb.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ui.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bq.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kr.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nt.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tr.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://su.colortex.cn

[N05] 最大公约数
来源：http://qz.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://fr.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zd.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://co.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pj.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rz.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://li.shxzskj.cn

Ruby: a.gcd(b)
来源：http://yn.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cb.panjiajie.cn

[N06] 判断回文字符串
来源：http://zw.lnxyls.cn

Py:   s == s[::-1]
来源：http://ne.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://de.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ys.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://nb.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pf.9csxet.cn

Go:   // 双指针从两端比较
来源：http://vc.panjiajie.cn

Ruby: s == s.reverse
来源：http://yv.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aj.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://cx.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fe.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qi.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mx.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://zp.hnjuh.cn

Java: // 手写 HashMap
来源：http://qc.hahajie.cn

Go:   // 手写 map[int]int
来源：http://ii.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://jv.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bb.newstarts.cn

[N08] 生成全排列
来源：http://gi.521024.cn

Py:   itertools.permutations(arr)
来源：http://ht.nszjky.cn

PHP:  // 手写递归交换
来源：http://le.521024.cn

JS:   // 手写回溯递归
来源：http://nl.nicolike.cn

TS:   // 手写回溯递归
来源：http://tx.9csxet.cn

Java: // 手写回溯递归
来源：http://hn.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://eo.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://qz.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ja.wgjwhj.cn

[N09] 栈与队列
来源：http://on.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vb.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ke.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fw.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cb.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zu.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pm.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ta.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yg.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://cb.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vz.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uj.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ht.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cm.asd995.cn

Java: class Node { int v; Node next; }
来源：http://yr.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://az.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://il.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qa.nszjky.cn

[N11] 二叉树中序遍历
来源：http://mm.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://md.hnjuh.cn

PHP:  // 手写递归函数
来源：http://yy.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mj.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ds.newstarts.cn

Java: // 手写递归
来源：http://gu.lnxyls.cn

Go:   // 手写递归
来源：http://qy.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ng.huixiangedu.cn

C#:   // 手写递归
来源：http://ws.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ms.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wt.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ue.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gv.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yv.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xo.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mc.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zt.nicolike.cn

================================================================================
来源：http://hu.shtwfgs.cn

O. 并发与异步
来源：http://io.521024.cn

================================================================================
来源：http://yk.huixiangedu.cn

[O01] 启动一个线程
来源：http://bz.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hj.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ry.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://to.jctech888.com.cn

TS:   // 同 JS
来源：http://gs.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://ml.huanxung.cn

Go:   go f()
来源：http://kz.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://oj.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://yg.jctech888.com.cn

[O02] 使用线程池
来源：http://xi.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sd.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zb.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ft.9csxet.cn

TS:   // worker_threads 线程池
来源：http://on.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oa.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vh.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bo.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sv.asd995.cn

[O03] 加锁保护共享数据
来源：http://ap.panjiajie.cn

Py:   with lock: shared += 1
来源：http://vj.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://hx.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yg.shtwfgs.cn

TS:   // 同 JS
来源：http://qq.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://hy.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yt.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ds.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://gj.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://io.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://iz.jianghongdianzi.cn


<!-- 参考信息 -->