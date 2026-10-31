代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://yw.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ex.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://mr.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dn.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ww.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nt.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yu.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lg.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ej.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yi.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yl.chemitech.net.cn

[K05] 深拷贝对象
来源：http://wd.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://di.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://oi.gzmigu.cn

JS:   structuredClone(obj)
来源：http://qh.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ql.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pv.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cn.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sc.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ou.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://ar.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xv.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vo.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nr.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cm.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fc.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jj.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xn.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ev.szxytkj.cn

[K07] 进制转换
来源：http://qv.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ot.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ro.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ve.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jl.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://la.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ii.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zm.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ho.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://pa.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://kp.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kg.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ax.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ti.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dr.asd995.cn

Go:   encoding/gob
来源：http://co.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://kp.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sn.newstarts.cn

================================================================================
来源：http://kg.szsharing.cn

L. 网络请求
来源：http://rc.jianghongdianzi.cn

================================================================================
来源：http://pg.lnxyls.cn

[L01] 发送 GET 请求
来源：http://wf.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kc.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nm.szxytkj.cn

JS:   await fetch(url)
来源：http://xc.lnxyls.cn

TS:   await fetch(url)
来源：http://rh.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kh.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://fq.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yv.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://mf.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tg.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oe.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rv.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nr.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gg.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rh.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zh.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uc.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://uc.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ka.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fr.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yc.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nd.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fa.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vj.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://td.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mq.huanxung.cn

[L04] 设置超时
来源：http://nf.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://kw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vl.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fz.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sr.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nf.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tu.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ub.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://de.nicolike.cn

[L05] 上传文件（multipart）
来源：http://qp.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hi.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xe.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://be.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yf.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zo.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tt.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gj.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dj.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://zk.bjjhwx.cn

Py:   resp.json()
来源：http://fa.asd995.cn

PHP:  json_decode($body, true);
来源：http://oo.huanxung.cn

JS:   await resp.json()
来源：http://ng.szsharing.cn

TS:   await resp.json()
来源：http://cm.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kt.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xm.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ow.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vh.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://dw.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mb.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nd.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://wg.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://qb.szxytkj.cn

Java: resp.statusCode()
来源：http://jt.bjjhwx.cn

Go:   resp.StatusCode
来源：http://mw.huanxung.cn

Ruby: resp.code.to_i
来源：http://op.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://ab.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://yf.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bn.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://zp.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jj.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lb.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pf.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://td.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zj.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zk.wgjwhj.cn

================================================================================
来源：http://dw.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://ql.muxihuayi.cn

================================================================================
来源：http://zb.colortex.cn

[M01] 读取命令行参数
来源：http://ct.nszjky.cn

Py:   sys.argv[1:]
来源：http://vf.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://bz.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://oq.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://mv.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://cn.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://cj.yuexingan06.cn

Ruby: ARGV
来源：http://xc.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://mh.shxzukj.cn

[M02] 读取环境变量
来源：http://ad.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://fv.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ex.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://zn.nszjky.cn

TS:   process.env.HOME
来源：http://yz.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://gg.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pr.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://lo.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bi.asd995.cn

[M03] 执行外部命令
来源：http://pn.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xs.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ve.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wy.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hq.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xp.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xy.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rc.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://he.newstarts.cn

[M04] 获取当前工作目录
来源：http://rn.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://jm.colortex.cn

PHP:  getcwd();
来源：http://lo.nszjky.cn

JS:   process.cwd()
来源：http://yo.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ay.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://vg.hnjuh.cn

Go:   os.Getwd()
来源：http://qz.wgjwhj.cn

Ruby: Dir.pwd
来源：http://yx.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ui.yuexingan06.cn

[M05] 设置退出码
来源：http://rt.shtwfgs.cn

Py:   sys.exit(1)
来源：http://fl.yuexingan06.cn

PHP:  exit(1);
来源：http://ap.shtwfgs.cn

JS:   process.exit(1)
来源：http://di.shtwfgs.cn

TS:   process.exit(1)
来源：http://of.shxzskj.cn

Java: System.exit(1)
来源：http://bs.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://gr.lnxyls.cn

Ruby: exit 1
来源：http://kp.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://im.shxzskj.cn

[M06] 向标准错误输出
来源：http://pj.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://xj.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ag.szsharing.cn

JS:   console.error("err")
来源：http://fj.hahajie.cn

TS:   console.error("err")
来源：http://qs.nicolike.cn

Java: System.err.println("err")
来源：http://bb.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qo.chemitech.net.cn

Ruby: warn "err"
来源：http://kp.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ni.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://jz.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://wy.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yz.521024.cn

JS:   require.main === module
来源：http://xx.shxzskj.cn

TS:   require.main === module
来源：http://dk.panjiajie.cn

Java: public static void main(String[] args)
来源：http://zq.bjjhwx.cn

Go:   func main()
来源：http://vz.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zk.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://nh.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://pt.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://wd.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://uy.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://mi.521024.cn

TS:   process.platform;  process.version
来源：http://vh.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lz.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yc.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cg.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gq.lnxyls.cn

================================================================================
来源：http://gm.nszjky.cn

N. 数据结构与算法
来源：http://gx.yuexingan06.cn

================================================================================
来源：http://ig.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://kv.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sl.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gi.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zh.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ub.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ic.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ex.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kc.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ht.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ch.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://fu.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cw.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yk.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kj.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://st.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ud.yuntaijiaju.cn

Ruby: arr.sort
来源：http://nr.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lh.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://rn.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jf.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://vy.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hg.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yo.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jl.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lb.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fj.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tr.lnxyls.cn

[N04] 斐波那契数列
来源：http://ch.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vo.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pb.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rz.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bg.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eb.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wb.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ty.shxzukj.cn

[N05] 最大公约数
来源：http://aj.szsharing.cn

Py:   math.gcd(a, b)
来源：http://hs.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fn.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://td.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rx.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://va.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vz.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://as.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yd.jctech888.com.cn

[N06] 判断回文字符串
来源：http://hs.nicolike.cn

Py:   s == s[::-1]
来源：http://sp.521024.cn

PHP:  $s === strrev($s);
来源：http://hd.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://gw.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://kt.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qb.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://pc.hnjuh.cn

Ruby: s == s.reverse
来源：http://gg.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wj.521024.cn

[N07] 两数之和（返回下标）
来源：http://gp.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mo.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qc.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://az.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://cb.szsharing.cn

Java: // 手写 HashMap
来源：http://ki.szsharing.cn

Go:   // 手写 map[int]int
来源：http://at.hnjuh.cn

Ruby: // 手写 Hash
来源：http://qu.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://my.shtwfgs.cn

[N08] 生成全排列
来源：http://yk.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://jh.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://si.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://wt.szsharing.cn

TS:   // 手写回溯递归
来源：http://bx.shxzskj.cn

Java: // 手写回溯递归
来源：http://ja.szsharing.cn

Go:   // 手写回溯递归
来源：http://wb.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://si.nicolike.cn

C#:   // 手写回溯递归
来源：http://cm.hahajie.cn

[N09] 栈与队列
来源：http://iz.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://es.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jd.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://px.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ed.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sn.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ez.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pa.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kq.bookmarksfly.cn

[N10] 链表节点定义
来源：http://lz.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ed.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hv.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oy.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nx.521024.cn

Java: class Node { int v; Node next; }
来源：http://ys.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qj.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://na.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fi.521024.cn

[N11] 二叉树中序遍历
来源：http://ay.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://as.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://gf.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tf.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://of.lnxyls.cn

Java: // 手写递归
来源：http://wp.gzmigu.cn

Go:   // 手写递归
来源：http://pb.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eh.huixiangedu.cn

C#:   // 手写递归
来源：http://kb.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tn.gzmigu.cn


<!-- 参考信息 -->