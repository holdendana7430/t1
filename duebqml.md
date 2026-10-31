代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ba.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://uh.9csxet.cn

JS:   structuredClone(obj)
来源：http://tw.asd995.cn

TS:   structuredClone(obj)
来源：http://ga.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zo.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://do.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ip.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hc.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ah.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ro.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qh.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lx.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zh.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yi.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ho.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bt.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kl.521024.cn

[K07] 进制转换
来源：http://mx.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kl.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lw.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ey.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://du.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qq.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cr.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eh.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://af.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://za.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://gh.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bf.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://if.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://qq.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.chemitech.net.cn

Go:   encoding/gob
来源：http://kx.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://fz.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hw.lnxyls.cn

================================================================================
来源：http://hv.9csxet.cn

L. 网络请求
来源：http://fk.shxzukj.cn

================================================================================
来源：http://up.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ip.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qq.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pq.szxytkj.cn

JS:   await fetch(url)
来源：http://ht.yuexingan06.cn

TS:   await fetch(url)
来源：http://nj.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://js.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://sh.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ef.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qt.szsharing.cn

[L02] 发送 POST JSON
来源：http://hq.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zr.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://os.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kc.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oy.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xv.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jz.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ax.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tv.9csxet.cn

[L03] 设置自定义请求头
来源：http://cv.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hf.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tg.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yn.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ki.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vr.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fj.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ej.chemitech.net.cn

[L04] 设置超时
来源：http://py.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://yr.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tn.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qj.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nc.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ui.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qq.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tq.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ii.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ja.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sn.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zo.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xt.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dy.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://np.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iu.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cf.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ne.colortex.cn

[L06] 解析响应为 JSON
来源：http://dw.521024.cn

Py:   resp.json()
来源：http://kr.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://nf.bookmarksfly.cn

JS:   await resp.json()
来源：http://sk.9csxet.cn

TS:   await resp.json()
来源：http://wz.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hg.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pf.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://ia.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cc.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://pw.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ht.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ru.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://dw.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://aa.asd995.cn

Java: resp.statusCode()
来源：http://nt.yuexingan06.cn

Go:   resp.StatusCode
来源：http://cx.shxzskj.cn

Ruby: resp.code.to_i
来源：http://bb.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://bj.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://qr.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ma.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://zc.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vq.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vx.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aa.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://no.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gh.9csxet.cn

================================================================================
来源：http://sa.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://yj.bjjhwx.cn

================================================================================
来源：http://pl.shxzukj.cn

[M01] 读取命令行参数
来源：http://sg.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://si.newstarts.cn

PHP:  $argv;  $argc;
来源：http://zp.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://ix.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://mh.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://go.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://zb.yuntaijiaju.cn

Ruby: ARGV
来源：http://kp.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://ze.shxzukj.cn

[M02] 读取环境变量
来源：http://iv.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://uh.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ar.shxzukj.cn

JS:   process.env.HOME
来源：http://ue.chemitech.net.cn

TS:   process.env.HOME
来源：http://zm.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://bb.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xl.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://jk.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rn.jctech888.com.cn

[M03] 执行外部命令
来源：http://wy.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vq.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ed.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://st.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uh.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pf.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bf.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qr.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://gb.panjiajie.cn

[M04] 获取当前工作目录
来源：http://km.szxytkj.cn

Py:   os.getcwd()
来源：http://ga.huanxung.cn

PHP:  getcwd();
来源：http://ig.shxzukj.cn

JS:   process.cwd()
来源：http://mk.yuexingan06.cn

TS:   process.cwd()
来源：http://vm.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ln.colortex.cn

Go:   os.Getwd()
来源：http://mw.9csxet.cn

Ruby: Dir.pwd
来源：http://bd.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kf.jianghongdianzi.cn

[M05] 设置退出码
来源：http://lk.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://jo.bjjhwx.cn

PHP:  exit(1);
来源：http://fo.panjiajie.cn

JS:   process.exit(1)
来源：http://uj.chemitech.net.cn

TS:   process.exit(1)
来源：http://pj.yuexingan06.cn

Java: System.exit(1)
来源：http://ba.asd995.cn

Go:   os.Exit(1)
来源：http://vz.hnjuh.cn

Ruby: exit 1
来源：http://ky.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ve.yuexingan06.cn

[M06] 向标准错误输出
来源：http://pw.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://ag.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ki.asd995.cn

JS:   console.error("err")
来源：http://ds.huixiangedu.cn

TS:   console.error("err")
来源：http://om.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://rp.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ys.huanxung.cn

Ruby: warn "err"
来源：http://bi.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://rw.hahajie.cn

[M07] 判断是否为主入口
来源：http://bk.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://nt.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://na.bjjhwx.cn

JS:   require.main === module
来源：http://kf.bookmarksfly.cn

TS:   require.main === module
来源：http://qe.shxzskj.cn

Java: public static void main(String[] args)
来源：http://se.szxytkj.cn

Go:   func main()
来源：http://qk.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://db.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://az.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://tq.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ta.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://la.panjiajie.cn

JS:   process.platform;  process.version
来源：http://hd.hnjuh.cn

TS:   process.platform;  process.version
来源：http://al.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bo.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xl.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://by.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ds.9csxet.cn

================================================================================
来源：http://am.newstarts.cn

N. 数据结构与算法
来源：http://xl.newstarts.cn

================================================================================
来源：http://xl.asd995.cn

[N01] 二分查找（有序数组）
来源：http://bc.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ud.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eu.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nz.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hs.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ti.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://xe.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sk.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://py.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://iw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://nw.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fx.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vs.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xl.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dw.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://fc.shxzukj.cn

Ruby: arr.sort
来源：http://zz.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qb.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://mx.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rq.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://ye.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nf.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cf.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ym.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qp.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qw.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hf.nicolike.cn

[N04] 斐波那契数列
来源：http://st.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ho.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dl.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qh.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://go.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lx.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pr.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jl.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://la.huanxung.cn

[N05] 最大公约数
来源：http://gz.newstarts.cn

Py:   math.gcd(a, b)
来源：http://gk.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fn.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kf.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ja.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lw.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ka.szxytkj.cn

Ruby: a.gcd(b)
来源：http://ba.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mb.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://iz.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://yw.newstarts.cn

PHP:  $s === strrev($s);
来源：http://ue.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://hk.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://zj.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cl.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://kb.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://us.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qh.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://pc.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://my.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vo.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rr.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://kz.521024.cn

Java: // 手写 HashMap
来源：http://et.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://zx.nicolike.cn

Ruby: // 手写 Hash
来源：http://wf.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bl.jctech888.com.cn

[N08] 生成全排列
来源：http://gd.521024.cn

Py:   itertools.permutations(arr)
来源：http://es.asd995.cn

PHP:  // 手写递归交换
来源：http://om.newstarts.cn

JS:   // 手写回溯递归
来源：http://ti.szxytkj.cn

TS:   // 手写回溯递归
来源：http://pl.lnxyls.cn

Java: // 手写回溯递归
来源：http://oq.huanxung.cn

Go:   // 手写回溯递归
来源：http://pk.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://pc.colortex.cn

C#:   // 手写回溯递归
来源：http://qm.asd995.cn

[N09] 栈与队列
来源：http://jf.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lh.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kq.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fk.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bl.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lw.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cv.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mt.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cm.521024.cn

[N10] 链表节点定义
来源：http://vn.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sv.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ay.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zi.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qr.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://id.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jq.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zh.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wi.asd995.cn

[N11] 二叉树中序遍历
来源：http://ef.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ae.hnjuh.cn

PHP:  // 手写递归函数
来源：http://jr.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pt.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hh.bookmarksfly.cn

Java: // 手写递归
来源：http://rl.gzmigu.cn

Go:   // 手写递归
来源：http://oh.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hx.yuntaijiaju.cn

C#:   // 手写递归
来源：http://lj.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yr.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fg.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zp.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rk.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hh.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ip.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://li.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sj.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lu.shxzukj.cn

================================================================================
来源：http://sg.muxihuayi.cn

O. 并发与异步
来源：http://iu.nicolike.cn

================================================================================
来源：http://ot.chemitech.net.cn

[O01] 启动一个线程
来源：http://zt.huixiangedu.cn


<!-- 参考信息 -->