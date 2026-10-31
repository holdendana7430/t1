代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://la.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oq.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hy.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ce.521024.cn

Py:   copy.deepcopy(obj)
来源：http://sr.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://ld.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://bd.panjiajie.cn

TS:   structuredClone(obj)
来源：http://ob.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xd.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mk.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fn.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ne.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://rp.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dm.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ro.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jo.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fo.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ph.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://at.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rd.szxytkj.cn

[K07] 进制转换
来源：http://ee.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yf.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ne.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nk.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://en.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iv.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vv.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dl.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dd.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://vt.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://wt.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sq.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://eo.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://dg.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bp.muxihuayi.cn

Go:   encoding/gob
来源：http://wm.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://pz.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qj.newstarts.cn

================================================================================
来源：http://tz.jianghongdianzi.cn

L. 网络请求
来源：http://qt.panjiajie.cn

================================================================================
来源：http://lo.shxzukj.cn

[L01] 发送 GET 请求
来源：http://lk.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wb.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xe.lnxyls.cn

JS:   await fetch(url)
来源：http://pi.hahajie.cn

TS:   await fetch(url)
来源：http://df.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ge.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://xo.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://am.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uz.9csxet.cn

[L02] 发送 POST JSON
来源：http://fk.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dn.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sk.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ww.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bg.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nf.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cl.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://km.panjiajie.cn

[L03] 设置自定义请求头
来源：http://hf.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tg.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vq.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cl.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tw.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nr.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jq.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aj.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://er.jctech888.com.cn

[L04] 设置超时
来源：http://dd.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://mm.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://li.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rh.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lg.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ov.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sh.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bu.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xb.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://ae.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xu.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jx.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kt.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hq.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ic.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cq.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yo.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pa.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://bz.9csxet.cn

Py:   resp.json()
来源：http://wp.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://cu.wgjwhj.cn

JS:   await resp.json()
来源：http://ii.yuexingan06.cn

TS:   await resp.json()
来源：http://dj.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ym.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pr.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://na.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ra.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://id.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eg.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yt.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ix.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://wk.szsharing.cn

Java: resp.statusCode()
来源：http://ya.chemitech.net.cn

Go:   resp.StatusCode
来源：http://mt.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://xs.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://tu.lnxyls.cn

[L08] 并发请求多个地址
来源：http://pf.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xn.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://qu.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tm.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cz.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zy.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rc.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ln.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://do.shxzskj.cn

================================================================================
来源：http://fc.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://bo.hnjuh.cn

================================================================================
来源：http://yt.muxihuayi.cn

[M01] 读取命令行参数
来源：http://fq.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://am.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://nm.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://cw.nszjky.cn

TS:   process.argv.slice(2)
来源：http://ub.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://on.521024.cn

Go:   os.Args[1:]
来源：http://vc.huanxung.cn

Ruby: ARGV
来源：http://xj.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ji.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://jb.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://do.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wr.haigaiapp.cn

JS:   process.env.HOME
来源：http://rr.huanxung.cn

TS:   process.env.HOME
来源：http://bb.gzmigu.cn

Java: System.getenv("HOME")
来源：http://cf.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iu.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://gp.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fg.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://ob.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://po.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wq.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://go.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cw.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dc.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mu.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sn.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://fh.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://ss.bookmarksfly.cn

Py:   os.getcwd()
来源：http://dy.hnjuh.cn

PHP:  getcwd();
来源：http://xq.newstarts.cn

JS:   process.cwd()
来源：http://fx.shxzukj.cn

TS:   process.cwd()
来源：http://th.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://dn.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://ug.lnxyls.cn

Ruby: Dir.pwd
来源：http://zy.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ce.jianghongdianzi.cn

[M05] 设置退出码
来源：http://vq.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://px.521024.cn

PHP:  exit(1);
来源：http://zr.bookmarksfly.cn

JS:   process.exit(1)
来源：http://cp.nszjky.cn

TS:   process.exit(1)
来源：http://xa.jianghongdianzi.cn

Java: System.exit(1)
来源：http://ok.hahajie.cn

Go:   os.Exit(1)
来源：http://mm.jianghongdianzi.cn

Ruby: exit 1
来源：http://jw.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sx.muxihuayi.cn

[M06] 向标准错误输出
来源：http://lv.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://dm.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zg.shxzskj.cn

JS:   console.error("err")
来源：http://hu.nszjky.cn

TS:   console.error("err")
来源：http://xo.nicolike.cn

Java: System.err.println("err")
来源：http://ua.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ye.haigaiapp.cn

Ruby: warn "err"
来源：http://tn.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://kk.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://dz.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://yy.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wn.asd995.cn

JS:   require.main === module
来源：http://cj.shxzskj.cn

TS:   require.main === module
来源：http://un.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://gw.colortex.cn

Go:   func main()
来源：http://cy.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qk.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://gm.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://hf.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://om.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ih.lnxyls.cn

JS:   process.platform;  process.version
来源：http://mg.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://pt.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://df.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lc.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gg.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gq.newstarts.cn

================================================================================
来源：http://cx.lnxyls.cn

N. 数据结构与算法
来源：http://zx.newstarts.cn

================================================================================
来源：http://eo.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://js.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nd.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ur.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cj.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jo.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uz.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://cu.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vr.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vn.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ch.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://le.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://no.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://am.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fg.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ay.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://fq.szsharing.cn

Ruby: arr.sort
来源：http://oa.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vk.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://ec.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://df.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ww.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iw.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://li.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ov.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sp.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ai.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xp.gzmigu.cn

[N04] 斐波那契数列
来源：http://ez.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://et.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ms.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mx.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gg.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jj.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ho.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zv.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rt.huixiangedu.cn

[N05] 最大公约数
来源：http://xx.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://pd.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sm.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jm.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hs.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dh.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zp.hnjuh.cn

Ruby: a.gcd(b)
来源：http://yt.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://da.panjiajie.cn

[N06] 判断回文字符串
来源：http://ka.szsharing.cn

Py:   s == s[::-1]
来源：http://tb.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://ol.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://tr.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://xg.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jt.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://yi.szxytkj.cn

Ruby: s == s.reverse
来源：http://oz.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rx.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://fe.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mh.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rn.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vq.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ll.huixiangedu.cn

Java: // 手写 HashMap
来源：http://hw.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://er.shxzskj.cn

Ruby: // 手写 Hash
来源：http://jo.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lx.yuexingan06.cn

[N08] 生成全排列
来源：http://nw.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://xl.szsharing.cn

PHP:  // 手写递归交换
来源：http://ng.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://yq.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://vr.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://od.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://os.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://yf.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://cm.hahajie.cn

[N09] 栈与队列
来源：http://wv.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zd.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://du.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zy.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hp.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zw.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://so.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lk.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ji.newstarts.cn

[N10] 链表节点定义
来源：http://ox.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fj.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rb.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pt.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ht.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://wf.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dy.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rd.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://du.nszjky.cn

[N11] 二叉树中序遍历
来源：http://os.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kx.szsharing.cn

PHP:  // 手写递归函数
来源：http://kv.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ab.nicolike.cn

Java: // 手写递归
来源：http://mr.huixiangedu.cn

Go:   // 手写递归
来源：http://lt.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xk.huanxung.cn

C#:   // 手写递归
来源：http://hs.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yo.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://az.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ex.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jd.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pc.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qp.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ui.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yo.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xs.yuexingan06.cn


<!-- 参考信息 -->