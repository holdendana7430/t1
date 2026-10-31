代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ra.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://ph.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ei.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ax.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cj.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qg.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ad.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ir.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://by.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wd.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://gy.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://id.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sr.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://he.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uz.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sh.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cc.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jp.hnjuh.cn

[K05] 深拷贝对象
来源：http://uf.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://gm.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://di.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://vn.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ok.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sp.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xa.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oy.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hb.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://no.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rj.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zq.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ez.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lk.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lj.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pm.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yy.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tv.szxytkj.cn

[K07] 进制转换
来源：http://qd.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uj.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ii.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oz.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zh.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zo.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pq.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ds.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ck.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://gd.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ht.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://si.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gk.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://gg.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jj.yuntaijiaju.cn

Go:   encoding/gob
来源：http://oe.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://yy.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://km.szxytkj.cn

================================================================================
来源：http://vx.jctech888.com.cn

L. 网络请求
来源：http://ti.yuexingan06.cn

================================================================================
来源：http://xw.szsharing.cn

[L01] 发送 GET 请求
来源：http://pb.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pk.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://af.hnjuh.cn

JS:   await fetch(url)
来源：http://kn.szxytkj.cn

TS:   await fetch(url)
来源：http://mw.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uk.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://lo.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jq.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ik.hahajie.cn

[L02] 发送 POST JSON
来源：http://gf.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lp.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aw.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ii.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zu.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://av.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tc.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ut.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xx.newstarts.cn

[L03] 设置自定义请求头
来源：http://vz.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ms.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sz.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gm.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tu.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xy.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dl.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hw.newstarts.cn

[L04] 设置超时
来源：http://af.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://sx.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bw.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qf.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xf.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pg.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qe.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xm.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://no.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yc.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oj.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://em.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ed.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ku.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oh.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qm.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ip.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://qp.szsharing.cn

Py:   resp.json()
来源：http://ot.9csxet.cn

PHP:  json_decode($body, true);
来源：http://cl.9csxet.cn

JS:   await resp.json()
来源：http://mz.jianghongdianzi.cn

TS:   await resp.json()
来源：http://qa.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gy.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nd.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://wi.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ri.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://cp.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qz.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://if.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://my.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://mu.huanxung.cn

Java: resp.statusCode()
来源：http://wl.newstarts.cn

Go:   resp.StatusCode
来源：http://lg.shxzskj.cn

Ruby: resp.code.to_i
来源：http://zi.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://en.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://uy.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://co.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://xy.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dz.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://al.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uv.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hs.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pa.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wc.huixinmuqiang.cn

================================================================================
来源：http://xz.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://is.colortex.cn

================================================================================
来源：http://rj.huanxung.cn

[M01] 读取命令行参数
来源：http://aa.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ra.nicolike.cn

PHP:  $argv;  $argc;
来源：http://wk.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://bu.9csxet.cn

TS:   process.argv.slice(2)
来源：http://kc.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://lh.shtwfgs.cn

Go:   os.Args[1:]
来源：http://qq.szxytkj.cn

Ruby: ARGV
来源：http://ur.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://it.szsharing.cn

[M02] 读取环境变量
来源：http://xg.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ic.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ue.colortex.cn

JS:   process.env.HOME
来源：http://ps.wgjwhj.cn

TS:   process.env.HOME
来源：http://is.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://td.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://im.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://ci.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://us.shtwfgs.cn

[M03] 执行外部命令
来源：http://xz.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sv.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gh.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vs.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oq.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ja.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yc.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tf.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://gr.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ln.bjjhwx.cn

Py:   os.getcwd()
来源：http://ao.nszjky.cn

PHP:  getcwd();
来源：http://eq.haigaiapp.cn

JS:   process.cwd()
来源：http://fx.bjjhwx.cn

TS:   process.cwd()
来源：http://hq.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://gs.lnxyls.cn

Go:   os.Getwd()
来源：http://be.muxihuayi.cn

Ruby: Dir.pwd
来源：http://yl.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hk.jianghongdianzi.cn

[M05] 设置退出码
来源：http://uy.szsharing.cn

Py:   sys.exit(1)
来源：http://lt.9csxet.cn

PHP:  exit(1);
来源：http://uc.huanxung.cn

JS:   process.exit(1)
来源：http://lh.shtwfgs.cn

TS:   process.exit(1)
来源：http://fs.9csxet.cn

Java: System.exit(1)
来源：http://dj.shxzskj.cn

Go:   os.Exit(1)
来源：http://zg.jianghongdianzi.cn

Ruby: exit 1
来源：http://iu.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://km.chemitech.net.cn

[M06] 向标准错误输出
来源：http://hl.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://xc.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rk.huanxung.cn

JS:   console.error("err")
来源：http://se.bookmarksfly.cn

TS:   console.error("err")
来源：http://ug.huanxung.cn

Java: System.err.println("err")
来源：http://wa.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qo.haigaiapp.cn

Ruby: warn "err"
来源：http://gk.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://wt.nszjky.cn

[M07] 判断是否为主入口
来源：http://va.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://cv.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kh.521024.cn

JS:   require.main === module
来源：http://ys.muxihuayi.cn

TS:   require.main === module
来源：http://iq.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://hn.jctech888.com.cn

Go:   func main()
来源：http://tt.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hc.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://az.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://yw.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ej.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://uq.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://ap.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://pk.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pk.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://is.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tl.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zx.bookmarksfly.cn

================================================================================
来源：http://oq.shxzskj.cn

N. 数据结构与算法
来源：http://pa.hahajie.cn

================================================================================
来源：http://jy.asd995.cn

[N01] 二分查找（有序数组）
来源：http://zo.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uq.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bm.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pf.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ar.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wa.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://if.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ps.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vz.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ik.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://so.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lc.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oa.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wp.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ua.yuntaijiaju.cn

Ruby: arr.sort
来源：http://cm.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://an.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://pq.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://so.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://oc.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qk.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rk.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xt.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qu.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wv.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dr.szsharing.cn

[N04] 斐波那契数列
来源：http://ie.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ux.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rp.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ov.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bn.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pu.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ny.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vn.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://js.colortex.cn

[N05] 最大公约数
来源：http://ot.newstarts.cn

Py:   math.gcd(a, b)
来源：http://uy.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cx.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://du.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pz.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fm.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ex.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://gb.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pa.hnjuh.cn

[N06] 判断回文字符串
来源：http://wx.huixiangedu.cn

Py:   s == s[::-1]
来源：http://zi.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://lv.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://fc.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://wq.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xa.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://qj.haigaiapp.cn

Ruby: s == s.reverse
来源：http://nb.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zt.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://gv.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gp.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fb.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mk.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://ew.shtwfgs.cn

Java: // 手写 HashMap
来源：http://zs.hahajie.cn

Go:   // 手写 map[int]int
来源：http://ov.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://gz.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bi.shxzskj.cn

[N08] 生成全排列
来源：http://nc.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ph.nszjky.cn

PHP:  // 手写递归交换
来源：http://rx.shxzskj.cn

JS:   // 手写回溯递归
来源：http://mi.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ze.gzmigu.cn

Java: // 手写回溯递归
来源：http://qq.szsharing.cn

Go:   // 手写回溯递归
来源：http://ae.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://la.hahajie.cn

C#:   // 手写回溯递归
来源：http://lt.muxihuayi.cn

[N09] 栈与队列
来源：http://ss.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ke.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ez.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://be.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ei.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://id.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cq.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bg.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hw.yuexingan06.cn

[N10] 链表节点定义
来源：http://eh.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xn.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fh.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aw.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://he.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://sn.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://le.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ur.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wm.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ss.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ln.jctech888.com.cn


<!-- 参考信息 -->