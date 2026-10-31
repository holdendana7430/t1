代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://ii.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pz.newstarts.cn

[K04] 读取 JSON 文件
来源：http://do.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sg.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vv.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pe.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hp.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xe.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://te.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://te.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sx.huanxung.cn

[K05] 深拷贝对象
来源：http://cz.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://qw.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://vb.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://fb.shxzskj.cn

TS:   structuredClone(obj)
来源：http://nt.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dh.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pd.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://th.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://px.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ry.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sw.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jp.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wi.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lz.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ba.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bn.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eq.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://js.shxzukj.cn

[K07] 进制转换
来源：http://zt.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gb.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wc.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rs.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nm.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zw.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dz.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ty.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pa.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ga.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://tl.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ye.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://gt.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://wy.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ty.shxzukj.cn

Go:   encoding/gob
来源：http://ya.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://ih.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xh.hnjuh.cn

================================================================================
来源：http://bn.colortex.cn

L. 网络请求
来源：http://sm.chemitech.net.cn

================================================================================
来源：http://tk.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://jh.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://op.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xc.chemitech.net.cn

JS:   await fetch(url)
来源：http://au.szxytkj.cn

TS:   await fetch(url)
来源：http://iz.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ph.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ee.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tt.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nl.asd995.cn

[L02] 发送 POST JSON
来源：http://yf.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oz.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jv.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vq.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qg.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tq.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://en.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ob.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ds.hahajie.cn

[L03] 设置自定义请求头
来源：http://nd.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tm.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ll.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fg.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bk.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vj.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gz.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://by.colortex.cn

[L04] 设置超时
来源：http://ke.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://vd.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tt.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://na.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iy.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qm.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ea.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gk.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ie.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ff.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ab.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qq.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ip.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rm.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vw.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zu.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gd.nicolike.cn

[L06] 解析响应为 JSON
来源：http://ge.szxytkj.cn

Py:   resp.json()
来源：http://gt.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://dr.szxytkj.cn

JS:   await resp.json()
来源：http://vm.hahajie.cn

TS:   await resp.json()
来源：http://on.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wi.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yk.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://oa.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zc.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://br.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pk.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yq.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://ha.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://uv.muxihuayi.cn

Java: resp.statusCode()
来源：http://wh.shtwfgs.cn

Go:   resp.StatusCode
来源：http://ma.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://wz.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://qy.521024.cn

[L08] 并发请求多个地址
来源：http://sf.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://th.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://br.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xd.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://df.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ti.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cr.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://is.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aj.colortex.cn

================================================================================
来源：http://yh.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://sj.huanxung.cn

================================================================================
来源：http://lm.newstarts.cn

[M01] 读取命令行参数
来源：http://uv.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://al.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://lk.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ek.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://sc.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://qg.shxzskj.cn

Go:   os.Args[1:]
来源：http://wv.haigaiapp.cn

Ruby: ARGV
来源：http://pp.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://gs.muxihuayi.cn

[M02] 读取环境变量
来源：http://ji.colortex.cn

Py:   os.environ.get("HOME")
来源：http://rc.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yp.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://qz.huanxung.cn

TS:   process.env.HOME
来源：http://yf.9csxet.cn

Java: System.getenv("HOME")
来源：http://gt.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tx.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://dl.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fr.szsharing.cn

[M03] 执行外部命令
来源：http://eu.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pl.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://th.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pf.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uj.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ly.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dp.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yd.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://ze.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://lw.bookmarksfly.cn

Py:   os.getcwd()
来源：http://kj.9csxet.cn

PHP:  getcwd();
来源：http://jj.wgjwhj.cn

JS:   process.cwd()
来源：http://ss.jianghongdianzi.cn

TS:   process.cwd()
来源：http://db.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://de.bookmarksfly.cn

Go:   os.Getwd()
来源：http://uf.panjiajie.cn

Ruby: Dir.pwd
来源：http://vq.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lw.yuexingan06.cn

[M05] 设置退出码
来源：http://hc.asd995.cn

Py:   sys.exit(1)
来源：http://us.huanxung.cn

PHP:  exit(1);
来源：http://cj.wgjwhj.cn

JS:   process.exit(1)
来源：http://cp.hahajie.cn

TS:   process.exit(1)
来源：http://gh.jianghongdianzi.cn

Java: System.exit(1)
来源：http://zo.asd995.cn

Go:   os.Exit(1)
来源：http://tw.szxytkj.cn

Ruby: exit 1
来源：http://cd.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cm.hahajie.cn

[M06] 向标准错误输出
来源：http://ya.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://yu.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qf.huixinmuqiang.cn

JS:   console.error("err")
来源：http://bp.hahajie.cn

TS:   console.error("err")
来源：http://ry.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://wi.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fp.yuexingan06.cn

Ruby: warn "err"
来源：http://mf.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://ao.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://mw.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://xo.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uu.shtwfgs.cn

JS:   require.main === module
来源：http://qp.shxzukj.cn

TS:   require.main === module
来源：http://gw.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://hy.haigaiapp.cn

Go:   func main()
来源：http://lp.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nm.huanxung.cn

C#:   static void Main(string[] args)
来源：http://ix.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://qs.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://su.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://dz.szxytkj.cn

JS:   process.platform;  process.version
来源：http://ob.nicolike.cn

TS:   process.platform;  process.version
来源：http://ag.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mo.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bv.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ls.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pp.newstarts.cn

================================================================================
来源：http://le.shxzskj.cn

N. 数据结构与算法
来源：http://rk.nszjky.cn

================================================================================
来源：http://pf.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://lp.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bt.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hm.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mu.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oy.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://nf.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://he.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uj.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://tr.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://fr.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hf.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aq.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dq.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fw.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://bo.haigaiapp.cn

Ruby: arr.sort
来源：http://cs.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tc.521024.cn

[N03] 快速排序（分治示例）
来源：http://wf.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hn.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://mr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sh.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://se.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mw.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oe.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oh.wgjwhj.cn

[N04] 斐波那契数列
来源：http://jl.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://as.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lu.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pp.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://af.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nz.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nn.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zh.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hh.9csxet.cn

[N05] 最大公约数
来源：http://jx.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ga.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://an.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oz.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cc.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dm.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bh.szxytkj.cn

Ruby: a.gcd(b)
来源：http://eu.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sr.521024.cn

[N06] 判断回文字符串
来源：http://lb.yuexingan06.cn

Py:   s == s[::-1]
来源：http://ji.szsharing.cn

PHP:  $s === strrev($s);
来源：http://hf.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://fj.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://vu.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wi.hahajie.cn

Go:   // 双指针从两端比较
来源：http://lw.huixiangedu.cn

Ruby: s == s.reverse
来源：http://sx.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://la.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://fx.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hx.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dj.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mk.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://bk.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://su.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://so.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://ti.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hp.chemitech.net.cn

[N08] 生成全排列
来源：http://ky.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://rt.9csxet.cn

PHP:  // 手写递归交换
来源：http://vd.newstarts.cn

JS:   // 手写回溯递归
来源：http://fg.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://cn.lnxyls.cn

Java: // 手写回溯递归
来源：http://on.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://jr.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://sl.shxzskj.cn

C#:   // 手写回溯递归
来源：http://lq.nicolike.cn

[N09] 栈与队列
来源：http://zb.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kp.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sx.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mz.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nl.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zq.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ft.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ia.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://it.bookmarksfly.cn

[N10] 链表节点定义
来源：http://rb.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kq.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jj.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://en.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zs.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://ct.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wq.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ez.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://if.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://kt.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cd.shxzskj.cn

PHP:  // 手写递归函数
来源：http://dt.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ds.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ng.yuexingan06.cn

Java: // 手写递归
来源：http://bu.huixiangedu.cn

Go:   // 手写递归
来源：http://mm.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bm.chemitech.net.cn

C#:   // 手写递归
来源：http://hz.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bc.chemitech.net.cn


<!-- 参考信息 -->