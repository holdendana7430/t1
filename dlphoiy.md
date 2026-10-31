代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gs.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pj.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ew.huixiangedu.cn

[K05] 深拷贝对象
来源：http://nj.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ax.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://qn.nszjky.cn

JS:   structuredClone(obj)
来源：http://wy.hnjuh.cn

TS:   structuredClone(obj)
来源：http://lz.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rm.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gm.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ko.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bn.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://uu.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eg.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zb.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xl.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sn.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ng.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ce.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vz.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iv.lnxyls.cn

[K07] 进制转换
来源：http://up.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ye.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zs.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dn.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qm.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zs.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vb.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sx.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rh.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://va.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://nq.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uu.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ea.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://rm.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ne.jctech888.com.cn

Go:   encoding/gob
来源：http://kv.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://uj.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lz.huixiangedu.cn

================================================================================
来源：http://ba.asd995.cn

L. 网络请求
来源：http://pp.hahajie.cn

================================================================================
来源：http://of.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://by.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://li.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bi.hahajie.cn

JS:   await fetch(url)
来源：http://uh.huixiangedu.cn

TS:   await fetch(url)
来源：http://wd.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oi.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://kr.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uf.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jn.nszjky.cn

[L02] 发送 POST JSON
来源：http://hh.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://le.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rg.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wz.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sn.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cg.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hx.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://of.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ik.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://di.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yv.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oq.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lg.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kl.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ue.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ip.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://if.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xd.yuexingan06.cn

[L04] 设置超时
来源：http://sj.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://kk.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ud.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sr.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://is.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gq.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sj.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bk.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://yj.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kq.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ky.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pd.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ff.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ti.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vi.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zx.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://wo.shxzskj.cn

Py:   resp.json()
来源：http://mr.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://fh.huanxung.cn

JS:   await resp.json()
来源：http://ea.gzmigu.cn

TS:   await resp.json()
来源：http://lw.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bx.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nu.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://my.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fn.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://cw.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bp.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sy.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ww.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://at.panjiajie.cn

Java: resp.statusCode()
来源：http://kc.shtwfgs.cn

Go:   resp.StatusCode
来源：http://rs.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://lt.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://zt.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ek.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ii.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://xh.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rn.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ug.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qy.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wv.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pd.szxytkj.cn

================================================================================
来源：http://yh.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://pi.shtwfgs.cn

================================================================================
来源：http://cw.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://kn.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://cc.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://pa.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://as.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://rz.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://tk.9csxet.cn

Go:   os.Args[1:]
来源：http://yz.asd995.cn

Ruby: ARGV
来源：http://wa.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://nw.chemitech.net.cn

[M02] 读取环境变量
来源：http://hf.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ol.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rr.nicolike.cn

JS:   process.env.HOME
来源：http://uk.colortex.cn

TS:   process.env.HOME
来源：http://me.shxzskj.cn

Java: System.getenv("HOME")
来源：http://pp.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gw.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://cm.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uo.szsharing.cn

[M03] 执行外部命令
来源：http://ar.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ql.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yq.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://li.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mo.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vt.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://am.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pd.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://we.szxytkj.cn

[M04] 获取当前工作目录
来源：http://cb.haigaiapp.cn

Py:   os.getcwd()
来源：http://hh.colortex.cn

PHP:  getcwd();
来源：http://aw.yuexingan06.cn

JS:   process.cwd()
来源：http://kl.shtwfgs.cn

TS:   process.cwd()
来源：http://qk.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ku.szsharing.cn

Go:   os.Getwd()
来源：http://em.521024.cn

Ruby: Dir.pwd
来源：http://um.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://da.hnjuh.cn

[M05] 设置退出码
来源：http://bu.huanxung.cn

Py:   sys.exit(1)
来源：http://ru.nicolike.cn

PHP:  exit(1);
来源：http://gl.wgjwhj.cn

JS:   process.exit(1)
来源：http://kf.huixiangedu.cn

TS:   process.exit(1)
来源：http://sz.chemitech.net.cn

Java: System.exit(1)
来源：http://af.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://xv.jianghongdianzi.cn

Ruby: exit 1
来源：http://rf.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dg.521024.cn

[M06] 向标准错误输出
来源：http://ps.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://ep.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rb.szsharing.cn

JS:   console.error("err")
来源：http://mt.panjiajie.cn

TS:   console.error("err")
来源：http://da.asd995.cn

Java: System.err.println("err")
来源：http://rw.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ty.yuexingan06.cn

Ruby: warn "err"
来源：http://lc.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://jw.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://xz.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://cm.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ot.huanxung.cn

JS:   require.main === module
来源：http://ta.bookmarksfly.cn

TS:   require.main === module
来源：http://rp.panjiajie.cn

Java: public static void main(String[] args)
来源：http://xx.shxzukj.cn

Go:   func main()
来源：http://cp.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vj.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://bz.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://hc.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://pz.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://nc.panjiajie.cn

JS:   process.platform;  process.version
来源：http://dm.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://xw.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ow.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nm.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sz.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://us.haigaiapp.cn

================================================================================
来源：http://lt.chemitech.net.cn

N. 数据结构与算法
来源：http://ls.lnxyls.cn

================================================================================
来源：http://zj.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://gf.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gp.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kj.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ay.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kc.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kf.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://zf.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pm.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ri.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://th.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://mc.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rb.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mo.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pn.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ti.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://oy.panjiajie.cn

Ruby: arr.sort
来源：http://fa.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pi.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://nk.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wx.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://ux.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lg.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bq.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fg.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xg.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://py.bjjhwx.cn

[N04] 斐波那契数列
来源：http://fs.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pa.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ux.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wm.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gu.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ny.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hm.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://du.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nj.szxytkj.cn

[N05] 最大公约数
来源：http://yp.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ke.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uy.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ul.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lh.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eb.9csxet.cn

Ruby: a.gcd(b)
来源：http://vd.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://im.szxytkj.cn

[N06] 判断回文字符串
来源：http://ju.huanxung.cn

Py:   s == s[::-1]
来源：http://lf.521024.cn

PHP:  $s === strrev($s);
来源：http://gv.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://dp.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://zy.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tw.colortex.cn

Go:   // 双指针从两端比较
来源：http://eq.huixiangedu.cn

Ruby: s == s.reverse
来源：http://xw.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fp.asd995.cn

[N07] 两数之和（返回下标）
来源：http://vr.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://it.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ex.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rl.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://dd.nszjky.cn

Java: // 手写 HashMap
来源：http://wu.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ge.hahajie.cn

Ruby: // 手写 Hash
来源：http://sd.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uj.bookmarksfly.cn

[N08] 生成全排列
来源：http://wl.asd995.cn

Py:   itertools.permutations(arr)
来源：http://hq.newstarts.cn

PHP:  // 手写递归交换
来源：http://ht.nszjky.cn

JS:   // 手写回溯递归
来源：http://dg.nicolike.cn

TS:   // 手写回溯递归
来源：http://rt.wgjwhj.cn

Java: // 手写回溯递归
来源：http://gg.shxzukj.cn

Go:   // 手写回溯递归
来源：http://sa.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://sh.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://nv.lnxyls.cn

[N09] 栈与队列
来源：http://oj.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lv.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bo.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ph.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gq.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tj.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xr.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pq.newstarts.cn

[N10] 链表节点定义
来源：http://bi.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lx.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://as.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lu.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kj.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://yj.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tw.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ky.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ux.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://de.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cp.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://yk.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cg.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vw.hahajie.cn

Java: // 手写递归
来源：http://tc.chemitech.net.cn

Go:   // 手写递归
来源：http://yi.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lv.panjiajie.cn

C#:   // 手写递归
来源：http://jg.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jy.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ks.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sq.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qg.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tu.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nv.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pu.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://om.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zy.521024.cn


<!-- 参考信息 -->