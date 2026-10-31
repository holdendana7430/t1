代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://lg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://av.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://cp.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oe.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qb.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wx.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ir.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rt.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ug.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nk.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qd.nszjky.cn

[K05] 深拷贝对象
来源：http://ty.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://pr.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://xy.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://hd.colortex.cn

TS:   structuredClone(obj)
来源：http://tv.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ig.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jd.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://to.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sa.nszjky.cn

[K06] 解析 URL 查询串
来源：http://sb.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hn.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yc.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xj.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zx.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ky.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cn.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iv.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://du.hnjuh.cn

[K07] 进制转换
来源：http://le.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fm.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uj.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yb.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wf.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jl.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jb.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qa.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gz.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://pr.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mm.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://dq.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://wo.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cz.newstarts.cn

Go:   encoding/gob
来源：http://gb.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://rp.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://om.panjiajie.cn

================================================================================
来源：http://dw.9csxet.cn

L. 网络请求
来源：http://zs.chemitech.net.cn

================================================================================
来源：http://co.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://kv.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zt.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gt.shxzukj.cn

JS:   await fetch(url)
来源：http://rf.nicolike.cn

TS:   await fetch(url)
来源：http://rw.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hg.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://pb.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qh.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cg.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://wa.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yl.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yj.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cq.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cy.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uw.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vm.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ip.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jq.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://sw.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://am.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ng.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vf.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eb.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mo.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mv.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sx.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lv.huanxung.cn

[L04] 设置超时
来源：http://az.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://vh.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vx.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tr.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://so.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ar.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rl.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nx.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uu.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ym.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yt.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bb.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jr.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zw.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ez.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bd.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bc.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rh.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://dl.huixiangedu.cn

Py:   resp.json()
来源：http://vy.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://kn.szsharing.cn

JS:   await resp.json()
来源：http://kg.asd995.cn

TS:   await resp.json()
来源：http://af.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rp.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tm.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://eu.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ie.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://rq.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qh.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://vg.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://sp.bjjhwx.cn

Java: resp.statusCode()
来源：http://bh.9csxet.cn

Go:   resp.StatusCode
来源：http://ma.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://gy.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ui.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://wg.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mw.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://ep.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eb.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aq.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://by.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gd.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dy.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nd.gzmigu.cn

================================================================================
来源：http://na.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://nd.huixinmuqiang.cn

================================================================================
来源：http://om.newstarts.cn

[M01] 读取命令行参数
来源：http://en.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://yq.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://kj.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://di.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://mc.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://by.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://jw.szsharing.cn

Ruby: ARGV
来源：http://oo.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://gl.shxzukj.cn

[M02] 读取环境变量
来源：http://bn.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://zb.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qc.panjiajie.cn

JS:   process.env.HOME
来源：http://uf.shxzukj.cn

TS:   process.env.HOME
来源：http://ms.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://zj.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mt.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ai.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fi.521024.cn

[M03] 执行外部命令
来源：http://nj.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lh.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ks.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gy.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fb.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ot.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vc.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rh.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://nl.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://ms.szsharing.cn

Py:   os.getcwd()
来源：http://ci.jianghongdianzi.cn

PHP:  getcwd();
来源：http://wz.panjiajie.cn

JS:   process.cwd()
来源：http://nr.chemitech.net.cn

TS:   process.cwd()
来源：http://jo.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ea.panjiajie.cn

Go:   os.Getwd()
来源：http://jl.newstarts.cn

Ruby: Dir.pwd
来源：http://na.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://di.szsharing.cn

[M05] 设置退出码
来源：http://vk.lnxyls.cn

Py:   sys.exit(1)
来源：http://jw.asd995.cn

PHP:  exit(1);
来源：http://ew.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://sz.yuexingan06.cn

TS:   process.exit(1)
来源：http://wu.huanxung.cn

Java: System.exit(1)
来源：http://id.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://zd.shxzukj.cn

Ruby: exit 1
来源：http://nr.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wg.asd995.cn

[M06] 向标准错误输出
来源：http://yw.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ka.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://he.shtwfgs.cn

JS:   console.error("err")
来源：http://eu.huixinmuqiang.cn

TS:   console.error("err")
来源：http://mt.521024.cn

Java: System.err.println("err")
来源：http://jy.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nu.colortex.cn

Ruby: warn "err"
来源：http://rw.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://rm.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://nz.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://th.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wg.bjjhwx.cn

JS:   require.main === module
来源：http://tm.hahajie.cn

TS:   require.main === module
来源：http://ow.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ex.huixinmuqiang.cn

Go:   func main()
来源：http://ps.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ac.colortex.cn

C#:   static void Main(string[] args)
来源：http://tu.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://nu.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://iz.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ei.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://lv.szxytkj.cn

TS:   process.platform;  process.version
来源：http://cb.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oa.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uc.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tb.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pl.shtwfgs.cn

================================================================================
来源：http://iz.huixinmuqiang.cn

N. 数据结构与算法
来源：http://zr.wgjwhj.cn

================================================================================
来源：http://ee.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://br.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ki.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ho.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qw.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sx.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://qa.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jr.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ls.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wf.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jh.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://df.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wd.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jd.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://oh.chemitech.net.cn

Ruby: arr.sort
来源：http://oc.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lj.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://cb.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pu.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://sn.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jp.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lx.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bk.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zp.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zn.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wj.haigaiapp.cn

[N04] 斐波那契数列
来源：http://us.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jn.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://er.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qw.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fu.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wp.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sk.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pw.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gd.nicolike.cn

[N05] 最大公约数
来源：http://qm.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://fk.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nd.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ag.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eo.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lu.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lr.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://rw.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zc.9csxet.cn

[N06] 判断回文字符串
来源：http://hx.panjiajie.cn

Py:   s == s[::-1]
来源：http://ok.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://tf.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ye.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://aq.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cl.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://dr.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://mw.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hi.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://is.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fr.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zi.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gk.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://xa.muxihuayi.cn

Java: // 手写 HashMap
来源：http://kw.asd995.cn

Go:   // 手写 map[int]int
来源：http://sj.gzmigu.cn

Ruby: // 手写 Hash
来源：http://os.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bd.jctech888.com.cn

[N08] 生成全排列
来源：http://do.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://qt.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://nm.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://qy.newstarts.cn

TS:   // 手写回溯递归
来源：http://kv.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://hf.szxytkj.cn

Go:   // 手写回溯递归
来源：http://ar.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://yw.shxzukj.cn

C#:   // 手写回溯递归
来源：http://qt.jctech888.com.cn

[N09] 栈与队列
来源：http://wj.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://el.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gs.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ax.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cy.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tm.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nr.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dc.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://td.colortex.cn

[N10] 链表节点定义
来源：http://kv.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cc.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hv.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zl.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vf.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://jc.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://im.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sa.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://db.hahajie.cn

[N11] 二叉树中序遍历
来源：http://wo.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tm.szxytkj.cn

PHP:  // 手写递归函数
来源：http://aq.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wk.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zx.shtwfgs.cn

Java: // 手写递归
来源：http://lv.yuntaijiaju.cn

Go:   // 手写递归
来源：http://mb.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ff.szxytkj.cn

C#:   // 手写递归
来源：http://ae.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://in.huixiangedu.cn


<!-- 参考信息 -->