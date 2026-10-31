代发 wailian999

TS:   JSON.parse(s)
来源：http://yk.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nd.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://tu.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://ij.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wc.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://cl.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uc.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pf.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ja.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pv.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kn.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wd.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kj.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wk.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ep.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ns.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ir.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qw.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qb.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yp.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jw.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ln.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tw.lnxyls.cn

[K05] 深拷贝对象
来源：http://rr.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://na.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://pa.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://rk.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://wl.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nk.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ho.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fh.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lf.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://sw.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://md.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cj.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vd.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ac.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fm.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xd.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qr.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sm.asd995.cn

[K07] 进制转换
来源：http://ll.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qf.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ot.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ns.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gy.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bv.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mp.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://af.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ci.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ig.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://vg.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nb.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://dd.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://eb.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nh.chemitech.net.cn

Go:   encoding/gob
来源：http://fk.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://wx.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uk.nicolike.cn

================================================================================
来源：http://ct.yuexingan06.cn

L. 网络请求
来源：http://kj.shxzskj.cn

================================================================================
来源：http://xx.gzmigu.cn

[L01] 发送 GET 请求
来源：http://ym.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vv.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dm.521024.cn

JS:   await fetch(url)
来源：http://vi.haigaiapp.cn

TS:   await fetch(url)
来源：http://aw.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://br.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://nm.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ly.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://td.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://va.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://av.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pv.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vc.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ju.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nm.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uw.huanxung.cn

[L03] 设置自定义请求头
来源：http://dj.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://se.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://et.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ud.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bw.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hy.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ih.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xa.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qr.9csxet.cn

[L04] 设置超时
来源：http://tn.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://gb.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cu.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oh.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rb.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ub.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zc.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nr.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://im.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ls.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://by.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dq.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mn.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jc.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ps.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nq.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ne.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://tj.wgjwhj.cn

Py:   resp.json()
来源：http://bw.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://vm.shtwfgs.cn

JS:   await resp.json()
来源：http://hi.jianghongdianzi.cn

TS:   await resp.json()
来源：http://cd.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hg.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://on.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ls.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hr.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://mk.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jc.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ru.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://el.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://hu.shtwfgs.cn

Java: resp.statusCode()
来源：http://fz.colortex.cn

Go:   resp.StatusCode
来源：http://nn.shxzukj.cn

Ruby: resp.code.to_i
来源：http://rl.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://sl.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://kw.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fu.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://yu.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vg.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://em.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ws.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vy.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ay.lnxyls.cn

================================================================================
来源：http://vr.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ou.panjiajie.cn

================================================================================
来源：http://rw.shxzskj.cn

[M01] 读取命令行参数
来源：http://zz.hnjuh.cn

Py:   sys.argv[1:]
来源：http://xh.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://dm.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://zy.newstarts.cn

TS:   process.argv.slice(2)
来源：http://qt.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://kd.wgjwhj.cn

Go:   os.Args[1:]
来源：http://od.huixinmuqiang.cn

Ruby: ARGV
来源：http://qv.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://rf.szsharing.cn

[M02] 读取环境变量
来源：http://ht.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://wp.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://te.9csxet.cn

JS:   process.env.HOME
来源：http://gw.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://gu.szxytkj.cn

Java: System.getenv("HOME")
来源：http://ij.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hg.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://jp.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jx.szsharing.cn

[M03] 执行外部命令
来源：http://gi.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xx.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yb.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nb.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://le.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pw.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jj.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://vt.nszjky.cn

[M04] 获取当前工作目录
来源：http://ap.szxytkj.cn

Py:   os.getcwd()
来源：http://db.shxzskj.cn

PHP:  getcwd();
来源：http://ae.shtwfgs.cn

JS:   process.cwd()
来源：http://sd.bookmarksfly.cn

TS:   process.cwd()
来源：http://uy.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://wv.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://wd.huixiangedu.cn

Ruby: Dir.pwd
来源：http://ew.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ez.newstarts.cn

[M05] 设置退出码
来源：http://au.newstarts.cn

Py:   sys.exit(1)
来源：http://hz.wgjwhj.cn

PHP:  exit(1);
来源：http://vv.huanxung.cn

JS:   process.exit(1)
来源：http://jm.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://yy.yuntaijiaju.cn

Java: System.exit(1)
来源：http://mq.chemitech.net.cn

Go:   os.Exit(1)
来源：http://si.muxihuayi.cn

Ruby: exit 1
来源：http://qt.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bl.yuexingan06.cn

[M06] 向标准错误输出
来源：http://jz.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://nt.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://do.bjjhwx.cn

JS:   console.error("err")
来源：http://pk.colortex.cn

TS:   console.error("err")
来源：http://wu.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://yo.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://id.shtwfgs.cn

Ruby: warn "err"
来源：http://pc.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://df.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://ef.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ex.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://go.chemitech.net.cn

JS:   require.main === module
来源：http://sw.shxzskj.cn

TS:   require.main === module
来源：http://io.hnjuh.cn

Java: public static void main(String[] args)
来源：http://os.huixinmuqiang.cn

Go:   func main()
来源：http://pr.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gp.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://yb.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://lp.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://jt.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://pc.panjiajie.cn

JS:   process.platform;  process.version
来源：http://jc.szsharing.cn

TS:   process.platform;  process.version
来源：http://rx.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lr.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ol.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yu.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vu.asd995.cn

================================================================================
来源：http://hw.shxzukj.cn

N. 数据结构与算法
来源：http://nw.panjiajie.cn

================================================================================
来源：http://gt.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://hr.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wl.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yc.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rd.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tt.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bf.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://ke.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ed.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gq.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://qe.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ae.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qe.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bq.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cu.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bc.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://sb.asd995.cn

Ruby: arr.sort
来源：http://bv.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ju.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://jv.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sy.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://op.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cq.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xu.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nt.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ye.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ae.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wd.jctech888.com.cn

[N04] 斐波那契数列
来源：http://bh.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ps.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zd.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://we.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yz.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://az.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sl.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ap.wgjwhj.cn

[N05] 最大公约数
来源：http://gb.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ej.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dz.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yx.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vx.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cy.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://em.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://bb.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://za.yuexingan06.cn

[N06] 判断回文字符串
来源：http://if.gzmigu.cn

Py:   s == s[::-1]
来源：http://sw.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://nf.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://wz.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://mr.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fy.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://js.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://no.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yf.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://dr.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tx.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rq.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ih.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://uu.lnxyls.cn

Java: // 手写 HashMap
来源：http://kj.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ni.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://fy.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://he.colortex.cn

[N08] 生成全排列
来源：http://eg.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://bf.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://eg.colortex.cn

JS:   // 手写回溯递归
来源：http://rz.nszjky.cn

TS:   // 手写回溯递归
来源：http://xu.shxzskj.cn

Java: // 手写回溯递归
来源：http://lz.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://po.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://qy.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://ps.521024.cn

[N09] 栈与队列
来源：http://bv.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vr.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cc.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xo.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://in.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://em.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yr.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ot.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yn.9csxet.cn

[N10] 链表节点定义
来源：http://mw.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mo.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ao.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mo.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ah.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://xo.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://by.shxzskj.cn


<!-- 参考信息 -->