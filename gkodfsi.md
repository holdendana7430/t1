代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ml.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bn.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ji.shxzskj.cn

[K05] 深拷贝对象
来源：http://ki.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://wq.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ij.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://qk.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://tf.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ka.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bg.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tg.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ul.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://yb.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://js.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sk.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gn.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vp.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ri.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tf.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pi.nszjky.cn

[K07] 进制转换
来源：http://is.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mr.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ui.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dt.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vg.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://al.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ik.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ue.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ut.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://jp.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://gq.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cw.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://fu.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://nm.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://as.yuntaijiaju.cn

Go:   encoding/gob
来源：http://vz.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://hd.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dh.asd995.cn

================================================================================
来源：http://tf.yuexingan06.cn

L. 网络请求
来源：http://vh.nicolike.cn

================================================================================
来源：http://ou.colortex.cn

[L01] 发送 GET 请求
来源：http://gz.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gb.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pu.huixiangedu.cn

JS:   await fetch(url)
来源：http://he.chemitech.net.cn

TS:   await fetch(url)
来源：http://tz.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yt.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://jy.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://af.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sk.hnjuh.cn

[L02] 发送 POST JSON
来源：http://ew.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mt.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qd.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ss.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://os.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gq.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ad.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xd.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nh.asd995.cn

[L03] 设置自定义请求头
来源：http://du.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bg.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://to.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ia.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qj.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gr.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ff.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://md.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kb.gzmigu.cn

[L04] 设置超时
来源：http://rg.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://yi.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hj.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sl.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sy.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jy.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lc.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vq.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dr.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://mv.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yi.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zi.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nk.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zu.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lm.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tj.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ol.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iu.hahajie.cn

[L06] 解析响应为 JSON
来源：http://dv.9csxet.cn

Py:   resp.json()
来源：http://ne.asd995.cn

PHP:  json_decode($body, true);
来源：http://az.yuexingan06.cn

JS:   await resp.json()
来源：http://ho.szxytkj.cn

TS:   await resp.json()
来源：http://yz.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://np.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zz.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://en.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jh.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ix.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qu.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xg.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ya.asd995.cn

TS:   resp.ok;  resp.status
来源：http://gz.muxihuayi.cn

Java: resp.statusCode()
来源：http://wt.nicolike.cn

Go:   resp.StatusCode
来源：http://tt.nicolike.cn

Ruby: resp.code.to_i
来源：http://xs.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://gi.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://tz.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://um.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://su.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ip.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gd.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hx.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kc.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qs.muxihuayi.cn

================================================================================
来源：http://qj.521024.cn

M. 命令行 / 进程 / 环境
来源：http://bo.nszjky.cn

================================================================================
来源：http://kj.huanxung.cn

[M01] 读取命令行参数
来源：http://sh.shxzukj.cn

Py:   sys.argv[1:]
来源：http://pv.521024.cn

PHP:  $argv;  $argc;
来源：http://xp.colortex.cn

JS:   process.argv.slice(2)
来源：http://xo.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://kn.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://wj.shxzskj.cn

Go:   os.Args[1:]
来源：http://gx.shtwfgs.cn

Ruby: ARGV
来源：http://nf.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jp.nszjky.cn

[M02] 读取环境变量
来源：http://mo.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://vn.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sm.lnxyls.cn

JS:   process.env.HOME
来源：http://nf.bjjhwx.cn

TS:   process.env.HOME
来源：http://wk.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://ie.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ey.nszjky.cn

Ruby: ENV["HOME"]
来源：http://jv.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vn.jctech888.com.cn

[M03] 执行外部命令
来源：http://ii.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jc.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wz.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tc.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yo.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xa.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rd.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xp.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ov.lnxyls.cn

[M04] 获取当前工作目录
来源：http://gb.hahajie.cn

Py:   os.getcwd()
来源：http://rq.lnxyls.cn

PHP:  getcwd();
来源：http://fi.huixiangedu.cn

JS:   process.cwd()
来源：http://zd.huixinmuqiang.cn

TS:   process.cwd()
来源：http://bd.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://kt.haigaiapp.cn

Go:   os.Getwd()
来源：http://it.9csxet.cn

Ruby: Dir.pwd
来源：http://fl.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ad.jianghongdianzi.cn

[M05] 设置退出码
来源：http://gy.huanxung.cn

Py:   sys.exit(1)
来源：http://au.chemitech.net.cn

PHP:  exit(1);
来源：http://ss.nszjky.cn

JS:   process.exit(1)
来源：http://jr.huanxung.cn

TS:   process.exit(1)
来源：http://la.panjiajie.cn

Java: System.exit(1)
来源：http://ui.shxzskj.cn

Go:   os.Exit(1)
来源：http://xk.nszjky.cn

Ruby: exit 1
来源：http://bh.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kb.yuexingan06.cn

[M06] 向标准错误输出
来源：http://am.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://rv.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vx.panjiajie.cn

JS:   console.error("err")
来源：http://gv.hnjuh.cn

TS:   console.error("err")
来源：http://ss.huanxung.cn

Java: System.err.println("err")
来源：http://el.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jw.chemitech.net.cn

Ruby: warn "err"
来源：http://cq.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://et.hahajie.cn

[M07] 判断是否为主入口
来源：http://ms.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://gz.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dv.muxihuayi.cn

JS:   require.main === module
来源：http://ud.nszjky.cn

TS:   require.main === module
来源：http://pv.lnxyls.cn

Java: public static void main(String[] args)
来源：http://zw.yuntaijiaju.cn

Go:   func main()
来源：http://dt.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ke.szsharing.cn

C#:   static void Main(string[] args)
来源：http://vj.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://du.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ua.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://db.szsharing.cn

JS:   process.platform;  process.version
来源：http://nw.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://cy.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tm.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kg.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bx.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://at.szsharing.cn

================================================================================
来源：http://gi.nszjky.cn

N. 数据结构与算法
来源：http://pv.shtwfgs.cn

================================================================================
来源：http://lq.colortex.cn

[N01] 二分查找（有序数组）
来源：http://nl.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://or.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lp.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bb.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://py.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sc.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://et.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ta.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://un.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://kw.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://ze.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://je.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rw.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://di.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qn.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ca.asd995.cn

Ruby: arr.sort
来源：http://ls.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yh.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://kw.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vn.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://dq.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ou.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mt.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cb.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oh.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bd.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xj.bjjhwx.cn

[N04] 斐波那契数列
来源：http://km.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tt.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rz.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qq.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fx.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qy.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hm.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xm.yuntaijiaju.cn

[N05] 最大公约数
来源：http://hg.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://gz.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ad.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ru.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nv.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sq.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://di.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://yc.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lv.nszjky.cn

[N06] 判断回文字符串
来源：http://js.newstarts.cn

Py:   s == s[::-1]
来源：http://be.hahajie.cn

PHP:  $s === strrev($s);
来源：http://fg.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://mx.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://hu.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ub.521024.cn

Go:   // 双指针从两端比较
来源：http://jd.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://hm.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vd.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://hg.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hl.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ik.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qa.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://rb.huanxung.cn

Java: // 手写 HashMap
来源：http://ff.hahajie.cn

Go:   // 手写 map[int]int
来源：http://vx.szxytkj.cn

Ruby: // 手写 Hash
来源：http://qj.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vw.bjjhwx.cn

[N08] 生成全排列
来源：http://qc.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://yg.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://uw.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://bt.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://sr.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://cc.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ib.colortex.cn

Ruby: arr.permutation.to_a
来源：http://ij.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://jy.szsharing.cn

[N09] 栈与队列
来源：http://vw.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xd.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lw.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vv.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nh.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kq.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oz.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zf.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ij.colortex.cn

[N10] 链表节点定义
来源：http://jv.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mh.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ue.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ua.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://ct.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ox.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zk.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://en.asd995.cn

[N11] 二叉树中序遍历
来源：http://li.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://on.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://me.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jv.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cy.9csxet.cn

Java: // 手写递归
来源：http://wb.muxihuayi.cn

Go:   // 手写递归
来源：http://iw.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gd.jctech888.com.cn

C#:   // 手写递归
来源：http://oo.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ci.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bz.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pt.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://js.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kv.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ym.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zd.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sj.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://my.521024.cn


<!-- 参考信息 -->