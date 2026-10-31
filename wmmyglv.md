代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eu.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ag.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://we.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dl.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xd.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ri.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tn.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zq.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fp.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ub.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://vm.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ec.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://my.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ig.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://op.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wv.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sb.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ge.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://zl.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://rr.newstarts.cn

JS:   structuredClone(obj)
来源：http://kq.521024.cn

TS:   structuredClone(obj)
来源：http://po.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fv.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gu.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yj.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mh.asd995.cn

[K06] 解析 URL 查询串
来源：http://ys.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ub.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gu.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dp.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sw.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pc.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tj.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dn.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ri.nszjky.cn

[K07] 进制转换
来源：http://xu.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zx.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yb.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yy.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hr.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xx.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ce.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jg.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ua.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://vg.colortex.cn

Py:   pickle.dumps(obj)
来源：http://rn.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jb.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ta.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://fb.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bx.colortex.cn

Go:   encoding/gob
来源：http://vb.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://um.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://so.szxytkj.cn

================================================================================
来源：http://bc.yuexingan06.cn

L. 网络请求
来源：http://tg.haigaiapp.cn

================================================================================
来源：http://sn.panjiajie.cn

[L01] 发送 GET 请求
来源：http://sr.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lo.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ho.hahajie.cn

JS:   await fetch(url)
来源：http://yx.newstarts.cn

TS:   await fetch(url)
来源：http://sz.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lw.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://tn.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ed.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qz.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://rt.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://az.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jd.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lj.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://df.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://th.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ie.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ox.colortex.cn

[L03] 设置自定义请求头
来源：http://pe.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sz.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uz.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fb.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://km.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lp.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vu.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yh.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oz.9csxet.cn

[L04] 设置超时
来源：http://uv.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://tt.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ln.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zh.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bz.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pl.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yc.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yd.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tz.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://qh.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qk.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hn.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yl.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kl.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rs.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zk.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qm.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kw.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://wn.jianghongdianzi.cn

Py:   resp.json()
来源：http://fz.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://gh.shxzukj.cn

JS:   await resp.json()
来源：http://kf.panjiajie.cn

TS:   await resp.json()
来源：http://zz.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yt.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kz.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://xu.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eb.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://iw.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gk.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xc.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ce.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://al.yuexingan06.cn

Java: resp.statusCode()
来源：http://on.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://fp.hnjuh.cn

Ruby: resp.code.to_i
来源：http://vg.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://wa.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://fq.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fc.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://vy.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lo.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mp.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://il.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nt.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xm.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://ym.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://si.521024.cn

================================================================================
来源：http://sj.nszjky.cn

[M01] 读取命令行参数
来源：http://zs.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://rk.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://qt.szsharing.cn

JS:   process.argv.slice(2)
来源：http://ox.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://ba.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://qk.521024.cn

Go:   os.Args[1:]
来源：http://rg.szxytkj.cn

Ruby: ARGV
来源：http://tv.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://au.nszjky.cn

[M02] 读取环境变量
来源：http://dh.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://zt.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bd.gzmigu.cn

JS:   process.env.HOME
来源：http://ol.huanxung.cn

TS:   process.env.HOME
来源：http://sn.hahajie.cn

Java: System.getenv("HOME")
来源：http://ey.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pc.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ux.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://if.521024.cn

[M03] 执行外部命令
来源：http://nh.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pd.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uk.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jh.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vc.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://da.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pj.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://or.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://ks.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://qx.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://mj.bjjhwx.cn

PHP:  getcwd();
来源：http://de.bookmarksfly.cn

JS:   process.cwd()
来源：http://tc.huanxung.cn

TS:   process.cwd()
来源：http://hb.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://xi.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://mu.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://ts.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yx.lnxyls.cn

[M05] 设置退出码
来源：http://jb.shtwfgs.cn

Py:   sys.exit(1)
来源：http://tw.szsharing.cn

PHP:  exit(1);
来源：http://mw.hnjuh.cn

JS:   process.exit(1)
来源：http://pu.yuexingan06.cn

TS:   process.exit(1)
来源：http://rd.hnjuh.cn

Java: System.exit(1)
来源：http://xu.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://hs.lnxyls.cn

Ruby: exit 1
来源：http://oc.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zn.lnxyls.cn

[M06] 向标准错误输出
来源：http://oa.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://fq.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ta.asd995.cn

JS:   console.error("err")
来源：http://qo.yuntaijiaju.cn

TS:   console.error("err")
来源：http://rt.chemitech.net.cn

Java: System.err.println("err")
来源：http://tf.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://le.bookmarksfly.cn

Ruby: warn "err"
来源：http://ro.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://fr.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://jn.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ao.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ml.shxzskj.cn

JS:   require.main === module
来源：http://yt.gzmigu.cn

TS:   require.main === module
来源：http://sy.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ib.szxytkj.cn

Go:   func main()
来源：http://hw.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cb.nszjky.cn

C#:   static void Main(string[] args)
来源：http://so.asd995.cn

[M08] 获取系统与运行时信息
来源：http://ej.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://pv.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://gv.szxytkj.cn

JS:   process.platform;  process.version
来源：http://gy.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://lb.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oy.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bw.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jv.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xt.asd995.cn

================================================================================
来源：http://sd.hnjuh.cn

N. 数据结构与算法
来源：http://bs.gzmigu.cn

================================================================================
来源：http://tf.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://gv.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fm.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ls.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ts.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bc.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ae.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cy.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bc.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://cf.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://xl.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://si.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mc.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ym.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ts.asd995.cn

Go:   slices.Sort(arr)
来源：http://fc.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ti.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qu.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://kk.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sv.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://fl.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xl.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jn.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nt.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kj.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://id.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://md.nicolike.cn

[N04] 斐波那契数列
来源：http://fu.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rb.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jz.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pd.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ud.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ph.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rc.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dm.muxihuayi.cn

[N05] 最大公约数
来源：http://vz.huanxung.cn

Py:   math.gcd(a, b)
来源：http://dd.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sp.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vv.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hm.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ch.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://uf.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://we.colortex.cn

[N06] 判断回文字符串
来源：http://ij.haigaiapp.cn

Py:   s == s[::-1]
来源：http://xp.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://cr.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://iw.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ef.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zy.nicolike.cn

Go:   // 双指针从两端比较
来源：http://gz.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://pt.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cn.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://fh.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://as.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ta.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zy.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://dn.asd995.cn

Java: // 手写 HashMap
来源：http://rh.nicolike.cn

Go:   // 手写 map[int]int
来源：http://yz.shxzskj.cn

Ruby: // 手写 Hash
来源：http://yh.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fl.hahajie.cn

[N08] 生成全排列
来源：http://fc.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://xb.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://wr.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://df.hnjuh.cn

TS:   // 手写回溯递归
来源：http://tz.chemitech.net.cn

Java: // 手写回溯递归
来源：http://lj.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ve.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://oa.hnjuh.cn

C#:   // 手写回溯递归
来源：http://eb.muxihuayi.cn

[N09] 栈与队列
来源：http://px.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zu.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dl.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ek.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://no.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bp.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jr.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://an.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hh.newstarts.cn

[N10] 链表节点定义
来源：http://iu.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jf.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yb.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tv.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ru.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://rq.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hr.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xc.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lk.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://mp.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tc.panjiajie.cn


<!-- 参考信息 -->