代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://co.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ye.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://px.nszjky.cn

[K05] 深拷贝对象
来源：http://dy.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://do.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://pz.asd995.cn

JS:   structuredClone(obj)
来源：http://qn.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://uc.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://co.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kk.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nb.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gk.huanxung.cn

[K06] 解析 URL 查询串
来源：http://fa.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qe.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pu.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mo.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oy.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mk.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xv.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jj.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wa.bookmarksfly.cn

[K07] 进制转换
来源：http://ac.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ly.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://br.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rs.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wt.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tp.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uc.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hn.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fw.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ei.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://xe.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nz.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://pn.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://uu.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kv.huixiangedu.cn

Go:   encoding/gob
来源：http://qe.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://kz.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jq.panjiajie.cn

================================================================================
来源：http://bm.haigaiapp.cn

L. 网络请求
来源：http://az.gzmigu.cn

================================================================================
来源：http://dh.9csxet.cn

[L01] 发送 GET 请求
来源：http://fz.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kv.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://an.chemitech.net.cn

JS:   await fetch(url)
来源：http://tn.szsharing.cn

TS:   await fetch(url)
来源：http://cl.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dk.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ke.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pa.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ny.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://sc.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://to.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ya.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uj.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ie.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vc.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kj.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://an.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bc.shxzukj.cn

[L03] 设置自定义请求头
来源：http://df.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uq.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nt.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hy.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://db.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ym.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ty.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fr.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ts.bookmarksfly.cn

[L04] 设置超时
来源：http://fa.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://xp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ce.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aa.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wk.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zx.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ye.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wd.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://uq.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ew.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bu.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wl.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://om.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lh.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nj.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pw.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lh.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://ts.chemitech.net.cn

Py:   resp.json()
来源：http://rm.nicolike.cn

PHP:  json_decode($body, true);
来源：http://rk.shxzskj.cn

JS:   await resp.json()
来源：http://pl.newstarts.cn

TS:   await resp.json()
来源：http://vx.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tn.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wh.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://tu.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tx.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ms.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xw.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ln.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://uw.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://id.shxzskj.cn

Java: resp.statusCode()
来源：http://ef.9csxet.cn

Go:   resp.StatusCode
来源：http://la.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://eh.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ft.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://dh.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tv.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://hc.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ht.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sg.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ve.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nk.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://as.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jl.haigaiapp.cn

================================================================================
来源：http://zb.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://hx.nszjky.cn

================================================================================
来源：http://ux.bjjhwx.cn

[M01] 读取命令行参数
来源：http://wr.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://im.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://sj.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://cu.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://fb.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://ov.shxzukj.cn

Go:   os.Args[1:]
来源：http://da.szxytkj.cn

Ruby: ARGV
来源：http://vx.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://mc.szsharing.cn

[M02] 读取环境变量
来源：http://gv.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ui.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jx.bjjhwx.cn

JS:   process.env.HOME
来源：http://by.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://uf.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://xl.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qw.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://xa.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.hnjuh.cn

[M03] 执行外部命令
来源：http://rv.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kn.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://si.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pn.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dd.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mq.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eb.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pu.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://mp.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://ss.gzmigu.cn

Py:   os.getcwd()
来源：http://ow.yuntaijiaju.cn

PHP:  getcwd();
来源：http://ho.hahajie.cn

JS:   process.cwd()
来源：http://ec.haigaiapp.cn

TS:   process.cwd()
来源：http://dc.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://eu.nicolike.cn

Go:   os.Getwd()
来源：http://vi.haigaiapp.cn

Ruby: Dir.pwd
来源：http://oz.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vp.gzmigu.cn

[M05] 设置退出码
来源：http://lp.huanxung.cn

Py:   sys.exit(1)
来源：http://fk.jctech888.com.cn

PHP:  exit(1);
来源：http://sx.panjiajie.cn

JS:   process.exit(1)
来源：http://lj.newstarts.cn

TS:   process.exit(1)
来源：http://jc.shxzukj.cn

Java: System.exit(1)
来源：http://sn.panjiajie.cn

Go:   os.Exit(1)
来源：http://jr.newstarts.cn

Ruby: exit 1
来源：http://sl.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://je.colortex.cn

[M06] 向标准错误输出
来源：http://bi.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ml.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zp.9csxet.cn

JS:   console.error("err")
来源：http://ya.chemitech.net.cn

TS:   console.error("err")
来源：http://ou.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://xl.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rk.yuexingan06.cn

Ruby: warn "err"
来源：http://so.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://xw.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://oz.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://hy.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xk.huixiangedu.cn

JS:   require.main === module
来源：http://hr.521024.cn

TS:   require.main === module
来源：http://vz.shxzskj.cn

Java: public static void main(String[] args)
来源：http://pq.szxytkj.cn

Go:   func main()
来源：http://ku.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ud.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://zn.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://ej.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://gd.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://po.szsharing.cn

JS:   process.platform;  process.version
来源：http://ie.newstarts.cn

TS:   process.platform;  process.version
来源：http://lb.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gh.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ec.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vv.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hv.9csxet.cn

================================================================================
来源：http://oj.haigaiapp.cn

N. 数据结构与算法
来源：http://bg.chemitech.net.cn

================================================================================
来源：http://ij.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://as.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gy.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aj.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gg.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mn.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://zz.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vi.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nx.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://pq.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ly.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mc.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zg.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gw.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sd.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://vb.9csxet.cn

Ruby: arr.sort
来源：http://kj.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xa.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://ne.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rr.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ax.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oa.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zm.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kz.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vb.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bc.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zc.lnxyls.cn

[N04] 斐波那契数列
来源：http://xy.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nj.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hr.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cw.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ls.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iw.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ye.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bb.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zu.nicolike.cn

[N05] 最大公约数
来源：http://av.asd995.cn

Py:   math.gcd(a, b)
来源：http://of.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://no.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uj.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nd.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mj.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rl.hnjuh.cn

Ruby: a.gcd(b)
来源：http://xd.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://we.lnxyls.cn

[N06] 判断回文字符串
来源：http://rf.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://li.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://kj.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://rf.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ll.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oc.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://yv.521024.cn

Ruby: s == s.reverse
来源：http://ig.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gg.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://og.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wk.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tu.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://is.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://xy.nicolike.cn

Java: // 手写 HashMap
来源：http://dj.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://yq.huanxung.cn

Ruby: // 手写 Hash
来源：http://wc.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://to.colortex.cn

[N08] 生成全排列
来源：http://vb.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://ar.nicolike.cn

PHP:  // 手写递归交换
来源：http://yv.nszjky.cn

JS:   // 手写回溯递归
来源：http://zn.szsharing.cn

TS:   // 手写回溯递归
来源：http://tk.bjjhwx.cn

Java: // 手写回溯递归
来源：http://kb.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ih.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://zs.shxzskj.cn

C#:   // 手写回溯递归
来源：http://jk.panjiajie.cn

[N09] 栈与队列
来源：http://fj.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yx.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rs.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hj.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nr.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vp.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://du.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ge.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bk.szsharing.cn

[N10] 链表节点定义
来源：http://et.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vn.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zv.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dh.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fj.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://pt.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tn.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lw.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://id.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://de.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gb.gzmigu.cn

PHP:  // 手写递归函数
来源：http://lq.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uk.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://se.yuexingan06.cn

Java: // 手写递归
来源：http://dr.panjiajie.cn

Go:   // 手写递归
来源：http://ap.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oh.jianghongdianzi.cn

C#:   // 手写递归
来源：http://lq.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fq.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mg.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mz.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dy.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://by.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ml.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://im.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nl.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fp.hahajie.cn


<!-- 参考信息 -->