代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sb.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vf.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ag.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sm.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yq.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://me.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://so.chemitech.net.cn

[K05] 深拷贝对象
来源：http://ky.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://gw.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://yn.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://br.shxzskj.cn

TS:   structuredClone(obj)
来源：http://qf.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ml.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ve.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yr.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fz.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://qz.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hi.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sl.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://po.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sf.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zl.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bi.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xi.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://et.nszjky.cn

[K07] 进制转换
来源：http://zu.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vs.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qm.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xh.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ep.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ij.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lp.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mn.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://ee.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://cp.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ux.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://gq.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://nn.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ka.szsharing.cn

Go:   encoding/gob
来源：http://xz.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://ny.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ax.gzmigu.cn

================================================================================
来源：http://ql.jctech888.com.cn

L. 网络请求
来源：http://gy.colortex.cn

================================================================================
来源：http://gq.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ia.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ne.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bn.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://cs.haigaiapp.cn

TS:   await fetch(url)
来源：http://we.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ll.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://fx.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qg.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cq.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ha.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ql.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ma.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lh.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pg.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dd.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mv.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xi.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mm.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://rd.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zc.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://so.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ic.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zy.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ee.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xi.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pf.gzmigu.cn

[L04] 设置超时
来源：http://tq.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://gr.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xo.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zq.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ty.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ju.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rw.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://br.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hm.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ti.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mm.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://om.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mm.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lm.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ei.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uj.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qa.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://br.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://yr.521024.cn

Py:   resp.json()
来源：http://ih.asd995.cn

PHP:  json_decode($body, true);
来源：http://ty.gzmigu.cn

JS:   await resp.json()
来源：http://qn.shtwfgs.cn

TS:   await resp.json()
来源：http://zo.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ng.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tl.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://am.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dk.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://jp.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vb.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ab.asd995.cn

JS:   resp.ok;  resp.status
来源：http://iv.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://bc.colortex.cn

Java: resp.statusCode()
来源：http://pi.szsharing.cn

Go:   resp.StatusCode
来源：http://ob.shxzukj.cn

Ruby: resp.code.to_i
来源：http://pi.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://do.szxytkj.cn

[L08] 并发请求多个地址
来源：http://jg.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://va.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://rm.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rm.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://od.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mo.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iz.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uw.haigaiapp.cn

================================================================================
来源：http://oy.521024.cn

M. 命令行 / 进程 / 环境
来源：http://bc.newstarts.cn

================================================================================
来源：http://hp.shxzskj.cn

[M01] 读取命令行参数
来源：http://pf.szsharing.cn

Py:   sys.argv[1:]
来源：http://zn.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://lx.nicolike.cn

JS:   process.argv.slice(2)
来源：http://df.nicolike.cn

TS:   process.argv.slice(2)
来源：http://nh.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://rq.szxytkj.cn

Go:   os.Args[1:]
来源：http://qx.lnxyls.cn

Ruby: ARGV
来源：http://dt.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://du.jctech888.com.cn

[M02] 读取环境变量
来源：http://nb.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://ht.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ki.shxzukj.cn

JS:   process.env.HOME
来源：http://jw.bookmarksfly.cn

TS:   process.env.HOME
来源：http://bh.hahajie.cn

Java: System.getenv("HOME")
来源：http://jx.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fg.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://cc.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fp.gzmigu.cn

[M03] 执行外部命令
来源：http://rw.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uv.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xd.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bn.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sv.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wh.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nw.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zl.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://aj.gzmigu.cn

[M04] 获取当前工作目录
来源：http://um.nicolike.cn

Py:   os.getcwd()
来源：http://rc.wgjwhj.cn

PHP:  getcwd();
来源：http://xn.shtwfgs.cn

JS:   process.cwd()
来源：http://mk.bookmarksfly.cn

TS:   process.cwd()
来源：http://hu.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://st.hahajie.cn

Go:   os.Getwd()
来源：http://to.shxzukj.cn

Ruby: Dir.pwd
来源：http://za.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uf.muxihuayi.cn

[M05] 设置退出码
来源：http://vn.szxytkj.cn

Py:   sys.exit(1)
来源：http://mp.szxytkj.cn

PHP:  exit(1);
来源：http://fa.shxzukj.cn

JS:   process.exit(1)
来源：http://fz.shxzukj.cn

TS:   process.exit(1)
来源：http://pe.yuexingan06.cn

Java: System.exit(1)
来源：http://uo.szxytkj.cn

Go:   os.Exit(1)
来源：http://oq.nicolike.cn

Ruby: exit 1
来源：http://ve.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dg.lnxyls.cn

[M06] 向标准错误输出
来源：http://ea.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://yu.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ow.shxzskj.cn

JS:   console.error("err")
来源：http://cs.huixinmuqiang.cn

TS:   console.error("err")
来源：http://er.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://oj.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tv.521024.cn

Ruby: warn "err"
来源：http://mp.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://yf.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://wp.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://ay.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ka.szxytkj.cn

JS:   require.main === module
来源：http://mg.newstarts.cn

TS:   require.main === module
来源：http://qm.szxytkj.cn

Java: public static void main(String[] args)
来源：http://hw.chemitech.net.cn

Go:   func main()
来源：http://ha.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hv.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://nf.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://ed.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://xn.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://ru.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://rh.szsharing.cn

TS:   process.platform;  process.version
来源：http://uw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vz.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ww.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hm.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eq.huixiangedu.cn

================================================================================
来源：http://oy.muxihuayi.cn

N. 数据结构与算法
来源：http://jl.huixinmuqiang.cn

================================================================================
来源：http://br.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://tv.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xb.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bx.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://co.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rj.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hk.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://kq.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gm.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ul.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://of.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://do.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kz.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://do.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wd.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vy.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://kg.huanxung.cn

Ruby: arr.sort
来源：http://ua.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nu.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://wh.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hs.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://df.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tm.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gy.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rs.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qx.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zz.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xo.521024.cn

[N04] 斐波那契数列
来源：http://es.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ss.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ks.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wg.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wh.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://si.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lf.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://be.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://in.521024.cn

[N05] 最大公约数
来源：http://pa.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://bn.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ql.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oi.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kv.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hy.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jp.panjiajie.cn

Ruby: a.gcd(b)
来源：http://dx.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wt.huanxung.cn

[N06] 判断回文字符串
来源：http://er.panjiajie.cn

Py:   s == s[::-1]
来源：http://ey.newstarts.cn

PHP:  $s === strrev($s);
来源：http://hb.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://vi.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://pt.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uj.huanxung.cn

Go:   // 双指针从两端比较
来源：http://kz.asd995.cn

Ruby: s == s.reverse
来源：http://av.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://un.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ug.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jl.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sm.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://hr.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://me.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://vt.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://gg.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wi.shxzukj.cn

[N08] 生成全排列
来源：http://uo.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://oj.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://mn.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://eo.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://ty.bjjhwx.cn

Java: // 手写回溯递归
来源：http://dj.hahajie.cn

Go:   // 手写回溯递归
来源：http://ie.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://bn.newstarts.cn

C#:   // 手写回溯递归
来源：http://cg.shxzukj.cn

[N09] 栈与队列
来源：http://zz.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dx.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lm.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zw.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ps.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pe.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mb.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lv.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mu.bjjhwx.cn

[N10] 链表节点定义
来源：http://ue.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zm.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fc.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kn.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bq.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://mv.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cd.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gp.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oe.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://yh.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uh.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://pb.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ly.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tf.shtwfgs.cn

Java: // 手写递归
来源：http://fs.nszjky.cn

Go:   // 手写递归
来源：http://px.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fc.yuexingan06.cn

C#:   // 手写递归
来源：http://wh.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ey.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nc.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dg.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ye.yuexingan06.cn


<!-- 参考信息 -->