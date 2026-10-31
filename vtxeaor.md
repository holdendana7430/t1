代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gj.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tm.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ph.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://un.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oj.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gb.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://co.huixiangedu.cn

[K05] 深拷贝对象
来源：http://yf.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://km.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://mg.newstarts.cn

JS:   structuredClone(obj)
来源：http://zn.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://bi.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uz.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ko.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oa.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cq.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://qr.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xb.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qb.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cz.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ob.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qq.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kd.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://is.colortex.cn

[K07] 进制转换
来源：http://ir.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zw.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yn.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yp.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zm.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://if.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vd.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uc.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://jw.asd995.cn

Py:   pickle.dumps(obj)
来源：http://nj.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vb.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ng.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://ga.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zy.hnjuh.cn

Go:   encoding/gob
来源：http://nl.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://zb.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ug.huixinmuqiang.cn

================================================================================
来源：http://fs.newstarts.cn

L. 网络请求
来源：http://ly.hahajie.cn

================================================================================
来源：http://ro.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://la.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tx.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bx.szxytkj.cn

JS:   await fetch(url)
来源：http://fy.haigaiapp.cn

TS:   await fetch(url)
来源：http://qo.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ll.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://dl.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rf.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ql.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ri.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ta.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zd.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uv.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lm.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ia.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qd.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dd.szsharing.cn

[L03] 设置自定义请求头
来源：http://hc.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wi.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wo.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qd.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mw.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ra.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jn.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gc.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cr.muxihuayi.cn

[L04] 设置超时
来源：http://la.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://og.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yc.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wc.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pm.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fe.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dz.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ex.newstarts.cn

[L05] 上传文件（multipart）
来源：http://ai.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wl.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wn.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dy.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nm.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bg.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zz.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zj.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://gm.jianghongdianzi.cn

Py:   resp.json()
来源：http://gu.hahajie.cn

PHP:  json_decode($body, true);
来源：http://nf.haigaiapp.cn

JS:   await resp.json()
来源：http://al.szxytkj.cn

TS:   await resp.json()
来源：http://mi.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pr.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qn.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ch.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://sy.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rg.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vg.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://hi.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ez.9csxet.cn

Java: resp.statusCode()
来源：http://ik.hnjuh.cn

Go:   resp.StatusCode
来源：http://rk.521024.cn

Ruby: resp.code.to_i
来源：http://in.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://jm.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://we.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://po.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://lz.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zq.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://as.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mi.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jv.hahajie.cn

================================================================================
来源：http://hi.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://kv.bjjhwx.cn

================================================================================
来源：http://kw.shtwfgs.cn

[M01] 读取命令行参数
来源：http://hu.shxzskj.cn

Py:   sys.argv[1:]
来源：http://yp.szsharing.cn

PHP:  $argv;  $argc;
来源：http://ay.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://mo.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://dy.521024.cn

Java: args 数组（main 方法参数）
来源：http://ag.hahajie.cn

Go:   os.Args[1:]
来源：http://zi.wgjwhj.cn

Ruby: ARGV
来源：http://mp.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://gf.bjjhwx.cn

[M02] 读取环境变量
来源：http://ln.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://as.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pl.bjjhwx.cn

JS:   process.env.HOME
来源：http://xc.jctech888.com.cn

TS:   process.env.HOME
来源：http://nn.nszjky.cn

Java: System.getenv("HOME")
来源：http://jv.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zy.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://wf.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://na.chemitech.net.cn

[M03] 执行外部命令
来源：http://ym.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nj.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ab.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ze.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jd.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bt.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vl.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vf.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://aq.shxzskj.cn

[M04] 获取当前工作目录
来源：http://qk.yuexingan06.cn

Py:   os.getcwd()
来源：http://ra.bookmarksfly.cn

PHP:  getcwd();
来源：http://lg.jianghongdianzi.cn

JS:   process.cwd()
来源：http://ch.521024.cn

TS:   process.cwd()
来源：http://ji.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ax.521024.cn

Go:   os.Getwd()
来源：http://gk.hnjuh.cn

Ruby: Dir.pwd
来源：http://ut.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://af.nszjky.cn

[M05] 设置退出码
来源：http://xs.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ec.jianghongdianzi.cn

PHP:  exit(1);
来源：http://za.nszjky.cn

JS:   process.exit(1)
来源：http://sa.huixiangedu.cn

TS:   process.exit(1)
来源：http://wa.huanxung.cn

Java: System.exit(1)
来源：http://ke.chemitech.net.cn

Go:   os.Exit(1)
来源：http://ev.yuexingan06.cn

Ruby: exit 1
来源：http://vj.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ij.muxihuayi.cn

[M06] 向标准错误输出
来源：http://eq.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://ix.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fm.shtwfgs.cn

JS:   console.error("err")
来源：http://ld.huixinmuqiang.cn

TS:   console.error("err")
来源：http://wi.panjiajie.cn

Java: System.err.println("err")
来源：http://og.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sl.muxihuayi.cn

Ruby: warn "err"
来源：http://sr.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://kv.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://aa.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://vs.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jm.asd995.cn

JS:   require.main === module
来源：http://up.panjiajie.cn

TS:   require.main === module
来源：http://pk.huanxung.cn

Java: public static void main(String[] args)
来源：http://vr.colortex.cn

Go:   func main()
来源：http://uv.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ai.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://no.colortex.cn

[M08] 获取系统与运行时信息
来源：http://js.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://rz.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://nb.huanxung.cn

JS:   process.platform;  process.version
来源：http://ty.nicolike.cn

TS:   process.platform;  process.version
来源：http://qf.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://za.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zg.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fk.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ey.newstarts.cn

================================================================================
来源：http://tv.shxzskj.cn

N. 数据结构与算法
来源：http://nh.chemitech.net.cn

================================================================================
来源：http://rk.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://ub.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ns.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ma.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zk.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ds.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cq.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://hr.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uk.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fs.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://jw.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://rb.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ny.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://de.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ou.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zd.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://sl.colortex.cn

Ruby: arr.sort
来源：http://xz.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ni.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://ow.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://re.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://xq.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vj.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qt.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ht.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://up.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xz.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bf.panjiajie.cn

[N04] 斐波那契数列
来源：http://dn.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ga.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yb.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wp.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ii.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vt.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ce.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zr.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lo.nszjky.cn

[N05] 最大公约数
来源：http://gs.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://wl.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nr.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://li.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ye.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xp.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ck.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ul.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bq.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://nk.muxihuayi.cn

Py:   s == s[::-1]
来源：http://wq.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://dm.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://ea.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://cy.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lo.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://go.shtwfgs.cn

Ruby: s == s.reverse
来源：http://re.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ns.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://pa.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wm.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qn.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zm.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ca.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ez.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://lo.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ex.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ga.szsharing.cn

[N08] 生成全排列
来源：http://wf.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ll.nicolike.cn

PHP:  // 手写递归交换
来源：http://mc.szxytkj.cn

JS:   // 手写回溯递归
来源：http://dl.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://jl.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://rz.panjiajie.cn

Go:   // 手写回溯递归
来源：http://lu.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://zc.szsharing.cn

C#:   // 手写回溯递归
来源：http://kf.jianghongdianzi.cn

[N09] 栈与队列
来源：http://tz.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lp.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ls.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xx.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ga.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ty.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://en.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://od.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qg.shxzskj.cn

[N10] 链表节点定义
来源：http://pd.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nc.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lt.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jy.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jt.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://mi.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ie.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jl.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vn.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://yk.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hh.nicolike.cn

PHP:  // 手写递归函数
来源：http://ya.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ye.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kk.asd995.cn

Java: // 手写递归
来源：http://ok.shxzskj.cn

Go:   // 手写递归
来源：http://yk.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vj.huixiangedu.cn

C#:   // 手写递归
来源：http://kl.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hd.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oa.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vq.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dl.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ob.hahajie.cn


<!-- 参考信息 -->