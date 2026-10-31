代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ag.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://gn.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fh.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qf.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sn.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qu.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wr.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rp.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dv.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wm.hahajie.cn

[K04] 读取 JSON 文件
来源：http://ij.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://io.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dp.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://te.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wc.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ip.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yw.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kr.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yb.chemitech.net.cn

[K05] 深拷贝对象
来源：http://mq.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://ht.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://pa.panjiajie.cn

JS:   structuredClone(obj)
来源：http://kt.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://qz.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kf.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tj.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qo.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fn.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://vg.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kx.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kt.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://il.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hf.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gg.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mo.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gb.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cj.szxytkj.cn

[K07] 进制转换
来源：http://el.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ap.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xi.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eb.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qf.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ri.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kp.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cy.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://il.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://bz.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://fy.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://on.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://ns.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://zs.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dx.panjiajie.cn

Go:   encoding/gob
来源：http://aq.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://ug.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tp.gzmigu.cn

================================================================================
来源：http://wz.wgjwhj.cn

L. 网络请求
来源：http://ap.nszjky.cn

================================================================================
来源：http://cc.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://bs.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sa.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nl.9csxet.cn

JS:   await fetch(url)
来源：http://py.gzmigu.cn

TS:   await fetch(url)
来源：http://yw.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gh.521024.cn

Go:   resp, err := http.Get(url)
来源：http://nq.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://by.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://td.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ev.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lv.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vb.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jn.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wu.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pv.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ji.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rp.shxzskj.cn

[L03] 设置自定义请求头
来源：http://ve.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vz.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://te.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ic.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ok.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ql.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gk.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yr.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mk.shxzskj.cn

[L04] 设置超时
来源：http://gt.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://nr.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oe.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oa.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ul.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rq.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nk.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hm.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ui.nicolike.cn

[L05] 上传文件（multipart）
来源：http://zo.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bd.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wa.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ac.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fc.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vk.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wp.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xp.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://go.9csxet.cn

[L06] 解析响应为 JSON
来源：http://uj.bookmarksfly.cn

Py:   resp.json()
来源：http://wu.newstarts.cn

PHP:  json_decode($body, true);
来源：http://rj.nszjky.cn

JS:   await resp.json()
来源：http://rt.jctech888.com.cn

TS:   await resp.json()
来源：http://kk.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ga.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iv.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://pa.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xp.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://fx.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ct.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ze.asd995.cn

JS:   resp.ok;  resp.status
来源：http://kd.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://ly.bookmarksfly.cn

Java: resp.statusCode()
来源：http://ji.asd995.cn

Go:   resp.StatusCode
来源：http://sa.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://kl.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://uj.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ao.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nj.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://xa.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ct.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sb.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ta.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iz.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ix.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xt.hnjuh.cn

================================================================================
来源：http://jl.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://eu.shxzskj.cn

================================================================================
来源：http://ej.yuexingan06.cn

[M01] 读取命令行参数
来源：http://cd.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://rk.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://kj.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://go.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://rk.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://oz.shxzskj.cn

Go:   os.Args[1:]
来源：http://pf.wgjwhj.cn

Ruby: ARGV
来源：http://cr.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://eg.nicolike.cn

[M02] 读取环境变量
来源：http://lc.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://wn.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lj.panjiajie.cn

JS:   process.env.HOME
来源：http://bd.gzmigu.cn

TS:   process.env.HOME
来源：http://sa.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://sk.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sk.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://mv.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cv.shxzukj.cn

[M03] 执行外部命令
来源：http://ee.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bo.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ff.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qr.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lw.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rt.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qh.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xj.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ce.newstarts.cn

[M04] 获取当前工作目录
来源：http://tu.muxihuayi.cn

Py:   os.getcwd()
来源：http://am.hnjuh.cn

PHP:  getcwd();
来源：http://jm.nicolike.cn

JS:   process.cwd()
来源：http://bg.huixinmuqiang.cn

TS:   process.cwd()
来源：http://zg.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bq.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://nt.hahajie.cn

Ruby: Dir.pwd
来源：http://yo.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zn.jctech888.com.cn

[M05] 设置退出码
来源：http://qv.haigaiapp.cn

Py:   sys.exit(1)
来源：http://tr.gzmigu.cn

PHP:  exit(1);
来源：http://vo.bjjhwx.cn

JS:   process.exit(1)
来源：http://si.bjjhwx.cn

TS:   process.exit(1)
来源：http://bx.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ll.hnjuh.cn

Go:   os.Exit(1)
来源：http://eu.haigaiapp.cn

Ruby: exit 1
来源：http://pb.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ik.lnxyls.cn

[M06] 向标准错误输出
来源：http://ti.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://fl.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mo.huixinmuqiang.cn

JS:   console.error("err")
来源：http://im.hnjuh.cn

TS:   console.error("err")
来源：http://ky.nicolike.cn

Java: System.err.println("err")
来源：http://xc.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uh.chemitech.net.cn

Ruby: warn "err"
来源：http://di.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://rw.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://jy.521024.cn

Py:   if __name__ == "__main__":
来源：http://uz.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qh.hahajie.cn

JS:   require.main === module
来源：http://dx.jianghongdianzi.cn

TS:   require.main === module
来源：http://kt.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://vs.lnxyls.cn

Go:   func main()
来源：http://mo.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yw.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://nk.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://yn.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://lw.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://vl.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://df.shxzukj.cn

TS:   process.platform;  process.version
来源：http://tw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xy.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sq.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nr.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vl.haigaiapp.cn

================================================================================
来源：http://vz.newstarts.cn

N. 数据结构与算法
来源：http://jr.jianghongdianzi.cn

================================================================================
来源：http://ws.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://tv.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ru.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://au.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zi.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ue.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lf.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://so.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iv.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ss.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://qm.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kj.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lu.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yv.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uy.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cv.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://xu.newstarts.cn

Ruby: arr.sort
来源：http://hw.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mp.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://zi.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bh.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://cu.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gd.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dq.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qk.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qh.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hr.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://za.huanxung.cn

[N04] 斐波那契数列
来源：http://ap.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qm.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ws.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bh.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gh.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rk.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gy.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xd.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kc.nicolike.cn

[N05] 最大公约数
来源：http://bp.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://as.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xk.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bw.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ta.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qj.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rr.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://zx.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mp.gzmigu.cn

[N06] 判断回文字符串
来源：http://zk.gzmigu.cn

Py:   s == s[::-1]
来源：http://hc.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ph.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ka.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://gg.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rt.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://sw.gzmigu.cn

Ruby: s == s.reverse
来源：http://aq.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://my.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ct.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cu.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://di.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cl.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://jd.shxzukj.cn

Java: // 手写 HashMap
来源：http://qb.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://bc.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://lo.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rp.yuntaijiaju.cn

[N08] 生成全排列
来源：http://jr.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://us.gzmigu.cn

PHP:  // 手写递归交换
来源：http://je.9csxet.cn

JS:   // 手写回溯递归
来源：http://zh.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://vp.bjjhwx.cn

Java: // 手写回溯递归
来源：http://al.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://tq.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://ld.shxzskj.cn

C#:   // 手写回溯递归
来源：http://jh.muxihuayi.cn

[N09] 栈与队列
来源：http://ot.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ky.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bk.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zi.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wk.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bm.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://le.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://no.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ld.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://cp.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ia.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qp.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sg.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pf.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ws.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nt.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qu.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bc.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://td.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ge.szsharing.cn


<!-- 参考信息 -->