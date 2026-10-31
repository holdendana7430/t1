代发 wailian999

TS:   JSON.parse(s)
来源：http://wv.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zi.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://qe.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://pa.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gm.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://rg.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yr.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ex.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ef.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ao.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ko.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ka.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ur.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://on.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://nf.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bu.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ec.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zl.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ky.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sz.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vw.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ip.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fy.hnjuh.cn

[K05] 深拷贝对象
来源：http://cd.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://vx.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://ir.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://jh.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://ed.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yu.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yd.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qv.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lt.colortex.cn

[K06] 解析 URL 查询串
来源：http://lc.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ew.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://id.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vk.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vg.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wq.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fh.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wv.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nz.szxytkj.cn

[K07] 进制转换
来源：http://rh.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xi.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vm.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nw.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://px.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zi.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bo.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nq.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ob.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://yu.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://na.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mi.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://yg.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://uw.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mu.shxzukj.cn

Go:   encoding/gob
来源：http://jm.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://jl.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gb.huixiangedu.cn

================================================================================
来源：http://mf.chemitech.net.cn

L. 网络请求
来源：http://mk.jctech888.com.cn

================================================================================
来源：http://vn.asd995.cn

[L01] 发送 GET 请求
来源：http://gf.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uo.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vc.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ls.szxytkj.cn

TS:   await fetch(url)
来源：http://nt.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lx.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://uy.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cb.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://op.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://yo.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kl.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tb.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vx.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zh.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jj.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ke.nszjky.cn

[L03] 设置自定义请求头
来源：http://an.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ha.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ej.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xa.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bp.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wo.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fv.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bj.newstarts.cn

[L04] 设置超时
来源：http://vg.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://te.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sx.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ze.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ud.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ci.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qd.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fc.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kt.9csxet.cn

[L05] 上传文件（multipart）
来源：http://kz.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zc.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bf.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fp.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rq.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://la.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wd.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nz.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://gz.muxihuayi.cn

Py:   resp.json()
来源：http://ht.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://qc.nicolike.cn

JS:   await resp.json()
来源：http://gz.yuntaijiaju.cn

TS:   await resp.json()
来源：http://lq.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ae.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iq.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://fx.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pl.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://hu.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://od.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qp.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://tl.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://uw.shxzukj.cn

Java: resp.statusCode()
来源：http://up.szsharing.cn

Go:   resp.StatusCode
来源：http://ud.shxzukj.cn

Ruby: resp.code.to_i
来源：http://la.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://iu.hahajie.cn

[L08] 并发请求多个地址
来源：http://sh.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xm.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ib.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xm.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ls.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ck.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yt.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ny.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iz.asd995.cn

================================================================================
来源：http://zi.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://di.9csxet.cn

================================================================================
来源：http://cr.hnjuh.cn

[M01] 读取命令行参数
来源：http://ng.nicolike.cn

Py:   sys.argv[1:]
来源：http://xe.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://lk.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://iy.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://jg.asd995.cn

Java: args 数组（main 方法参数）
来源：http://ls.nszjky.cn

Go:   os.Args[1:]
来源：http://ws.yuntaijiaju.cn

Ruby: ARGV
来源：http://xd.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://uh.colortex.cn

[M02] 读取环境变量
来源：http://ee.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://cb.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jr.wgjwhj.cn

JS:   process.env.HOME
来源：http://ux.huanxung.cn

TS:   process.env.HOME
来源：http://po.nszjky.cn

Java: System.getenv("HOME")
来源：http://db.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dm.nicolike.cn

Ruby: ENV["HOME"]
来源：http://nf.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://di.haigaiapp.cn

[M03] 执行外部命令
来源：http://cb.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ep.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ht.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wx.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ll.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wq.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ly.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zg.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://ln.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://sf.gzmigu.cn

Py:   os.getcwd()
来源：http://kw.bjjhwx.cn

PHP:  getcwd();
来源：http://nd.lnxyls.cn

JS:   process.cwd()
来源：http://zn.panjiajie.cn

TS:   process.cwd()
来源：http://dy.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://xh.jctech888.com.cn

Go:   os.Getwd()
来源：http://na.521024.cn

Ruby: Dir.pwd
来源：http://hh.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://en.hnjuh.cn

[M05] 设置退出码
来源：http://ru.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://qk.chemitech.net.cn

PHP:  exit(1);
来源：http://tf.panjiajie.cn

JS:   process.exit(1)
来源：http://xv.521024.cn

TS:   process.exit(1)
来源：http://og.yuntaijiaju.cn

Java: System.exit(1)
来源：http://ff.521024.cn

Go:   os.Exit(1)
来源：http://ma.colortex.cn

Ruby: exit 1
来源：http://tg.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://on.huanxung.cn

[M06] 向标准错误输出
来源：http://pq.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://qz.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jk.huixinmuqiang.cn

JS:   console.error("err")
来源：http://vy.szsharing.cn

TS:   console.error("err")
来源：http://hn.huanxung.cn

Java: System.err.println("err")
来源：http://sj.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ve.521024.cn

Ruby: warn "err"
来源：http://vs.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ps.hahajie.cn

[M07] 判断是否为主入口
来源：http://rt.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://kr.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xy.muxihuayi.cn

JS:   require.main === module
来源：http://gu.lnxyls.cn

TS:   require.main === module
来源：http://us.lnxyls.cn

Java: public static void main(String[] args)
来源：http://lt.nszjky.cn

Go:   func main()
来源：http://so.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ob.nszjky.cn

C#:   static void Main(string[] args)
来源：http://zt.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://yw.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://yx.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://an.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://se.nicolike.cn

TS:   process.platform;  process.version
来源：http://jr.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rr.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gh.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://we.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ce.521024.cn

================================================================================
来源：http://aj.jctech888.com.cn

N. 数据结构与算法
来源：http://hj.nicolike.cn

================================================================================
来源：http://pa.colortex.cn

[N01] 二分查找（有序数组）
来源：http://fg.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://or.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dp.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hr.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lk.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://af.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://iq.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wy.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ld.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gt.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ny.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xs.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cy.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://io.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://md.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://kk.huixiangedu.cn

Ruby: arr.sort
来源：http://gj.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ji.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://mc.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lj.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://qk.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://le.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mc.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lz.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://df.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kp.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qk.shtwfgs.cn

[N04] 斐波那契数列
来源：http://ph.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bt.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qg.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cb.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mf.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rq.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ty.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://za.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hv.shxzskj.cn

[N05] 最大公约数
来源：http://ml.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://lu.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mc.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wt.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fy.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fv.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kp.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://lz.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wv.9csxet.cn

[N06] 判断回文字符串
来源：http://mn.hnjuh.cn

Py:   s == s[::-1]
来源：http://pq.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://im.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://zb.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://hz.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ge.szsharing.cn

Go:   // 双指针从两端比较
来源：http://ei.521024.cn

Ruby: s == s.reverse
来源：http://yw.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ty.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://va.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gk.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pe.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ar.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://yw.nicolike.cn

Java: // 手写 HashMap
来源：http://dh.newstarts.cn

Go:   // 手写 map[int]int
来源：http://nm.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://qc.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cz.yuexingan06.cn

[N08] 生成全排列
来源：http://rz.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://go.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://mq.lnxyls.cn

JS:   // 手写回溯递归
来源：http://qu.lnxyls.cn

TS:   // 手写回溯递归
来源：http://ym.9csxet.cn

Java: // 手写回溯递归
来源：http://nl.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ou.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://hn.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://sk.szxytkj.cn

[N09] 栈与队列
来源：http://sg.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ek.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mf.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cu.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gy.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zb.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://er.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oq.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lb.nicolike.cn

[N10] 链表节点定义
来源：http://od.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cb.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ij.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pe.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oc.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ud.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://el.huanxung.cn


<!-- 参考信息 -->