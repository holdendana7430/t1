代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://us.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://er.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lp.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sd.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yb.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aj.nicolike.cn

[K04] 读取 JSON 文件
来源：http://uf.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bl.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tz.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cp.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fl.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ds.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kw.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qo.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fd.szsharing.cn

[K05] 深拷贝对象
来源：http://nh.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://mv.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://be.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://qo.hnjuh.cn

TS:   structuredClone(obj)
来源：http://kz.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ig.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ic.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fk.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fu.nszjky.cn

[K06] 解析 URL 查询串
来源：http://ic.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://os.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iv.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sq.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tz.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rp.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hp.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zv.bookmarksfly.cn

[K07] 进制转换
来源：http://na.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pa.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://no.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vz.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://di.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pp.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gq.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ch.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rz.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://ay.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://dg.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lp.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zx.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://wg.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ap.jctech888.com.cn

Go:   encoding/gob
来源：http://iw.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://fp.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qp.huixinmuqiang.cn

================================================================================
来源：http://hk.szsharing.cn

L. 网络请求
来源：http://ry.huixiangedu.cn

================================================================================
来源：http://nm.hahajie.cn

[L01] 发送 GET 请求
来源：http://na.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://co.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mo.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://by.muxihuayi.cn

TS:   await fetch(url)
来源：http://bm.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xb.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ys.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ru.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://va.colortex.cn

[L02] 发送 POST JSON
来源：http://qd.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://op.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xm.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ie.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rh.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iz.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ws.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fb.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://nz.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cg.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ge.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dj.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bp.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lc.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ck.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xa.colortex.cn

[L04] 设置超时
来源：http://yy.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://dl.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gs.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://je.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yh.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ut.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lz.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://px.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lf.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://xz.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ei.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ka.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bz.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yy.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vu.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rh.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bj.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://or.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://rw.shxzskj.cn

Py:   resp.json()
来源：http://ge.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://js.jianghongdianzi.cn

JS:   await resp.json()
来源：http://at.muxihuayi.cn

TS:   await resp.json()
来源：http://zm.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ar.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vr.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://bb.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cz.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://gd.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tl.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oy.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://pf.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ho.wgjwhj.cn

Java: resp.statusCode()
来源：http://zp.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://qh.hnjuh.cn

Ruby: resp.code.to_i
来源：http://tl.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://gl.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://rd.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yb.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://cm.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uq.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mu.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bl.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xi.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vp.shxzskj.cn

================================================================================
来源：http://nw.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://iv.szsharing.cn

================================================================================
来源：http://vu.hahajie.cn

[M01] 读取命令行参数
来源：http://fp.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://xe.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://op.colortex.cn

JS:   process.argv.slice(2)
来源：http://qf.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://sh.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://af.chemitech.net.cn

Go:   os.Args[1:]
来源：http://ei.jctech888.com.cn

Ruby: ARGV
来源：http://dj.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://id.muxihuayi.cn

[M02] 读取环境变量
来源：http://mf.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://dl.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oh.szsharing.cn

JS:   process.env.HOME
来源：http://iw.shxzskj.cn

TS:   process.env.HOME
来源：http://ve.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://kg.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://be.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://el.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xh.chemitech.net.cn

[M03] 执行外部命令
来源：http://qb.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://en.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oi.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pw.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xz.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lo.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xy.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mi.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://tv.lnxyls.cn

[M04] 获取当前工作目录
来源：http://fw.bjjhwx.cn

Py:   os.getcwd()
来源：http://mm.haigaiapp.cn

PHP:  getcwd();
来源：http://ii.haigaiapp.cn

JS:   process.cwd()
来源：http://hu.haigaiapp.cn

TS:   process.cwd()
来源：http://wv.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://zd.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://do.szxytkj.cn

Ruby: Dir.pwd
来源：http://tc.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qz.nicolike.cn

[M05] 设置退出码
来源：http://zh.lnxyls.cn

Py:   sys.exit(1)
来源：http://en.nszjky.cn

PHP:  exit(1);
来源：http://ge.bjjhwx.cn

JS:   process.exit(1)
来源：http://ct.newstarts.cn

TS:   process.exit(1)
来源：http://az.bjjhwx.cn

Java: System.exit(1)
来源：http://xm.shxzskj.cn

Go:   os.Exit(1)
来源：http://vu.szxytkj.cn

Ruby: exit 1
来源：http://lg.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rv.shxzskj.cn

[M06] 向标准错误输出
来源：http://ml.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://ay.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://me.huanxung.cn

JS:   console.error("err")
来源：http://vc.szxytkj.cn

TS:   console.error("err")
来源：http://eh.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://nm.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yu.panjiajie.cn

Ruby: warn "err"
来源：http://pb.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://om.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://xs.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://ra.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wu.yuntaijiaju.cn

JS:   require.main === module
来源：http://bd.shxzukj.cn

TS:   require.main === module
来源：http://ws.shxzukj.cn

Java: public static void main(String[] args)
来源：http://sh.szxytkj.cn

Go:   func main()
来源：http://gi.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mx.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://wj.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://im.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://bn.nicolike.cn

JS:   process.platform;  process.version
来源：http://ec.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://ei.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sq.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sk.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://md.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.shxzukj.cn

================================================================================
来源：http://cp.521024.cn

N. 数据结构与算法
来源：http://ai.huixiangedu.cn

================================================================================
来源：http://jc.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://rf.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ce.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sr.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rk.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xs.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vp.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://yr.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kd.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://zc.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://pa.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ai.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://un.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vv.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zd.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://wp.nicolike.cn

Ruby: arr.sort
来源：http://fg.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zf.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://yp.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sc.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://tx.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rq.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hj.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rs.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ew.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wh.shxzskj.cn

[N04] 斐波那契数列
来源：http://bv.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wq.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ah.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pi.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hg.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rx.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ys.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jw.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fh.jctech888.com.cn

[N05] 最大公约数
来源：http://hz.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://kr.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ut.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pq.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gv.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tl.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://gk.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ft.nicolike.cn

[N06] 判断回文字符串
来源：http://dm.huanxung.cn

Py:   s == s[::-1]
来源：http://yo.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ky.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://pk.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://ve.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mj.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ez.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ee.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hw.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://bm.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lp.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sw.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://aq.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://lu.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://ps.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ta.hnjuh.cn

Ruby: // 手写 Hash
来源：http://wq.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cz.wgjwhj.cn

[N08] 生成全排列
来源：http://sl.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://bl.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://rm.colortex.cn

JS:   // 手写回溯递归
来源：http://tf.colortex.cn

TS:   // 手写回溯递归
来源：http://zo.newstarts.cn

Java: // 手写回溯递归
来源：http://av.nicolike.cn

Go:   // 手写回溯递归
来源：http://rz.521024.cn

Ruby: arr.permutation.to_a
来源：http://og.colortex.cn

C#:   // 手写回溯递归
来源：http://xy.newstarts.cn

[N09] 栈与队列
来源：http://qd.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pl.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wr.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tr.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://in.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xm.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xj.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ww.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ui.521024.cn

[N10] 链表节点定义
来源：http://dg.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bn.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wn.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ue.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ok.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://pn.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uc.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sw.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ja.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://vv.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nx.hnjuh.cn

PHP:  // 手写递归函数
来源：http://np.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bq.shxzukj.cn

Java: // 手写递归
来源：http://nt.hahajie.cn


<!-- 参考信息 -->