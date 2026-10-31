代发 wailian999

TS:   JSON.parse(s)
来源：http://qu.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ay.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://nh.9csxet.cn

Ruby: JSON.parse(s)
来源：http://iq.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ue.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://gr.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ag.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xn.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qk.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ap.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hd.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ho.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yp.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ef.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://vy.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jk.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jx.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://po.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ub.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yc.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ro.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pq.gzmigu.cn

[K05] 深拷贝对象
来源：http://bg.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://jr.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://mm.hahajie.cn

JS:   structuredClone(obj)
来源：http://wb.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://bt.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://it.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ly.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://np.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://le.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://ia.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sr.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ls.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xu.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qj.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sq.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fz.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nx.szsharing.cn

[K07] 进制转换
来源：http://la.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nn.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hm.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kx.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pm.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eb.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nv.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://le.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jn.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://uo.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://me.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wz.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://uu.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://lp.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yk.newstarts.cn

Go:   encoding/gob
来源：http://js.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://va.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lq.bookmarksfly.cn

================================================================================
来源：http://qq.yuexingan06.cn

L. 网络请求
来源：http://bw.haigaiapp.cn

================================================================================
来源：http://pl.shxzukj.cn

[L01] 发送 GET 请求
来源：http://fn.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fw.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dk.bjjhwx.cn

JS:   await fetch(url)
来源：http://yd.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://ee.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tg.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://as.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://du.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nf.shxzskj.cn

[L02] 发送 POST JSON
来源：http://fx.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vn.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mf.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hd.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gs.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://op.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zs.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zc.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ds.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://gg.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ml.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fc.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fb.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://px.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xi.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tr.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ff.bookmarksfly.cn

[L04] 设置超时
来源：http://sl.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://fr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zr.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://up.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pk.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ik.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aw.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ye.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gu.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://dx.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uk.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ow.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ra.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://in.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dv.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bh.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pg.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://qm.yuexingan06.cn

Py:   resp.json()
来源：http://ul.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://wj.hnjuh.cn

JS:   await resp.json()
来源：http://xb.lnxyls.cn

TS:   await resp.json()
来源：http://wv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ce.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ke.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://ts.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dx.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://lb.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kd.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rc.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://go.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ab.bookmarksfly.cn

Java: resp.statusCode()
来源：http://qp.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://if.nszjky.cn

Ruby: resp.code.to_i
来源：http://gi.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://iu.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://ou.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pi.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://cp.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dy.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://au.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gr.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gq.szxytkj.cn

================================================================================
来源：http://ye.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://or.yuexingan06.cn

================================================================================
来源：http://nf.lnxyls.cn

[M01] 读取命令行参数
来源：http://zt.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://mf.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://lj.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ki.521024.cn

TS:   process.argv.slice(2)
来源：http://ge.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://ko.lnxyls.cn

Go:   os.Args[1:]
来源：http://js.muxihuayi.cn

Ruby: ARGV
来源：http://rj.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://cu.huixiangedu.cn

[M02] 读取环境变量
来源：http://hz.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://lq.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mg.shxzukj.cn

JS:   process.env.HOME
来源：http://qm.shxzukj.cn

TS:   process.env.HOME
来源：http://og.szsharing.cn

Java: System.getenv("HOME")
来源：http://vd.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tn.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://hv.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ce.newstarts.cn

[M03] 执行外部命令
来源：http://lw.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fq.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://an.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ps.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yt.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wi.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://af.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zw.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://pz.hnjuh.cn

[M04] 获取当前工作目录
来源：http://gz.szxytkj.cn

Py:   os.getcwd()
来源：http://qq.huixinmuqiang.cn

PHP:  getcwd();
来源：http://qu.hnjuh.cn

JS:   process.cwd()
来源：http://hy.lnxyls.cn

TS:   process.cwd()
来源：http://ne.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://ur.chemitech.net.cn

Go:   os.Getwd()
来源：http://pl.wgjwhj.cn

Ruby: Dir.pwd
来源：http://rn.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ye.newstarts.cn

[M05] 设置退出码
来源：http://za.wgjwhj.cn

Py:   sys.exit(1)
来源：http://za.panjiajie.cn

PHP:  exit(1);
来源：http://ux.bookmarksfly.cn

JS:   process.exit(1)
来源：http://mf.nszjky.cn

TS:   process.exit(1)
来源：http://bo.yuexingan06.cn

Java: System.exit(1)
来源：http://mf.newstarts.cn

Go:   os.Exit(1)
来源：http://fy.jianghongdianzi.cn

Ruby: exit 1
来源：http://jm.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gf.gzmigu.cn

[M06] 向标准错误输出
来源：http://fh.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://qx.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ib.shtwfgs.cn

JS:   console.error("err")
来源：http://pd.yuexingan06.cn

TS:   console.error("err")
来源：http://po.szxytkj.cn

Java: System.err.println("err")
来源：http://gj.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yc.huixiangedu.cn

Ruby: warn "err"
来源：http://nk.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://te.newstarts.cn

[M07] 判断是否为主入口
来源：http://lh.asd995.cn

Py:   if __name__ == "__main__":
来源：http://cj.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pz.nszjky.cn

JS:   require.main === module
来源：http://ls.panjiajie.cn

TS:   require.main === module
来源：http://lp.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ga.huixiangedu.cn

Go:   func main()
来源：http://vh.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ej.colortex.cn

C#:   static void Main(string[] args)
来源：http://wc.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ss.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://jg.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://ea.asd995.cn

JS:   process.platform;  process.version
来源：http://rm.szxytkj.cn

TS:   process.platform;  process.version
来源：http://dt.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ga.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nf.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fd.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vl.asd995.cn

================================================================================
来源：http://zr.asd995.cn

N. 数据结构与算法
来源：http://rz.shxzukj.cn

================================================================================
来源：http://xn.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://gi.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rj.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fs.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ov.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yu.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ji.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://xb.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://up.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gm.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://qb.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://mp.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hh.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nj.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://im.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zq.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://on.lnxyls.cn

Ruby: arr.sort
来源：http://da.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mh.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://ls.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sw.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://ni.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uf.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ks.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oe.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zv.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ox.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dp.hnjuh.cn

[N04] 斐波那契数列
来源：http://gj.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ts.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qb.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ea.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hl.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cb.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nk.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sd.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jp.muxihuayi.cn

[N05] 最大公约数
来源：http://xl.szsharing.cn

Py:   math.gcd(a, b)
来源：http://uv.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://so.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bk.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xc.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zq.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pa.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://lt.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ve.shxzskj.cn

[N06] 判断回文字符串
来源：http://ag.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://la.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://rt.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://yd.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ht.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nu.szsharing.cn

Go:   // 双指针从两端比较
来源：http://hy.nicolike.cn

Ruby: s == s.reverse
来源：http://ix.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://la.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://hf.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nw.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ki.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hc.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://ob.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ri.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ee.asd995.cn

Ruby: // 手写 Hash
来源：http://jv.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pl.jctech888.com.cn

[N08] 生成全排列
来源：http://rk.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://ze.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://wd.hahajie.cn

JS:   // 手写回溯递归
来源：http://xc.huanxung.cn

TS:   // 手写回溯递归
来源：http://io.szxytkj.cn

Java: // 手写回溯递归
来源：http://lw.hnjuh.cn

Go:   // 手写回溯递归
来源：http://np.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://oi.szsharing.cn

C#:   // 手写回溯递归
来源：http://gl.muxihuayi.cn

[N09] 栈与队列
来源：http://ba.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zp.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fh.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tm.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hy.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yi.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ry.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qd.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ut.lnxyls.cn

[N10] 链表节点定义
来源：http://qr.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ci.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pu.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oc.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kd.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://kq.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vl.jianghongdianzi.cn


<!-- 参考信息 -->