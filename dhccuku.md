代发 wailian999

TS:   JSON.parse(s)
来源：http://pb.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ku.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://sq.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ef.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zm.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://zx.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qb.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kt.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bd.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tp.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wo.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ew.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bq.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rc.colortex.cn

[K04] 读取 JSON 文件
来源：http://wb.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ad.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lb.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iu.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ta.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://se.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lt.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nu.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hd.haigaiapp.cn

[K05] 深拷贝对象
来源：http://qw.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://yy.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://lz.newstarts.cn

JS:   structuredClone(obj)
来源：http://jb.hnjuh.cn

TS:   structuredClone(obj)
来源：http://br.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://he.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jx.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ct.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qh.521024.cn

[K06] 解析 URL 查询串
来源：http://fh.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yl.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ch.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dv.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bh.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ym.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dr.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vs.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://en.chemitech.net.cn

[K07] 进制转换
来源：http://vx.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vk.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://km.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://la.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zs.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://co.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pw.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wc.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oy.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://lz.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://ld.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dd.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://eg.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ds.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fo.haigaiapp.cn

Go:   encoding/gob
来源：http://ih.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://sx.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uh.nszjky.cn

================================================================================
来源：http://ar.chemitech.net.cn

L. 网络请求
来源：http://mf.shxzskj.cn

================================================================================
来源：http://kk.shxzskj.cn

[L01] 发送 GET 请求
来源：http://fi.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rk.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fp.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://vq.lnxyls.cn

TS:   await fetch(url)
来源：http://hc.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qf.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://sv.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yn.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pl.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://fe.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fi.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://az.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qb.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rg.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hg.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zd.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mp.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pb.gzmigu.cn

[L03] 设置自定义请求头
来源：http://hs.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fq.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mo.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jp.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yy.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dd.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ws.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pw.jctech888.com.cn

[L04] 设置超时
来源：http://jt.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ad.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qa.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rz.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://px.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bp.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fb.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zv.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kn.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://dz.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bm.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://se.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://us.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://le.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dh.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://og.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xw.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gn.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://ml.shxzskj.cn

Py:   resp.json()
来源：http://aa.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://vd.bjjhwx.cn

JS:   await resp.json()
来源：http://yq.521024.cn

TS:   await resp.json()
来源：http://sv.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qc.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://si.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://qq.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ib.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://pl.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rn.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ks.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ep.asd995.cn

TS:   resp.ok;  resp.status
来源：http://vl.nszjky.cn

Java: resp.statusCode()
来源：http://jh.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://ro.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://pc.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://hp.nicolike.cn

[L08] 并发请求多个地址
来源：http://yr.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vp.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://gz.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mx.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://il.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yl.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rs.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ea.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dy.shtwfgs.cn

================================================================================
来源：http://zl.521024.cn

M. 命令行 / 进程 / 环境
来源：http://op.yuntaijiaju.cn

================================================================================
来源：http://ms.jctech888.com.cn

[M01] 读取命令行参数
来源：http://np.shxzskj.cn

Py:   sys.argv[1:]
来源：http://zp.hahajie.cn

PHP:  $argv;  $argc;
来源：http://gd.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://rv.colortex.cn

TS:   process.argv.slice(2)
来源：http://en.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://oc.nszjky.cn

Go:   os.Args[1:]
来源：http://hs.521024.cn

Ruby: ARGV
来源：http://tz.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://zl.9csxet.cn

[M02] 读取环境变量
来源：http://gf.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://wz.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ts.hnjuh.cn

JS:   process.env.HOME
来源：http://wi.newstarts.cn

TS:   process.env.HOME
来源：http://zf.szsharing.cn

Java: System.getenv("HOME")
来源：http://ya.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ic.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://fo.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://im.bjjhwx.cn

[M03] 执行外部命令
来源：http://gg.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eo.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vu.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yu.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kr.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rs.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pp.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lh.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://px.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://wo.bjjhwx.cn

Py:   os.getcwd()
来源：http://as.yuntaijiaju.cn

PHP:  getcwd();
来源：http://py.yuexingan06.cn

JS:   process.cwd()
来源：http://gh.chemitech.net.cn

TS:   process.cwd()
来源：http://ck.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ys.nszjky.cn

Go:   os.Getwd()
来源：http://bo.chemitech.net.cn

Ruby: Dir.pwd
来源：http://hw.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pq.yuexingan06.cn

[M05] 设置退出码
来源：http://tw.shxzukj.cn

Py:   sys.exit(1)
来源：http://aa.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ge.521024.cn

JS:   process.exit(1)
来源：http://zs.newstarts.cn

TS:   process.exit(1)
来源：http://fc.wgjwhj.cn

Java: System.exit(1)
来源：http://mg.szsharing.cn

Go:   os.Exit(1)
来源：http://sx.shxzskj.cn

Ruby: exit 1
来源：http://mg.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jk.szsharing.cn

[M06] 向标准错误输出
来源：http://gd.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://sz.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ii.haigaiapp.cn

JS:   console.error("err")
来源：http://un.9csxet.cn

TS:   console.error("err")
来源：http://bo.szxytkj.cn

Java: System.err.println("err")
来源：http://lz.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://so.huanxung.cn

Ruby: warn "err"
来源：http://nt.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://jj.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://hs.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://ru.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rt.nszjky.cn

JS:   require.main === module
来源：http://ox.lnxyls.cn

TS:   require.main === module
来源：http://tk.9csxet.cn

Java: public static void main(String[] args)
来源：http://fe.hnjuh.cn

Go:   func main()
来源：http://io.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mn.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://cq.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://ws.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://qc.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://sm.hnjuh.cn

JS:   process.platform;  process.version
来源：http://wc.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://su.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yf.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://my.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oo.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bf.nicolike.cn

================================================================================
来源：http://yx.yuexingan06.cn

N. 数据结构与算法
来源：http://oj.yuexingan06.cn

================================================================================
来源：http://km.521024.cn

[N01] 二分查找（有序数组）
来源：http://be.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fg.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iu.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uq.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rd.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ck.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://ym.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ob.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cs.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://yk.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://gz.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ud.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nz.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cf.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ba.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://rq.newstarts.cn

Ruby: arr.sort
来源：http://xy.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bd.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://wg.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://as.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://kj.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tl.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lp.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ev.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://su.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://al.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ui.newstarts.cn

[N04] 斐波那契数列
来源：http://gy.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cy.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qj.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ht.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ci.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xy.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gw.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tj.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pd.521024.cn

[N05] 最大公约数
来源：http://md.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://yh.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jr.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gl.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jv.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ve.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://es.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://bl.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tk.asd995.cn

[N06] 判断回文字符串
来源：http://kh.nicolike.cn

Py:   s == s[::-1]
来源：http://xh.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://ky.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://bf.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://uc.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fw.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://ox.lnxyls.cn

Ruby: s == s.reverse
来源：http://ty.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uy.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://ie.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wn.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lr.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fb.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://fs.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://zl.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://me.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ln.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rq.lnxyls.cn

[N08] 生成全排列
来源：http://kg.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://wf.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://nk.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://vj.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://od.shxzukj.cn

Java: // 手写回溯递归
来源：http://rk.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://mq.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://yq.gzmigu.cn

C#:   // 手写回溯递归
来源：http://qy.chemitech.net.cn

[N09] 栈与队列
来源：http://cn.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uj.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://to.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://io.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ah.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yg.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ou.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kt.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yv.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://xk.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nj.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iq.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tr.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lo.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://vd.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yo.jianghongdianzi.cn


<!-- 参考信息 -->