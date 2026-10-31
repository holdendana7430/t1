代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pv.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uh.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kf.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://na.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jq.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vo.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ll.yuexingan06.cn

[K05] 深拷贝对象
来源：http://ws.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://qj.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://za.szsharing.cn

JS:   structuredClone(obj)
来源：http://us.hahajie.cn

TS:   structuredClone(obj)
来源：http://do.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vp.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ul.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wr.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mp.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://uf.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rx.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vd.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nu.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aa.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gf.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bq.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gr.szxytkj.cn

[K07] 进制转换
来源：http://qt.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kn.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lz.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zd.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xa.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ke.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://al.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qw.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://pe.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://di.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tb.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ab.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://ur.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zo.jctech888.com.cn

Go:   encoding/gob
来源：http://ye.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://qd.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fx.huanxung.cn

================================================================================
来源：http://nv.lnxyls.cn

L. 网络请求
来源：http://ft.bjjhwx.cn

================================================================================
来源：http://sx.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://oi.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eb.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kv.panjiajie.cn

JS:   await fetch(url)
来源：http://tp.shxzskj.cn

TS:   await fetch(url)
来源：http://hp.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kq.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://hc.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ax.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gu.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://df.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://al.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://px.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ro.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nu.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jt.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://we.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qs.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qi.szxytkj.cn

[L03] 设置自定义请求头
来源：http://df.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yc.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ha.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sl.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ss.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://re.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hs.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iy.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yq.hahajie.cn

[L04] 设置超时
来源：http://li.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://ni.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ot.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wy.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://en.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dz.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sw.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ir.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tz.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://qn.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ch.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dp.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mm.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fd.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vw.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rp.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ci.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mc.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://mw.muxihuayi.cn

Py:   resp.json()
来源：http://xy.9csxet.cn

PHP:  json_decode($body, true);
来源：http://wl.wgjwhj.cn

JS:   await resp.json()
来源：http://lm.huanxung.cn

TS:   await resp.json()
来源：http://fm.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vr.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://od.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dt.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://on.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sq.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://je.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://gy.shxzskj.cn

Java: resp.statusCode()
来源：http://pk.hahajie.cn

Go:   resp.StatusCode
来源：http://wj.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://vx.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://jo.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://zr.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aq.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://fo.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wi.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kn.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nf.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ko.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ic.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aq.huixiangedu.cn

================================================================================
来源：http://ej.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://hv.huixinmuqiang.cn

================================================================================
来源：http://pi.haigaiapp.cn

[M01] 读取命令行参数
来源：http://ku.gzmigu.cn

Py:   sys.argv[1:]
来源：http://sl.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://sq.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://vk.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ur.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://da.lnxyls.cn

Go:   os.Args[1:]
来源：http://pr.huixinmuqiang.cn

Ruby: ARGV
来源：http://js.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://bl.gzmigu.cn

[M02] 读取环境变量
来源：http://bg.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://mg.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ep.lnxyls.cn

JS:   process.env.HOME
来源：http://qa.nicolike.cn

TS:   process.env.HOME
来源：http://hd.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://wp.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wq.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://sa.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ga.panjiajie.cn

[M03] 执行外部命令
来源：http://ym.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pp.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://si.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lz.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ed.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://io.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pr.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uf.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://xc.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://wv.jctech888.com.cn

Py:   os.getcwd()
来源：http://bh.szxytkj.cn

PHP:  getcwd();
来源：http://gj.shxzskj.cn

JS:   process.cwd()
来源：http://km.szsharing.cn

TS:   process.cwd()
来源：http://rw.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://in.szxytkj.cn

Go:   os.Getwd()
来源：http://je.gzmigu.cn

Ruby: Dir.pwd
来源：http://ts.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hr.haigaiapp.cn

[M05] 设置退出码
来源：http://lk.szxytkj.cn

Py:   sys.exit(1)
来源：http://ur.haigaiapp.cn

PHP:  exit(1);
来源：http://sh.9csxet.cn

JS:   process.exit(1)
来源：http://ve.shtwfgs.cn

TS:   process.exit(1)
来源：http://dz.shxzskj.cn

Java: System.exit(1)
来源：http://yi.asd995.cn

Go:   os.Exit(1)
来源：http://fa.nszjky.cn

Ruby: exit 1
来源：http://ry.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mu.huanxung.cn

[M06] 向标准错误输出
来源：http://on.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://az.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cy.colortex.cn

JS:   console.error("err")
来源：http://gv.colortex.cn

TS:   console.error("err")
来源：http://gy.9csxet.cn

Java: System.err.println("err")
来源：http://uc.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://as.panjiajie.cn

Ruby: warn "err"
来源：http://lx.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://dt.panjiajie.cn

[M07] 判断是否为主入口
来源：http://lq.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://gz.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uw.colortex.cn

JS:   require.main === module
来源：http://yq.hnjuh.cn

TS:   require.main === module
来源：http://io.panjiajie.cn

Java: public static void main(String[] args)
来源：http://bb.jctech888.com.cn

Go:   func main()
来源：http://ms.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jz.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://ia.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://ct.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://bb.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://ai.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://bi.huanxung.cn

TS:   process.platform;  process.version
来源：http://fs.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gg.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ky.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ns.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nt.panjiajie.cn

================================================================================
来源：http://uw.haigaiapp.cn

N. 数据结构与算法
来源：http://aa.panjiajie.cn

================================================================================
来源：http://vq.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://im.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://es.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zg.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ah.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lz.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ds.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jm.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lb.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://yv.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://vc.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oc.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uj.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ii.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pe.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://tn.haigaiapp.cn

Ruby: arr.sort
来源：http://ff.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lz.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://mp.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ab.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://yv.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jz.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bd.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ve.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lq.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sc.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cz.asd995.cn

[N04] 斐波那契数列
来源：http://tt.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ix.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bh.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kv.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cx.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gt.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yr.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fq.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kw.hnjuh.cn

[N05] 最大公约数
来源：http://dv.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://cx.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vv.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jm.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oq.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dk.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zr.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://ww.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sm.jctech888.com.cn

[N06] 判断回文字符串
来源：http://ri.wgjwhj.cn

Py:   s == s[::-1]
来源：http://dn.nszjky.cn

PHP:  $s === strrev($s);
来源：http://ht.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://fq.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://jf.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ox.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://qq.shxzukj.cn

Ruby: s == s.reverse
来源：http://xn.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ie.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://mz.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ib.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oe.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dd.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://dy.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://aa.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://yn.shxzukj.cn

Ruby: // 手写 Hash
来源：http://xa.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://td.colortex.cn

[N08] 生成全排列
来源：http://ju.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://jo.gzmigu.cn

PHP:  // 手写递归交换
来源：http://tw.hnjuh.cn

JS:   // 手写回溯递归
来源：http://fm.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://rv.shtwfgs.cn

Java: // 手写回溯递归
来源：http://ar.521024.cn

Go:   // 手写回溯递归
来源：http://wt.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://xt.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://zj.shxzukj.cn

[N09] 栈与队列
来源：http://nv.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nj.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hk.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bo.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hg.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lw.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tu.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://za.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hh.yuexingan06.cn

[N10] 链表节点定义
来源：http://ma.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tx.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mh.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pw.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hm.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://jp.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://za.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wd.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ph.hahajie.cn

[N11] 二叉树中序遍历
来源：http://nj.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gt.lnxyls.cn

PHP:  // 手写递归函数
来源：http://wm.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lq.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qu.jianghongdianzi.cn

Java: // 手写递归
来源：http://fh.yuexingan06.cn

Go:   // 手写递归
来源：http://ck.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hd.szsharing.cn

C#:   // 手写递归
来源：http://vg.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lq.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fg.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gn.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tv.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jb.hahajie.cn


<!-- 参考信息 -->