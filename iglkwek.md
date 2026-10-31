代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wq.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gm.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://um.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mp.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mm.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yx.szsharing.cn

[K04] 读取 JSON 文件
来源：http://oj.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ly.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qc.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uc.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qa.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xq.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://no.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vf.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zh.haigaiapp.cn

[K05] 深拷贝对象
来源：http://lr.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://cu.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://py.lnxyls.cn

JS:   structuredClone(obj)
来源：http://hd.gzmigu.cn

TS:   structuredClone(obj)
来源：http://sg.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ii.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dg.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://la.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qp.asd995.cn

[K06] 解析 URL 查询串
来源：http://mn.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nr.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://se.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://em.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qh.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qq.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qa.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ub.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wb.bookmarksfly.cn

[K07] 进制转换
来源：http://iy.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jr.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://at.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xv.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fw.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rk.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mu.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lt.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ac.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://wn.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://id.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cf.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://eq.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://wi.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ri.colortex.cn

Go:   encoding/gob
来源：http://ib.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://iu.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ds.lnxyls.cn

================================================================================
来源：http://sb.szxytkj.cn

L. 网络请求
来源：http://jo.colortex.cn

================================================================================
来源：http://dz.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ch.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xq.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cs.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://nx.9csxet.cn

TS:   await fetch(url)
来源：http://mf.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lv.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ie.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rx.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zw.colortex.cn

[L02] 发送 POST JSON
来源：http://go.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pd.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ch.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://an.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nw.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qw.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://si.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hs.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wn.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://jw.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xa.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gr.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ci.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kc.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://js.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jr.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pw.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mv.huixiangedu.cn

[L04] 设置超时
来源：http://og.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://gy.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wy.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jr.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mx.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fm.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zg.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pj.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://at.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://lg.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jm.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tp.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gh.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://um.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pk.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xr.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xp.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://od.521024.cn

Py:   resp.json()
来源：http://kb.521024.cn

PHP:  json_decode($body, true);
来源：http://fo.wgjwhj.cn

JS:   await resp.json()
来源：http://di.newstarts.cn

TS:   await resp.json()
来源：http://qz.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dm.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ct.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://gd.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gp.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://gi.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fn.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pl.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://wv.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://hr.wgjwhj.cn

Java: resp.statusCode()
来源：http://ue.nicolike.cn

Go:   resp.StatusCode
来源：http://bx.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://cy.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://xn.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://wj.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zu.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ti.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dk.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uw.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qn.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lh.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rh.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ge.lnxyls.cn

================================================================================
来源：http://xo.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://rt.9csxet.cn

================================================================================
来源：http://io.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://vc.gzmigu.cn

Py:   sys.argv[1:]
来源：http://ph.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://fr.colortex.cn

JS:   process.argv.slice(2)
来源：http://ms.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://eb.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://pz.chemitech.net.cn

Go:   os.Args[1:]
来源：http://bp.nicolike.cn

Ruby: ARGV
来源：http://ny.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://kp.asd995.cn

[M02] 读取环境变量
来源：http://zi.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://pb.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ws.muxihuayi.cn

JS:   process.env.HOME
来源：http://bo.yuexingan06.cn

TS:   process.env.HOME
来源：http://rz.huanxung.cn

Java: System.getenv("HOME")
来源：http://ms.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mq.nicolike.cn

Ruby: ENV["HOME"]
来源：http://yc.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dk.colortex.cn

[M03] 执行外部命令
来源：http://fi.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kr.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fu.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zq.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://va.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nr.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gp.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ej.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ok.9csxet.cn

[M04] 获取当前工作目录
来源：http://wk.nicolike.cn

Py:   os.getcwd()
来源：http://sz.szsharing.cn

PHP:  getcwd();
来源：http://dv.nicolike.cn

JS:   process.cwd()
来源：http://fx.huanxung.cn

TS:   process.cwd()
来源：http://tm.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://gk.panjiajie.cn

Go:   os.Getwd()
来源：http://kk.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ll.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pg.nszjky.cn

[M05] 设置退出码
来源：http://uq.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://kp.hahajie.cn

PHP:  exit(1);
来源：http://gz.hahajie.cn

JS:   process.exit(1)
来源：http://fd.szsharing.cn

TS:   process.exit(1)
来源：http://gt.asd995.cn

Java: System.exit(1)
来源：http://sx.huixiangedu.cn

Go:   os.Exit(1)
来源：http://jh.szsharing.cn

Ruby: exit 1
来源：http://bm.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dh.nicolike.cn

[M06] 向标准错误输出
来源：http://qq.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://eu.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ke.bjjhwx.cn

JS:   console.error("err")
来源：http://oc.haigaiapp.cn

TS:   console.error("err")
来源：http://rx.lnxyls.cn

Java: System.err.println("err")
来源：http://bk.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jg.9csxet.cn

Ruby: warn "err"
来源：http://mr.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://pl.panjiajie.cn

[M07] 判断是否为主入口
来源：http://td.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://db.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vm.jctech888.com.cn

JS:   require.main === module
来源：http://cf.haigaiapp.cn

TS:   require.main === module
来源：http://np.huanxung.cn

Java: public static void main(String[] args)
来源：http://nl.huixiangedu.cn

Go:   func main()
来源：http://vl.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nx.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ey.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://bc.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://pn.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://xs.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://re.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://hv.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ht.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lq.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://db.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yz.asd995.cn

================================================================================
来源：http://na.szsharing.cn

N. 数据结构与算法
来源：http://ft.newstarts.cn

================================================================================
来源：http://hl.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://hq.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lu.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ui.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ar.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://up.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qt.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://eg.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ol.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ft.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://sg.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ur.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jn.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://df.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ue.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ix.newstarts.cn

Go:   slices.Sort(arr)
来源：http://jj.huixiangedu.cn

Ruby: arr.sort
来源：http://yl.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gu.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://dt.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kv.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ge.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vz.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uy.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gp.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kn.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cf.lnxyls.cn

[N04] 斐波那契数列
来源：http://dw.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wh.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://di.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dt.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fu.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://de.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bn.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://di.jctech888.com.cn

[N05] 最大公约数
来源：http://my.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://me.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kw.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ty.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lo.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vb.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fc.hnjuh.cn

Ruby: a.gcd(b)
来源：http://jh.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dq.asd995.cn

[N06] 判断回文字符串
来源：http://zh.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://zx.521024.cn

PHP:  $s === strrev($s);
来源：http://ie.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://jp.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://ym.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pm.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://fu.9csxet.cn

Ruby: s == s.reverse
来源：http://cc.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dm.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://zh.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ld.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aq.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://up.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ej.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://jl.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ds.hahajie.cn

Ruby: // 手写 Hash
来源：http://cs.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cb.lnxyls.cn

[N08] 生成全排列
来源：http://th.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://rd.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://tc.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ti.521024.cn

TS:   // 手写回溯递归
来源：http://tu.yuexingan06.cn

Java: // 手写回溯递归
来源：http://oi.nszjky.cn

Go:   // 手写回溯递归
来源：http://pd.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://nn.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://eb.szxytkj.cn

[N09] 栈与队列
来源：http://ob.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rm.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zp.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xp.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ri.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eb.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mx.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zk.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://il.shxzukj.cn

[N10] 链表节点定义
来源：http://tz.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fc.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fz.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gr.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kg.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://jo.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ws.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gt.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qe.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://hf.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hb.huanxung.cn

PHP:  // 手写递归函数
来源：http://hq.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eg.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uw.haigaiapp.cn

Java: // 手写递归
来源：http://pd.shxzskj.cn


<!-- 参考信息 -->