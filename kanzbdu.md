代发 wailian999

TS:   JSON.parse(s)
来源：http://kz.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wf.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://vx.huanxung.cn

Ruby: JSON.parse(s)
来源：http://xi.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sx.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://sq.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gz.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ok.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lc.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ww.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ra.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sh.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oo.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tf.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://hr.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qs.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bk.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sn.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xc.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dx.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://um.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mc.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fm.newstarts.cn

[K05] 深拷贝对象
来源：http://uo.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://df.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://wi.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://zx.szxytkj.cn

TS:   structuredClone(obj)
来源：http://qr.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ml.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xe.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fy.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vc.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://hw.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ow.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zg.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://os.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lq.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gy.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fw.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xy.szsharing.cn

[K07] 进制转换
来源：http://ud.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gq.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://en.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zm.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ml.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kp.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ly.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yi.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iw.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ny.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://xq.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ta.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://qo.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ji.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://el.muxihuayi.cn

Go:   encoding/gob
来源：http://qd.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://aa.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qj.asd995.cn

================================================================================
来源：http://au.szxytkj.cn

L. 网络请求
来源：http://ak.huanxung.cn

================================================================================
来源：http://dd.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://as.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nl.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uz.newstarts.cn

JS:   await fetch(url)
来源：http://va.gzmigu.cn

TS:   await fetch(url)
来源：http://td.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aj.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://lx.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hk.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nr.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://ty.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iz.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zy.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hk.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pv.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rd.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yz.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yc.panjiajie.cn

[L03] 设置自定义请求头
来源：http://lh.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://to.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pw.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://as.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gj.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ws.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vf.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://on.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wj.jctech888.com.cn

[L04] 设置超时
来源：http://ro.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://lv.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nd.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uj.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ly.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ps.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kx.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yf.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hu.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://qj.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://op.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tu.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://im.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wu.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lu.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lw.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yd.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zf.huanxung.cn

[L06] 解析响应为 JSON
来源：http://jn.nszjky.cn

Py:   resp.json()
来源：http://pv.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://ce.yuexingan06.cn

JS:   await resp.json()
来源：http://lh.panjiajie.cn

TS:   await resp.json()
来源：http://nd.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rl.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hl.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://zd.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mn.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://fp.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://au.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ft.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ls.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://bx.nszjky.cn

Java: resp.statusCode()
来源：http://vz.asd995.cn

Go:   resp.StatusCode
来源：http://ys.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://fd.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://mq.shxzukj.cn

[L08] 并发请求多个地址
来源：http://tf.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://da.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://bn.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ah.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xm.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zf.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zn.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xa.9csxet.cn

================================================================================
来源：http://vu.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://jb.colortex.cn

================================================================================
来源：http://qv.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://jf.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://xb.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://lu.nszjky.cn

JS:   process.argv.slice(2)
来源：http://lh.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://mj.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://nn.newstarts.cn

Go:   os.Args[1:]
来源：http://jz.bookmarksfly.cn

Ruby: ARGV
来源：http://ig.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://wh.521024.cn

[M02] 读取环境变量
来源：http://cf.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://xl.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yq.szxytkj.cn

JS:   process.env.HOME
来源：http://pg.jctech888.com.cn

TS:   process.env.HOME
来源：http://tx.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://jx.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gy.newstarts.cn

Ruby: ENV["HOME"]
来源：http://wx.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ho.gzmigu.cn

[M03] 执行外部命令
来源：http://gc.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://my.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rj.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lh.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dk.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ij.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fb.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rj.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://cz.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://pc.yuexingan06.cn

Py:   os.getcwd()
来源：http://yx.nszjky.cn

PHP:  getcwd();
来源：http://ps.szxytkj.cn

JS:   process.cwd()
来源：http://cc.yuexingan06.cn

TS:   process.cwd()
来源：http://zt.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://xo.huixiangedu.cn

Go:   os.Getwd()
来源：http://nc.jctech888.com.cn

Ruby: Dir.pwd
来源：http://st.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sc.9csxet.cn

[M05] 设置退出码
来源：http://fo.hahajie.cn

Py:   sys.exit(1)
来源：http://cd.asd995.cn

PHP:  exit(1);
来源：http://kq.chemitech.net.cn

JS:   process.exit(1)
来源：http://ad.asd995.cn

TS:   process.exit(1)
来源：http://ri.colortex.cn

Java: System.exit(1)
来源：http://sl.jctech888.com.cn

Go:   os.Exit(1)
来源：http://zz.huixiangedu.cn

Ruby: exit 1
来源：http://pr.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wp.huanxung.cn

[M06] 向标准错误输出
来源：http://ya.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://nu.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://km.colortex.cn

JS:   console.error("err")
来源：http://zz.jctech888.com.cn

TS:   console.error("err")
来源：http://hw.hnjuh.cn

Java: System.err.println("err")
来源：http://vp.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://on.bookmarksfly.cn

Ruby: warn "err"
来源：http://ue.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ep.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://gr.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://cq.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ji.huixiangedu.cn

JS:   require.main === module
来源：http://kl.bookmarksfly.cn

TS:   require.main === module
来源：http://yg.szsharing.cn

Java: public static void main(String[] args)
来源：http://dh.nszjky.cn

Go:   func main()
来源：http://dy.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rt.asd995.cn

C#:   static void Main(string[] args)
来源：http://ta.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://hk.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://je.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://et.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://iu.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://lx.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zu.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ze.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://er.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://at.szsharing.cn

================================================================================
来源：http://wu.yuntaijiaju.cn

N. 数据结构与算法
来源：http://cw.shxzskj.cn

================================================================================
来源：http://pk.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://ne.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qe.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pa.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nc.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qx.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gk.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://rd.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lj.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zv.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://av.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://hg.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eb.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ij.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ty.nicolike.cn

Go:   slices.Sort(arr)
来源：http://vw.muxihuayi.cn

Ruby: arr.sort
来源：http://oh.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ki.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://bk.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dy.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://zf.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jz.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tu.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gz.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ud.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mq.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gy.lnxyls.cn

[N04] 斐波那契数列
来源：http://oc.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://te.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bo.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ra.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qx.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dl.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oh.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rp.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ma.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://wx.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dz.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zk.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eq.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yj.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ki.521024.cn

Ruby: a.gcd(b)
来源：http://dh.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bu.hahajie.cn

[N06] 判断回文字符串
来源：http://ju.asd995.cn

Py:   s == s[::-1]
来源：http://cn.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://re.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://lb.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://wd.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yw.huanxung.cn

Go:   // 双指针从两端比较
来源：http://aq.521024.cn

Ruby: s == s.reverse
来源：http://yt.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oh.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://cp.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cp.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://un.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jf.521024.cn

TS:   // 手写 Map<string, number>
来源：http://fx.colortex.cn

Java: // 手写 HashMap
来源：http://oo.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ds.nszjky.cn

Ruby: // 手写 Hash
来源：http://sa.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vp.haigaiapp.cn

[N08] 生成全排列
来源：http://yd.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://kf.panjiajie.cn

PHP:  // 手写递归交换
来源：http://zu.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ms.hnjuh.cn

TS:   // 手写回溯递归
来源：http://lu.yuexingan06.cn

Java: // 手写回溯递归
来源：http://fe.521024.cn

Go:   // 手写回溯递归
来源：http://hq.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://gs.lnxyls.cn

C#:   // 手写回溯递归
来源：http://rd.szsharing.cn

[N09] 栈与队列
来源：http://fi.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tc.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ck.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wu.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zl.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ly.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://us.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sv.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yf.9csxet.cn

[N10] 链表节点定义
来源：http://pv.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://he.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qe.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fw.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dz.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://bv.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pe.9csxet.cn


<!-- 参考信息 -->