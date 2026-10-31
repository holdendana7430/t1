代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://cj.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://ec.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://sf.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sj.lnxyls.cn

Go:   encoding/gob
来源：http://ro.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://ec.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vu.yuntaijiaju.cn

================================================================================
来源：http://kv.521024.cn

L. 网络请求
来源：http://kj.wgjwhj.cn

================================================================================
来源：http://hs.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://vf.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ze.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ak.521024.cn

JS:   await fetch(url)
来源：http://on.yuexingan06.cn

TS:   await fetch(url)
来源：http://hy.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wh.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://bc.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ai.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ym.9csxet.cn

[L02] 发送 POST JSON
来源：http://rh.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ho.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qx.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tn.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://di.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xy.9csxet.cn

[L03] 设置自定义请求头
来源：http://kt.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fs.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ak.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zb.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rq.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ho.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jz.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vd.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dx.hnjuh.cn

[L04] 设置超时
来源：http://oe.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://fa.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sr.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wq.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qd.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xc.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lk.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kl.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ow.asd995.cn

[L05] 上传文件（multipart）
来源：http://ws.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fa.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ib.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zw.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://an.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rx.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fo.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://he.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pl.521024.cn

[L06] 解析响应为 JSON
来源：http://ww.huixiangedu.cn

Py:   resp.json()
来源：http://tx.nszjky.cn

PHP:  json_decode($body, true);
来源：http://jf.jianghongdianzi.cn

JS:   await resp.json()
来源：http://tb.muxihuayi.cn

TS:   await resp.json()
来源：http://dv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sw.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ii.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://mn.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pl.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://ml.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xc.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eu.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://je.asd995.cn

TS:   resp.ok;  resp.status
来源：http://rj.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://wn.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://wf.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ls.521024.cn

C#:   (int)resp.StatusCode
来源：http://zy.nszjky.cn

[L08] 并发请求多个地址
来源：http://vt.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nv.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://tg.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qf.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wf.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://om.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://us.yuexingan06.cn

================================================================================
来源：http://hk.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://zs.panjiajie.cn

================================================================================
来源：http://gu.9csxet.cn

[M01] 读取命令行参数
来源：http://nw.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://bt.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://gx.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://yd.521024.cn

TS:   process.argv.slice(2)
来源：http://bq.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://tb.szsharing.cn

Go:   os.Args[1:]
来源：http://op.huixinmuqiang.cn

Ruby: ARGV
来源：http://oq.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://dy.szsharing.cn

[M02] 读取环境变量
来源：http://mk.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://pd.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vo.panjiajie.cn

JS:   process.env.HOME
来源：http://cz.shxzskj.cn

TS:   process.env.HOME
来源：http://hm.nicolike.cn

Java: System.getenv("HOME")
来源：http://vn.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ac.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://dl.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eh.yuexingan06.cn

[M03] 执行外部命令
来源：http://zd.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://te.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hw.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mo.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vz.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nq.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lf.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yi.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://nd.lnxyls.cn

[M04] 获取当前工作目录
来源：http://fk.huixiangedu.cn

Py:   os.getcwd()
来源：http://ke.gzmigu.cn

PHP:  getcwd();
来源：http://vt.lnxyls.cn

JS:   process.cwd()
来源：http://ug.huixiangedu.cn

TS:   process.cwd()
来源：http://nc.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://tj.hnjuh.cn

Go:   os.Getwd()
来源：http://ow.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://xg.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ig.hahajie.cn

[M05] 设置退出码
来源：http://xj.szsharing.cn

Py:   sys.exit(1)
来源：http://vx.huanxung.cn

PHP:  exit(1);
来源：http://kw.chemitech.net.cn

JS:   process.exit(1)
来源：http://as.panjiajie.cn

TS:   process.exit(1)
来源：http://zy.bjjhwx.cn

Java: System.exit(1)
来源：http://oe.shtwfgs.cn

Go:   os.Exit(1)
来源：http://nc.chemitech.net.cn

Ruby: exit 1
来源：http://xv.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vh.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://th.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://ut.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hf.gzmigu.cn

JS:   console.error("err")
来源：http://fd.shxzukj.cn

TS:   console.error("err")
来源：http://dr.shxzukj.cn

Java: System.err.println("err")
来源：http://zk.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oi.asd995.cn

Ruby: warn "err"
来源：http://sc.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://sa.huanxung.cn

[M07] 判断是否为主入口
来源：http://mb.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://qg.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uv.yuntaijiaju.cn

JS:   require.main === module
来源：http://kf.panjiajie.cn

TS:   require.main === module
来源：http://mp.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://df.szxytkj.cn

Go:   func main()
来源：http://iz.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wc.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://tt.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://no.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://ls.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://cd.lnxyls.cn

JS:   process.platform;  process.version
来源：http://kc.hnjuh.cn

TS:   process.platform;  process.version
来源：http://dz.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xe.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://es.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://we.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zb.shxzukj.cn

================================================================================
来源：http://oz.szxytkj.cn

N. 数据结构与算法
来源：http://lz.nicolike.cn

================================================================================
来源：http://we.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://di.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yg.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pp.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sr.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xe.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xr.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://jd.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sw.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rn.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qg.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://qa.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://az.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ic.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sg.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lb.szsharing.cn

Go:   slices.Sort(arr)
来源：http://zl.shxzskj.cn

Ruby: arr.sort
来源：http://ae.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hs.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://vy.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bv.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ww.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lt.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ih.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lh.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nm.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ch.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uy.huanxung.cn

[N04] 斐波那契数列
来源：http://do.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cu.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fs.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ug.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xv.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eg.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vk.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mn.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pk.haigaiapp.cn

[N05] 最大公约数
来源：http://nf.hahajie.cn

Py:   math.gcd(a, b)
来源：http://jl.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://el.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bw.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aa.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cr.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cb.newstarts.cn

Ruby: a.gcd(b)
来源：http://oz.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jw.muxihuayi.cn

[N06] 判断回文字符串
来源：http://lo.panjiajie.cn

Py:   s == s[::-1]
来源：http://ip.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://xh.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://fh.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ni.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://od.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://dm.huixiangedu.cn

Ruby: s == s.reverse
来源：http://dl.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oz.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://eo.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pu.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vp.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jc.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://bu.haigaiapp.cn

Java: // 手写 HashMap
来源：http://ty.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://yp.szsharing.cn

Ruby: // 手写 Hash
来源：http://uy.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ua.panjiajie.cn

[N08] 生成全排列
来源：http://lh.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://hg.gzmigu.cn

PHP:  // 手写递归交换
来源：http://jq.colortex.cn

JS:   // 手写回溯递归
来源：http://lq.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://ta.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://vz.asd995.cn

Go:   // 手写回溯递归
来源：http://bx.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://lq.shxzukj.cn

C#:   // 手写回溯递归
来源：http://bt.bookmarksfly.cn

[N09] 栈与队列
来源：http://bx.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eo.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lh.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hm.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iz.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pd.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uh.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hw.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cz.chemitech.net.cn

[N10] 链表节点定义
来源：http://gg.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sa.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xa.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ro.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wk.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://fk.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rh.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rn.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qe.colortex.cn

[N11] 二叉树中序遍历
来源：http://kx.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jx.colortex.cn

PHP:  // 手写递归函数
来源：http://lx.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vb.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bz.colortex.cn

Java: // 手写递归
来源：http://yt.bjjhwx.cn

Go:   // 手写递归
来源：http://lg.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ec.hnjuh.cn

C#:   // 手写递归
来源：http://rs.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vo.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kd.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ba.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qz.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bg.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sb.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bx.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lm.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lg.yuexingan06.cn

================================================================================
来源：http://zs.shtwfgs.cn

O. 并发与异步
来源：http://yq.shtwfgs.cn

================================================================================
来源：http://fv.wgjwhj.cn

[O01] 启动一个线程
来源：http://jc.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pv.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mr.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bb.asd995.cn

TS:   // 同 JS
来源：http://kk.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://xg.colortex.cn

Go:   go f()
来源：http://au.9csxet.cn

Ruby: Thread.new { f }
来源：http://vd.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://jz.shxzukj.cn

[O02] 使用线程池
来源：http://st.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hb.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jx.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://fz.nicolike.cn

TS:   // worker_threads 线程池
来源：http://py.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ge.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://md.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bd.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dp.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://xh.panjiajie.cn

Py:   with lock: shared += 1
来源：http://me.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ul.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xx.hnjuh.cn

TS:   // 同 JS
来源：http://ps.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://km.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gz.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tj.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://zo.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://pb.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://xk.muxihuayi.cn


<!-- 参考信息 -->