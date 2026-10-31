代发 wailian999

[K06] 解析 URL 查询串
来源：http://zb.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pb.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gw.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ir.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wb.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vw.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uw.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iv.shxzukj.cn

[K07] 进制转换
来源：http://iy.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zd.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vw.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jx.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nr.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sv.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zo.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zq.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rw.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://sr.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://hg.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lw.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ts.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://au.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://is.bookmarksfly.cn

Go:   encoding/gob
来源：http://ud.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://jn.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wu.huixinmuqiang.cn

================================================================================
来源：http://wb.shxzskj.cn

L. 网络请求
来源：http://fw.newstarts.cn

================================================================================
来源：http://km.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://nk.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://br.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xo.nszjky.cn

JS:   await fetch(url)
来源：http://aq.hahajie.cn

TS:   await fetch(url)
来源：http://cx.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mg.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://hf.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ie.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zx.nszjky.cn

[L02] 发送 POST JSON
来源：http://yu.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://si.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bb.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oa.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ci.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mn.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ev.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pj.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qc.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://if.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qw.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://df.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vx.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jk.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fx.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vd.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kd.jianghongdianzi.cn

[L04] 设置超时
来源：http://os.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://rm.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xc.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pr.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://um.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://km.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jr.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nl.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pn.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://ou.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://av.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gi.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gu.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yo.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ii.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zg.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xk.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fb.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://uk.shxzskj.cn

Py:   resp.json()
来源：http://ir.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ta.jianghongdianzi.cn

JS:   await resp.json()
来源：http://wh.shtwfgs.cn

TS:   await resp.json()
来源：http://un.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://px.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sg.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://if.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nd.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://nv.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gy.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bb.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://dz.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://gd.nicolike.cn

Java: resp.statusCode()
来源：http://un.haigaiapp.cn

Go:   resp.StatusCode
来源：http://tm.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://xq.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://ak.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://wz.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zf.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://zd.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gt.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hw.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bn.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pr.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ws.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wv.nicolike.cn

================================================================================
来源：http://bt.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://hr.shxzskj.cn

================================================================================
来源：http://sj.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://yt.huanxung.cn

Py:   sys.argv[1:]
来源：http://sy.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://tr.asd995.cn

JS:   process.argv.slice(2)
来源：http://uw.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://fq.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://au.colortex.cn

Go:   os.Args[1:]
来源：http://mx.nicolike.cn

Ruby: ARGV
来源：http://yk.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://yu.asd995.cn

[M02] 读取环境变量
来源：http://qh.colortex.cn

Py:   os.environ.get("HOME")
来源：http://jm.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vj.huanxung.cn

JS:   process.env.HOME
来源：http://ml.shtwfgs.cn

TS:   process.env.HOME
来源：http://vm.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://md.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xf.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://jr.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uh.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://jy.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qe.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yl.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://so.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://li.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mf.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ir.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gi.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://pp.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://zk.huixiangedu.cn

Py:   os.getcwd()
来源：http://yf.szsharing.cn

PHP:  getcwd();
来源：http://hl.newstarts.cn

JS:   process.cwd()
来源：http://ae.huanxung.cn

TS:   process.cwd()
来源：http://ek.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://sl.panjiajie.cn

Go:   os.Getwd()
来源：http://bz.chemitech.net.cn

Ruby: Dir.pwd
来源：http://jf.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ru.shxzskj.cn

[M05] 设置退出码
来源：http://jz.huanxung.cn

Py:   sys.exit(1)
来源：http://to.hahajie.cn

PHP:  exit(1);
来源：http://yv.hnjuh.cn

JS:   process.exit(1)
来源：http://fc.szxytkj.cn

TS:   process.exit(1)
来源：http://xz.9csxet.cn

Java: System.exit(1)
来源：http://lm.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://pk.haigaiapp.cn

Ruby: exit 1
来源：http://ve.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://go.wgjwhj.cn

[M06] 向标准错误输出
来源：http://ld.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://ag.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hr.nicolike.cn

JS:   console.error("err")
来源：http://gq.shtwfgs.cn

TS:   console.error("err")
来源：http://ht.hahajie.cn

Java: System.err.println("err")
来源：http://pm.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yi.szsharing.cn

Ruby: warn "err"
来源：http://lm.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://no.szxytkj.cn

[M07] 判断是否为主入口
来源：http://td.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://eu.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uo.haigaiapp.cn

JS:   require.main === module
来源：http://ap.szxytkj.cn

TS:   require.main === module
来源：http://ve.panjiajie.cn

Java: public static void main(String[] args)
来源：http://qf.panjiajie.cn

Go:   func main()
来源：http://ql.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tb.521024.cn

C#:   static void Main(string[] args)
来源：http://hs.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://oz.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://qj.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://pb.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://kg.nicolike.cn

TS:   process.platform;  process.version
来源：http://mo.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oe.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rf.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aj.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ew.jianghongdianzi.cn

================================================================================
来源：http://bm.yuexingan06.cn

N. 数据结构与算法
来源：http://yx.jianghongdianzi.cn

================================================================================
来源：http://lx.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://qt.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nf.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tl.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hg.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gd.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://wf.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ee.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sg.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://jb.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kd.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ov.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://np.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yd.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lg.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://dd.wgjwhj.cn

Ruby: arr.sort
来源：http://ja.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zh.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://lw.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qy.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://tf.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hk.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ik.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zq.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zw.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xx.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qn.szxytkj.cn

[N04] 斐波那契数列
来源：http://ky.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qh.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fk.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wz.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vq.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uh.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rl.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://je.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ot.muxihuayi.cn

[N05] 最大公约数
来源：http://yk.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://ky.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ix.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lg.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mh.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qp.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://to.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uf.newstarts.cn

[N06] 判断回文字符串
来源：http://ox.chemitech.net.cn

Py:   s == s[::-1]
来源：http://mb.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://zq.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://is.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://bi.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ag.asd995.cn

Go:   // 双指针从两端比较
来源：http://gl.shxzukj.cn

Ruby: s == s.reverse
来源：http://kr.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uo.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://uy.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ks.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rq.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xl.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://rw.szxytkj.cn

Java: // 手写 HashMap
来源：http://mp.newstarts.cn

Go:   // 手写 map[int]int
来源：http://la.panjiajie.cn

Ruby: // 手写 Hash
来源：http://uw.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kc.chemitech.net.cn

[N08] 生成全排列
来源：http://sq.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://pc.newstarts.cn

PHP:  // 手写递归交换
来源：http://td.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://rz.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://ow.asd995.cn

Java: // 手写回溯递归
来源：http://fv.huanxung.cn

Go:   // 手写回溯递归
来源：http://zp.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://qp.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://us.huixinmuqiang.cn

[N09] 栈与队列
来源：http://nb.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nd.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sf.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pt.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dn.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jq.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pg.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oa.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wm.szxytkj.cn

[N10] 链表节点定义
来源：http://xs.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rw.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hf.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pw.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zi.colortex.cn

Java: class Node { int v; Node next; }
来源：http://zn.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sb.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ni.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ae.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://tf.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qn.panjiajie.cn

PHP:  // 手写递归函数
来源：http://ge.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kc.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zr.bookmarksfly.cn

Java: // 手写递归
来源：http://xw.jctech888.com.cn

Go:   // 手写递归
来源：http://aj.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://es.yuntaijiaju.cn

C#:   // 手写递归
来源：http://dg.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jk.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://le.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zn.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://so.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aw.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ux.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ni.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lb.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fg.huixinmuqiang.cn

================================================================================
来源：http://ef.szsharing.cn

O. 并发与异步
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://yp.panjiajie.cn

[O01] 启动一个线程
来源：http://ia.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oq.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ti.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tq.hahajie.cn

TS:   // 同 JS
来源：http://oh.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://ce.bookmarksfly.cn

Go:   go f()
来源：http://ku.szxytkj.cn

Ruby: Thread.new { f }
来源：http://cs.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://sg.huixiangedu.cn


<!-- 参考信息 -->