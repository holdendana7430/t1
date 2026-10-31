代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gz.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bo.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qk.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nq.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dy.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mk.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hv.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ai.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://vt.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://xp.newstarts.cn

JS:   structuredClone(obj)
来源：http://bb.shxzukj.cn

TS:   structuredClone(obj)
来源：http://jt.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rs.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mm.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fv.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://po.asd995.cn

[K06] 解析 URL 查询串
来源：http://lt.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eo.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lg.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ph.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oq.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://na.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tf.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fk.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rs.nicolike.cn

[K07] 进制转换
来源：http://zd.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://do.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://is.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tx.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uv.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sb.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dx.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zp.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ov.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://gg.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://fu.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tx.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://nk.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://ks.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dy.szxytkj.cn

Go:   encoding/gob
来源：http://ou.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://na.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rm.panjiajie.cn

================================================================================
来源：http://qu.huanxung.cn

L. 网络请求
来源：http://ye.muxihuayi.cn

================================================================================
来源：http://xq.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://tn.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iy.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://it.newstarts.cn

JS:   await fetch(url)
来源：http://te.szxytkj.cn

TS:   await fetch(url)
来源：http://yd.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yx.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://eu.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cf.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ae.hnjuh.cn

[L02] 发送 POST JSON
来源：http://dz.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qo.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ai.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yz.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wb.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://se.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ur.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xm.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ry.szsharing.cn

[L03] 设置自定义请求头
来源：http://db.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ni.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xd.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fr.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vs.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://re.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pq.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cj.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fl.jctech888.com.cn

[L04] 设置超时
来源：http://or.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://dl.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jl.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tb.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vp.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qn.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gs.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yz.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://bh.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gh.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wb.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pp.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mq.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gd.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bm.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://am.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kk.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://eq.wgjwhj.cn

Py:   resp.json()
来源：http://ju.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ve.shxzskj.cn

JS:   await resp.json()
来源：http://sz.hnjuh.cn

TS:   await resp.json()
来源：http://fa.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ym.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xp.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://bi.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wg.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://es.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lm.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ja.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://xn.colortex.cn

TS:   resp.ok;  resp.status
来源：http://sg.newstarts.cn

Java: resp.statusCode()
来源：http://lf.szxytkj.cn

Go:   resp.StatusCode
来源：http://zi.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://an.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://jx.nszjky.cn

[L08] 并发请求多个地址
来源：http://aw.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sk.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://du.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ax.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jg.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wm.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ly.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gu.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tj.jianghongdianzi.cn

================================================================================
来源：http://lt.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://gp.panjiajie.cn

================================================================================
来源：http://ym.muxihuayi.cn

[M01] 读取命令行参数
来源：http://bx.huanxung.cn

Py:   sys.argv[1:]
来源：http://qp.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://bv.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://eo.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://gl.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://of.nicolike.cn

Go:   os.Args[1:]
来源：http://ax.chemitech.net.cn

Ruby: ARGV
来源：http://dd.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://dd.nszjky.cn

[M02] 读取环境变量
来源：http://ka.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://rl.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lu.jctech888.com.cn

JS:   process.env.HOME
来源：http://yc.huixiangedu.cn

TS:   process.env.HOME
来源：http://oe.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://hf.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wh.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://af.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wm.panjiajie.cn

[M03] 执行外部命令
来源：http://wh.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yf.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ch.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sj.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ak.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cz.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mr.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zi.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://bv.huanxung.cn

[M04] 获取当前工作目录
来源：http://jm.lnxyls.cn

Py:   os.getcwd()
来源：http://bj.wgjwhj.cn

PHP:  getcwd();
来源：http://vs.huanxung.cn

JS:   process.cwd()
来源：http://eb.gzmigu.cn

TS:   process.cwd()
来源：http://dr.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://yl.yuexingan06.cn

Go:   os.Getwd()
来源：http://wf.yuexingan06.cn

Ruby: Dir.pwd
来源：http://mu.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hh.newstarts.cn

[M05] 设置退出码
来源：http://mq.asd995.cn

Py:   sys.exit(1)
来源：http://nq.chemitech.net.cn

PHP:  exit(1);
来源：http://kr.hnjuh.cn

JS:   process.exit(1)
来源：http://mu.bjjhwx.cn

TS:   process.exit(1)
来源：http://cm.haigaiapp.cn

Java: System.exit(1)
来源：http://ws.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://na.chemitech.net.cn

Ruby: exit 1
来源：http://kj.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jm.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://bf.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://tb.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oa.newstarts.cn

JS:   console.error("err")
来源：http://lp.hahajie.cn

TS:   console.error("err")
来源：http://su.muxihuayi.cn

Java: System.err.println("err")
来源：http://bq.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kt.lnxyls.cn

Ruby: warn "err"
来源：http://hm.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://wm.hahajie.cn

[M07] 判断是否为主入口
来源：http://mx.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://pb.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fq.yuexingan06.cn

JS:   require.main === module
来源：http://ft.shxzukj.cn

TS:   require.main === module
来源：http://wy.huanxung.cn

Java: public static void main(String[] args)
来源：http://nv.jianghongdianzi.cn

Go:   func main()
来源：http://ol.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ui.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://pp.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://pl.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://db.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://os.panjiajie.cn

JS:   process.platform;  process.version
来源：http://fj.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://jf.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://le.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ir.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gf.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.jianghongdianzi.cn

================================================================================
来源：http://eh.yuexingan06.cn

N. 数据结构与算法
来源：http://xl.521024.cn

================================================================================
来源：http://sh.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://yr.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nf.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://as.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xa.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qs.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fm.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://oy.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gm.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ax.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://eu.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fn.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bb.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://be.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vx.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kf.asd995.cn

Go:   slices.Sort(arr)
来源：http://jo.521024.cn

Ruby: arr.sort
来源：http://la.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uh.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://gi.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gx.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://qw.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wn.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pi.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yr.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jp.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eh.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cx.wgjwhj.cn

[N04] 斐波那契数列
来源：http://wq.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mr.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://la.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sr.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hg.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cz.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ig.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vq.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nm.muxihuayi.cn

[N05] 最大公约数
来源：http://rz.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://hk.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://og.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qy.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bq.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hu.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xf.newstarts.cn

Ruby: a.gcd(b)
来源：http://jx.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sd.huixiangedu.cn

[N06] 判断回文字符串
来源：http://aw.haigaiapp.cn

Py:   s == s[::-1]
来源：http://hg.nszjky.cn

PHP:  $s === strrev($s);
来源：http://qc.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://il.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://ou.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://re.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://gf.yuexingan06.cn

Ruby: s == s.reverse
来源：http://yf.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ne.asd995.cn

[N07] 两数之和（返回下标）
来源：http://si.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ml.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sv.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jb.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ee.newstarts.cn

Java: // 手写 HashMap
来源：http://da.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://pg.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ou.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ct.panjiajie.cn

[N08] 生成全排列
来源：http://oj.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://yn.lnxyls.cn

PHP:  // 手写递归交换
来源：http://iv.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://rn.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://sc.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ep.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://xk.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ff.panjiajie.cn

C#:   // 手写回溯递归
来源：http://is.shxzskj.cn

[N09] 栈与队列
来源：http://ky.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://no.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qc.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yu.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ao.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uj.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cc.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://js.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fp.nicolike.cn

[N10] 链表节点定义
来源：http://nw.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fd.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iy.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yj.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pi.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://pr.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ip.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ne.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bn.newstarts.cn

[N11] 二叉树中序遍历
来源：http://kr.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oq.shxzskj.cn

PHP:  // 手写递归函数
来源：http://pp.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lw.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ji.hahajie.cn

Java: // 手写递归
来源：http://jp.nszjky.cn

Go:   // 手写递归
来源：http://qg.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bu.haigaiapp.cn

C#:   // 手写递归
来源：http://mj.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nz.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hq.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kv.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ia.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vh.szsharing.cn


<!-- 参考信息 -->