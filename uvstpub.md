代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://gy.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mx.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://ff.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vb.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lp.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ei.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pp.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vi.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ed.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tg.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kz.chemitech.net.cn

[K05] 深拷贝对象
来源：http://oo.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://fh.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://mf.hnjuh.cn

JS:   structuredClone(obj)
来源：http://eg.hnjuh.cn

TS:   structuredClone(obj)
来源：http://uq.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kb.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yf.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ic.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sh.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://wj.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://em.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kt.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ll.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oi.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wz.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://he.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ho.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hs.szxytkj.cn

[K07] 进制转换
来源：http://yn.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ob.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ru.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kr.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qa.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xy.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lp.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nq.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://in.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://gm.521024.cn

Py:   pickle.dumps(obj)
来源：http://vi.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gb.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://au.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://at.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ph.shtwfgs.cn

Go:   encoding/gob
来源：http://xx.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://rl.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nn.panjiajie.cn

================================================================================
来源：http://vk.szxytkj.cn

L. 网络请求
来源：http://sh.huixinmuqiang.cn

================================================================================
来源：http://jq.colortex.cn

[L01] 发送 GET 请求
来源：http://tx.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dl.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xb.shtwfgs.cn

JS:   await fetch(url)
来源：http://uc.nszjky.cn

TS:   await fetch(url)
来源：http://at.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jy.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://rt.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gc.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ye.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://kk.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://co.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ve.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://te.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lo.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vw.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qz.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pm.szxytkj.cn

[L03] 设置自定义请求头
来源：http://rv.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dg.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://we.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ua.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mo.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yd.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iw.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jm.chemitech.net.cn

[L04] 设置超时
来源：http://td.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ey.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vt.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wy.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qi.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kk.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://in.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://du.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ev.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://hn.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sd.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rz.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xw.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://be.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yg.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hl.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kx.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jg.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://of.shxzskj.cn

Py:   resp.json()
来源：http://oe.colortex.cn

PHP:  json_decode($body, true);
来源：http://ba.nszjky.cn

JS:   await resp.json()
来源：http://ht.9csxet.cn

TS:   await resp.json()
来源：http://ej.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wl.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nh.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ye.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kj.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://kf.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lh.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bm.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://vn.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://zh.haigaiapp.cn

Java: resp.statusCode()
来源：http://qp.hahajie.cn

Go:   resp.StatusCode
来源：http://ou.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://tm.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://rx.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ka.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qv.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://ff.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pe.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wi.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ud.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tq.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://es.521024.cn

================================================================================
来源：http://sw.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://uo.huanxung.cn

================================================================================
来源：http://bv.shxzskj.cn

[M01] 读取命令行参数
来源：http://zr.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://yj.newstarts.cn

PHP:  $argv;  $argc;
来源：http://jt.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://nb.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://py.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://os.colortex.cn

Go:   os.Args[1:]
来源：http://zw.nicolike.cn

Ruby: ARGV
来源：http://jq.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ik.haigaiapp.cn

[M02] 读取环境变量
来源：http://xt.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://mm.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gs.haigaiapp.cn

JS:   process.env.HOME
来源：http://oz.szxytkj.cn

TS:   process.env.HOME
来源：http://gl.shxzskj.cn

Java: System.getenv("HOME")
来源：http://mx.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ti.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://gj.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lv.bjjhwx.cn

[M03] 执行外部命令
来源：http://pw.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mu.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yu.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kw.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ci.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mi.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ut.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rz.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://hp.gzmigu.cn

[M04] 获取当前工作目录
来源：http://jh.nszjky.cn

Py:   os.getcwd()
来源：http://ol.nicolike.cn

PHP:  getcwd();
来源：http://tu.nszjky.cn

JS:   process.cwd()
来源：http://tp.nszjky.cn

TS:   process.cwd()
来源：http://mp.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://xi.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://en.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ii.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yd.shxzukj.cn

[M05] 设置退出码
来源：http://av.nicolike.cn

Py:   sys.exit(1)
来源：http://lx.wgjwhj.cn

PHP:  exit(1);
来源：http://ng.nicolike.cn

JS:   process.exit(1)
来源：http://vu.hahajie.cn

TS:   process.exit(1)
来源：http://hg.yuntaijiaju.cn

Java: System.exit(1)
来源：http://uz.hahajie.cn

Go:   os.Exit(1)
来源：http://xd.huixiangedu.cn

Ruby: exit 1
来源：http://nd.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ak.panjiajie.cn

[M06] 向标准错误输出
来源：http://kt.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://xn.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rc.panjiajie.cn

JS:   console.error("err")
来源：http://bt.9csxet.cn

TS:   console.error("err")
来源：http://vp.gzmigu.cn

Java: System.err.println("err")
来源：http://mq.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wy.jianghongdianzi.cn

Ruby: warn "err"
来源：http://it.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://sx.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://vi.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://ra.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pc.wgjwhj.cn

JS:   require.main === module
来源：http://ae.chemitech.net.cn

TS:   require.main === module
来源：http://kx.szsharing.cn

Java: public static void main(String[] args)
来源：http://ke.lnxyls.cn

Go:   func main()
来源：http://qm.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gd.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://mp.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://rc.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://le.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ut.hahajie.cn

JS:   process.platform;  process.version
来源：http://js.hahajie.cn

TS:   process.platform;  process.version
来源：http://tm.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ph.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://od.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lo.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ei.asd995.cn

================================================================================
来源：http://wo.colortex.cn

N. 数据结构与算法
来源：http://ow.521024.cn

================================================================================
来源：http://tc.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://rb.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hs.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yf.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dp.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tv.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ku.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://oe.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xl.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eo.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://cc.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://xq.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dh.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gc.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hm.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yn.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://lh.szsharing.cn

Ruby: arr.sort
来源：http://rj.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ra.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://jq.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cb.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://uh.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yr.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cu.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://an.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fu.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yi.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xa.521024.cn

[N04] 斐波那契数列
来源：http://zj.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vp.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://id.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pe.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ht.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dz.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mg.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://da.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fy.jctech888.com.cn

[N05] 最大公约数
来源：http://rq.521024.cn

Py:   math.gcd(a, b)
来源：http://vr.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uy.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xa.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://an.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hw.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vs.huanxung.cn

Ruby: a.gcd(b)
来源：http://mn.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pp.szsharing.cn

[N06] 判断回文字符串
来源：http://ji.shxzskj.cn

Py:   s == s[::-1]
来源：http://us.huanxung.cn

PHP:  $s === strrev($s);
来源：http://fv.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://it.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://fg.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qg.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://ly.shxzukj.cn

Ruby: s == s.reverse
来源：http://pu.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yl.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://yr.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qd.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ts.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fl.521024.cn

TS:   // 手写 Map<string, number>
来源：http://jx.huixiangedu.cn

Java: // 手写 HashMap
来源：http://up.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://nk.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ay.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://au.nicolike.cn

[N08] 生成全排列
来源：http://ew.asd995.cn

Py:   itertools.permutations(arr)
来源：http://gz.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://qy.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://vy.9csxet.cn

TS:   // 手写回溯递归
来源：http://ep.asd995.cn

Java: // 手写回溯递归
来源：http://oi.521024.cn

Go:   // 手写回溯递归
来源：http://zu.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://rh.shxzukj.cn

C#:   // 手写回溯递归
来源：http://ah.jctech888.com.cn

[N09] 栈与队列
来源：http://ak.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fk.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wb.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fr.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dn.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ev.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://im.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wh.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ru.szxytkj.cn

[N10] 链表节点定义
来源：http://kv.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pj.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pm.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hf.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://je.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://oa.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tc.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rs.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://be.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://zj.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nd.gzmigu.cn

PHP:  // 手写递归函数
来源：http://yn.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ju.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vp.newstarts.cn

Java: // 手写递归
来源：http://dz.shxzskj.cn

Go:   // 手写递归
来源：http://em.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ag.yuexingan06.cn

C#:   // 手写递归
来源：http://bx.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pu.newstarts.cn


<!-- 参考信息 -->