代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jw.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zo.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bc.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qh.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nb.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rr.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sx.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ty.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gk.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bw.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://nr.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fu.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vu.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fl.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fy.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://va.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tj.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ag.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sm.muxihuayi.cn

[K05] 深拷贝对象
来源：http://nz.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://fi.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ic.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://fm.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://gd.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gu.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://es.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://og.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dd.szsharing.cn

[K06] 解析 URL 查询串
来源：http://cu.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yk.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://un.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cg.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cn.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fs.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ig.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dy.shxzukj.cn

[K07] 进制转换
来源：http://zk.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kt.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://af.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://au.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hi.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ha.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xg.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ig.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qj.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://zc.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://pv.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nb.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://qd.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://bw.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ds.hnjuh.cn

Go:   encoding/gob
来源：http://vq.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://sy.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://st.huixinmuqiang.cn

================================================================================
来源：http://uk.bookmarksfly.cn

L. 网络请求
来源：http://wp.huixinmuqiang.cn

================================================================================
来源：http://hn.shxzskj.cn

[L01] 发送 GET 请求
来源：http://sa.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lt.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://db.jctech888.com.cn

JS:   await fetch(url)
来源：http://tg.nszjky.cn

TS:   await fetch(url)
来源：http://ad.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dh.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://ju.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ib.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wy.gzmigu.cn

[L02] 发送 POST JSON
来源：http://tb.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://as.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ry.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ts.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lr.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yf.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cd.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kk.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ne.nszjky.cn

[L03] 设置自定义请求头
来源：http://fy.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lo.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ch.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jt.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bo.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bh.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sl.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rx.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ba.lnxyls.cn

[L04] 设置超时
来源：http://sg.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ze.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rq.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gf.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wt.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lt.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jp.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://si.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://md.9csxet.cn

[L05] 上传文件（multipart）
来源：http://rq.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ss.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yt.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kq.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://st.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://up.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mc.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nl.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wf.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://cr.521024.cn

Py:   resp.json()
来源：http://np.szsharing.cn

PHP:  json_decode($body, true);
来源：http://na.hahajie.cn

JS:   await resp.json()
来源：http://uz.gzmigu.cn

TS:   await resp.json()
来源：http://ez.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ac.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://va.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://av.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dh.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://on.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cs.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pc.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://ne.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://vk.nszjky.cn

Java: resp.statusCode()
来源：http://bx.lnxyls.cn

Go:   resp.StatusCode
来源：http://ad.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://tn.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://fk.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://bu.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sm.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://og.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ki.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xr.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ak.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kp.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sv.shxzukj.cn

================================================================================
来源：http://kv.521024.cn

M. 命令行 / 进程 / 环境
来源：http://lr.yuexingan06.cn

================================================================================
来源：http://xa.521024.cn

[M01] 读取命令行参数
来源：http://pk.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://os.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://df.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://dg.9csxet.cn

TS:   process.argv.slice(2)
来源：http://zt.521024.cn

Java: args 数组（main 方法参数）
来源：http://tn.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ob.yuexingan06.cn

Ruby: ARGV
来源：http://oj.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://ts.hnjuh.cn

[M02] 读取环境变量
来源：http://de.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://dp.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bi.asd995.cn

JS:   process.env.HOME
来源：http://sv.521024.cn

TS:   process.env.HOME
来源：http://mg.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://kc.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pi.hahajie.cn

Ruby: ENV["HOME"]
来源：http://fi.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pt.shxzskj.cn

[M03] 执行外部命令
来源：http://yx.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vi.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fq.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://si.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bh.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oy.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://my.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vb.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://po.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://ri.nszjky.cn

Py:   os.getcwd()
来源：http://kz.huixinmuqiang.cn

PHP:  getcwd();
来源：http://tv.jianghongdianzi.cn

JS:   process.cwd()
来源：http://ph.szsharing.cn

TS:   process.cwd()
来源：http://tl.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ml.lnxyls.cn

Go:   os.Getwd()
来源：http://un.huixiangedu.cn

Ruby: Dir.pwd
来源：http://xr.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oi.newstarts.cn

[M05] 设置退出码
来源：http://ym.newstarts.cn

Py:   sys.exit(1)
来源：http://ip.yuexingan06.cn

PHP:  exit(1);
来源：http://zf.huixiangedu.cn

JS:   process.exit(1)
来源：http://uk.yuexingan06.cn

TS:   process.exit(1)
来源：http://wu.shxzskj.cn

Java: System.exit(1)
来源：http://hv.shtwfgs.cn

Go:   os.Exit(1)
来源：http://vv.jianghongdianzi.cn

Ruby: exit 1
来源：http://ii.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nb.nszjky.cn

[M06] 向标准错误输出
来源：http://nd.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ow.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://po.shxzskj.cn

JS:   console.error("err")
来源：http://oi.nszjky.cn

TS:   console.error("err")
来源：http://qi.haigaiapp.cn

Java: System.err.println("err")
来源：http://pt.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qh.huixinmuqiang.cn

Ruby: warn "err"
来源：http://st.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://fg.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://pn.asd995.cn

Py:   if __name__ == "__main__":
来源：http://zn.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ha.yuexingan06.cn

JS:   require.main === module
来源：http://uj.9csxet.cn

TS:   require.main === module
来源：http://nj.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://nj.huixinmuqiang.cn

Go:   func main()
来源：http://kv.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qo.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://kr.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ft.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://he.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yw.nszjky.cn

JS:   process.platform;  process.version
来源：http://lb.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://rt.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vo.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dp.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rb.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://av.szxytkj.cn

================================================================================
来源：http://pr.huixinmuqiang.cn

N. 数据结构与算法
来源：http://ah.521024.cn

================================================================================
来源：http://vy.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://lz.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vm.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tz.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bf.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lb.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jp.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://cm.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xm.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oy.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://iv.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ks.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lh.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mn.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sj.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ua.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://rz.yuexingan06.cn

Ruby: arr.sort
来源：http://wa.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nr.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://ns.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://db.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://nl.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mc.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yx.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lu.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mb.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dt.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eu.shxzskj.cn

[N04] 斐波那契数列
来源：http://yl.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mb.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jq.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gk.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uj.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sd.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uj.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oo.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sd.bookmarksfly.cn

[N05] 最大公约数
来源：http://jj.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://vc.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://we.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iq.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wq.nszjky.cn

Ruby: a.gcd(b)
来源：http://gh.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fy.nicolike.cn

[N06] 判断回文字符串
来源：http://bw.huanxung.cn

Py:   s == s[::-1]
来源：http://st.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://jm.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://yx.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://gl.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tz.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://si.hahajie.cn

Ruby: s == s.reverse
来源：http://ia.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lz.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://py.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://px.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bh.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wx.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://tf.muxihuayi.cn

Java: // 手写 HashMap
来源：http://im.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://dz.huanxung.cn

Ruby: // 手写 Hash
来源：http://pe.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mz.panjiajie.cn

[N08] 生成全排列
来源：http://uo.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://yj.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://ls.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://zm.shxzukj.cn

TS:   // 手写回溯递归
来源：http://eu.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://lq.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://hj.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ir.521024.cn

C#:   // 手写回溯递归
来源：http://eq.jctech888.com.cn

[N09] 栈与队列
来源：http://ll.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nq.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dn.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bh.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kw.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kk.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sc.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mr.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lg.521024.cn

[N10] 链表节点定义
来源：http://qg.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wz.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ro.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wd.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fd.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://zz.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ep.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mk.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vc.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://cw.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kb.gzmigu.cn


<!-- 参考信息 -->