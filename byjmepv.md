代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ex.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lz.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pn.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ij.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ve.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rz.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tj.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cr.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pg.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ii.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://zi.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rl.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lr.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nc.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ab.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sa.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oz.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ln.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dh.yuexingan06.cn

[K05] 深拷贝对象
来源：http://wo.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://oz.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://of.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://er.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://pq.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fv.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qd.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dp.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dm.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://tu.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ua.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bq.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dq.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fx.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://km.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gp.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sl.nicolike.cn

[K07] 进制转换
来源：http://oi.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yu.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qe.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yx.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dp.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sy.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aj.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rb.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ik.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://zu.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://nm.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://px.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://oo.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://rp.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kb.jianghongdianzi.cn

Go:   encoding/gob
来源：http://zh.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ho.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bs.yuntaijiaju.cn

================================================================================
来源：http://ic.szsharing.cn

L. 网络请求
来源：http://lz.bjjhwx.cn

================================================================================
来源：http://as.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://eg.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ud.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qj.colortex.cn

JS:   await fetch(url)
来源：http://uo.chemitech.net.cn

TS:   await fetch(url)
来源：http://xd.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cs.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ro.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zr.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pp.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://xh.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://la.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nw.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fl.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nd.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hx.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dn.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://io.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rj.nicolike.cn

[L03] 设置自定义请求头
来源：http://ny.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ln.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mq.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gp.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ot.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rd.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wg.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zp.shtwfgs.cn

[L04] 设置超时
来源：http://vy.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://gg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://co.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://am.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zp.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gy.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fu.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kr.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ve.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ug.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ny.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wj.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mc.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jc.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lx.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dg.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qx.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://un.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://ci.521024.cn

Py:   resp.json()
来源：http://bk.nszjky.cn

PHP:  json_decode($body, true);
来源：http://mo.muxihuayi.cn

JS:   await resp.json()
来源：http://am.huixiangedu.cn

TS:   await resp.json()
来源：http://nq.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xo.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rx.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://zb.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kl.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://rd.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bm.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cu.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://mr.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://in.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://wm.szsharing.cn

Go:   resp.StatusCode
来源：http://yg.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://fz.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://gq.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://yt.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jw.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://wq.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://db.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bn.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dj.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tb.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ne.colortex.cn

================================================================================
来源：http://ay.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://xc.yuexingan06.cn

================================================================================
来源：http://cn.wgjwhj.cn

[M01] 读取命令行参数
来源：http://sb.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://cm.colortex.cn

PHP:  $argv;  $argc;
来源：http://zp.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://nq.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://eg.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://sf.shtwfgs.cn

Go:   os.Args[1:]
来源：http://tr.szsharing.cn

Ruby: ARGV
来源：http://lh.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://bz.lnxyls.cn

[M02] 读取环境变量
来源：http://wg.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://bf.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ji.lnxyls.cn

JS:   process.env.HOME
来源：http://uy.shxzukj.cn

TS:   process.env.HOME
来源：http://az.huanxung.cn

Java: System.getenv("HOME")
来源：http://ga.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://io.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://mq.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yg.9csxet.cn

[M03] 执行外部命令
来源：http://bl.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jx.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wi.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yv.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ks.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://he.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://to.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uc.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://eu.szxytkj.cn

[M04] 获取当前工作目录
来源：http://mx.panjiajie.cn

Py:   os.getcwd()
来源：http://uc.szsharing.cn

PHP:  getcwd();
来源：http://ms.szsharing.cn

JS:   process.cwd()
来源：http://up.nicolike.cn

TS:   process.cwd()
来源：http://bw.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://co.hahajie.cn

Go:   os.Getwd()
来源：http://xx.huanxung.cn

Ruby: Dir.pwd
来源：http://ox.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lv.bookmarksfly.cn

[M05] 设置退出码
来源：http://ep.521024.cn

Py:   sys.exit(1)
来源：http://pp.huixiangedu.cn

PHP:  exit(1);
来源：http://jy.jctech888.com.cn

JS:   process.exit(1)
来源：http://qo.jctech888.com.cn

TS:   process.exit(1)
来源：http://qt.chemitech.net.cn

Java: System.exit(1)
来源：http://qb.asd995.cn

Go:   os.Exit(1)
来源：http://ei.newstarts.cn

Ruby: exit 1
来源：http://zh.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tm.panjiajie.cn

[M06] 向标准错误输出
来源：http://xf.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://gn.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ym.chemitech.net.cn

JS:   console.error("err")
来源：http://nl.521024.cn

TS:   console.error("err")
来源：http://py.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://gg.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gv.szsharing.cn

Ruby: warn "err"
来源：http://nv.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ka.newstarts.cn

[M07] 判断是否为主入口
来源：http://zp.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://fj.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://up.chemitech.net.cn

JS:   require.main === module
来源：http://qk.yuntaijiaju.cn

TS:   require.main === module
来源：http://oj.szsharing.cn

Java: public static void main(String[] args)
来源：http://yk.nszjky.cn

Go:   func main()
来源：http://rs.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ma.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://tx.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://nz.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://uu.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://rt.shxzukj.cn

JS:   process.platform;  process.version
来源：http://dy.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://ko.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gb.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ss.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qc.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vc.shxzskj.cn

================================================================================
来源：http://zw.chemitech.net.cn

N. 数据结构与算法
来源：http://gf.nszjky.cn

================================================================================
来源：http://kf.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://vv.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bp.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vb.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gl.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wq.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://nf.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ej.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xh.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ob.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://al.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://os.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gj.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wq.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://az.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://mm.hahajie.cn

Ruby: arr.sort
来源：http://lh.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://li.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://sa.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iv.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://fn.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://se.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bh.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://si.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xo.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wb.yuexingan06.cn

[N04] 斐波那契数列
来源：http://xd.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yv.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pt.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ls.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kq.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://si.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lf.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gr.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jd.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ai.9csxet.cn

Py:   math.gcd(a, b)
来源：http://de.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lv.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yx.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qk.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bt.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hm.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://fv.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tx.lnxyls.cn

[N06] 判断回文字符串
来源：http://ad.szxytkj.cn

Py:   s == s[::-1]
来源：http://lf.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://it.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://kf.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://yg.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cz.colortex.cn

Go:   // 双指针从两端比较
来源：http://gg.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://sw.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pj.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://cn.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bu.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tn.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kr.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://bh.9csxet.cn

Java: // 手写 HashMap
来源：http://bf.newstarts.cn

Go:   // 手写 map[int]int
来源：http://xx.hahajie.cn

Ruby: // 手写 Hash
来源：http://ql.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uu.shxzskj.cn

[N08] 生成全排列
来源：http://ku.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://kc.nicolike.cn

PHP:  // 手写递归交换
来源：http://nq.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://gs.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://hv.haigaiapp.cn

Java: // 手写回溯递归
来源：http://zy.hahajie.cn

Go:   // 手写回溯递归
来源：http://bm.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ci.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://el.yuntaijiaju.cn

[N09] 栈与队列
来源：http://bf.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wv.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gi.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ds.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nh.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ic.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rv.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iw.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ya.nszjky.cn

[N10] 链表节点定义
来源：http://xd.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eq.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iv.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ax.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rk.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://dq.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nt.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bv.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://im.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://li.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wz.huixiangedu.cn


<!-- 参考信息 -->