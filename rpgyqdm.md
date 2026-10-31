代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fr.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://co.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dh.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xg.nszjky.cn

[K07] 进制转换
来源：http://kb.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ht.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://on.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rm.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://db.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qf.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pq.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pd.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kb.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://vq.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://fw.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ny.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://nm.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ml.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kd.huixinmuqiang.cn

Go:   encoding/gob
来源：http://lf.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://jr.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uy.hahajie.cn

================================================================================
来源：http://ib.huanxung.cn

L. 网络请求
来源：http://uy.muxihuayi.cn

================================================================================
来源：http://st.gzmigu.cn

[L01] 发送 GET 请求
来源：http://jk.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ox.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mz.9csxet.cn

JS:   await fetch(url)
来源：http://nh.nszjky.cn

TS:   await fetch(url)
来源：http://mk.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pe.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://xe.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://he.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xr.521024.cn

[L02] 发送 POST JSON
来源：http://ag.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uj.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://go.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ul.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xe.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ms.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sx.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ip.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ei.colortex.cn

[L03] 设置自定义请求头
来源：http://ot.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sy.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jh.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uq.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eb.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://js.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://io.gzmigu.cn

[L04] 设置超时
来源：http://se.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://mj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hh.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wy.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://di.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://al.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fl.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ch.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fk.asd995.cn

[L05] 上传文件（multipart）
来源：http://wl.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rx.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mv.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://td.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ff.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xx.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sw.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zd.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cl.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://iu.bjjhwx.cn

Py:   resp.json()
来源：http://kf.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://cb.9csxet.cn

JS:   await resp.json()
来源：http://of.panjiajie.cn

TS:   await resp.json()
来源：http://xl.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bk.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bz.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ug.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yo.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://mk.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bq.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vv.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://zf.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://hz.panjiajie.cn

Java: resp.statusCode()
来源：http://dn.yuexingan06.cn

Go:   resp.StatusCode
来源：http://oq.nicolike.cn

Ruby: resp.code.to_i
来源：http://vy.colortex.cn

C#:   (int)resp.StatusCode
来源：http://au.shxzukj.cn

[L08] 并发请求多个地址
来源：http://db.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ta.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://sl.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wm.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fq.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nl.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xv.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lf.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ru.nicolike.cn

================================================================================
来源：http://mo.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ea.nicolike.cn

================================================================================
来源：http://ao.shxzukj.cn

[M01] 读取命令行参数
来源：http://dv.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://pm.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://um.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://kk.szsharing.cn

TS:   process.argv.slice(2)
来源：http://zd.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://cj.szsharing.cn

Go:   os.Args[1:]
来源：http://ki.chemitech.net.cn

Ruby: ARGV
来源：http://dx.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://wb.shtwfgs.cn

[M02] 读取环境变量
来源：http://pc.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://qu.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rp.newstarts.cn

JS:   process.env.HOME
来源：http://vy.shxzskj.cn

TS:   process.env.HOME
来源：http://iy.shxzskj.cn

Java: System.getenv("HOME")
来源：http://hz.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ny.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://qd.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dt.huanxung.cn

[M03] 执行外部命令
来源：http://hq.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mj.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zz.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nl.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pe.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dt.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wp.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eo.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://kr.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ik.szxytkj.cn

Py:   os.getcwd()
来源：http://cp.szxytkj.cn

PHP:  getcwd();
来源：http://sy.huixinmuqiang.cn

JS:   process.cwd()
来源：http://gx.huanxung.cn

TS:   process.cwd()
来源：http://ty.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ug.521024.cn

Go:   os.Getwd()
来源：http://qf.huanxung.cn

Ruby: Dir.pwd
来源：http://fz.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ar.huixinmuqiang.cn

[M05] 设置退出码
来源：http://uo.bjjhwx.cn

Py:   sys.exit(1)
来源：http://yx.panjiajie.cn

PHP:  exit(1);
来源：http://rq.panjiajie.cn

JS:   process.exit(1)
来源：http://ks.shxzskj.cn

TS:   process.exit(1)
来源：http://gc.jianghongdianzi.cn

Java: System.exit(1)
来源：http://nv.szsharing.cn

Go:   os.Exit(1)
来源：http://tv.shxzskj.cn

Ruby: exit 1
来源：http://wd.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gd.muxihuayi.cn

[M06] 向标准错误输出
来源：http://gg.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://is.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pi.shxzukj.cn

JS:   console.error("err")
来源：http://of.panjiajie.cn

TS:   console.error("err")
来源：http://ra.bjjhwx.cn

Java: System.err.println("err")
来源：http://gt.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wk.521024.cn

Ruby: warn "err"
来源：http://vt.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://zu.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ri.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://pi.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pj.szsharing.cn

JS:   require.main === module
来源：http://ea.wgjwhj.cn

TS:   require.main === module
来源：http://qi.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://zb.newstarts.cn

Go:   func main()
来源：http://mm.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://se.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://rt.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://uk.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ad.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ub.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://pr.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://mm.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://px.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://se.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ew.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ai.bjjhwx.cn

================================================================================
来源：http://tt.jctech888.com.cn

N. 数据结构与算法
来源：http://kp.hahajie.cn

================================================================================
来源：http://xb.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://qj.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iv.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ks.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vl.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sj.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uh.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://cq.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sd.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://db.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://zz.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ps.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://va.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ps.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mk.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://sz.asd995.cn

Ruby: arr.sort
来源：http://en.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ac.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://pl.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aq.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://pa.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pk.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ay.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ee.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ti.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rb.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rl.lnxyls.cn

[N04] 斐波那契数列
来源：http://wb.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sg.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xk.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ud.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ol.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oq.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ff.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fm.asd995.cn

[N05] 最大公约数
来源：http://xf.asd995.cn

Py:   math.gcd(a, b)
来源：http://by.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xb.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://th.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://le.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bw.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cu.panjiajie.cn

Ruby: a.gcd(b)
来源：http://py.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vz.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ge.panjiajie.cn

Py:   s == s[::-1]
来源：http://zi.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://it.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://gr.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://rc.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xv.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://tj.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://om.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kg.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://dw.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cs.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lk.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sy.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://nm.szsharing.cn

Java: // 手写 HashMap
来源：http://ls.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://hk.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://yc.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wq.muxihuayi.cn

[N08] 生成全排列
来源：http://hr.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://sa.9csxet.cn

PHP:  // 手写递归交换
来源：http://do.nicolike.cn

JS:   // 手写回溯递归
来源：http://nv.szxytkj.cn

TS:   // 手写回溯递归
来源：http://dg.szsharing.cn

Java: // 手写回溯递归
来源：http://ny.szsharing.cn

Go:   // 手写回溯递归
来源：http://ym.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://wp.hahajie.cn

C#:   // 手写回溯递归
来源：http://qt.jianghongdianzi.cn

[N09] 栈与队列
来源：http://wx.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dr.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vd.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yf.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ax.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gc.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ri.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qm.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ot.hnjuh.cn

[N10] 链表节点定义
来源：http://ii.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xa.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jv.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ck.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mm.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://oy.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sn.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bg.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ky.nszjky.cn

[N11] 二叉树中序遍历
来源：http://zy.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ut.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://cu.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://me.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://py.huanxung.cn

Java: // 手写递归
来源：http://ok.9csxet.cn

Go:   // 手写递归
来源：http://og.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xb.jianghongdianzi.cn

C#:   // 手写递归
来源：http://sg.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uu.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tr.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hj.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kk.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cj.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yf.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cg.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yc.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.gzmigu.cn

================================================================================
来源：http://im.newstarts.cn

O. 并发与异步
来源：http://vb.yuexingan06.cn

================================================================================
来源：http://bl.hnjuh.cn

[O01] 启动一个线程
来源：http://aa.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gj.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yb.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fz.shxzskj.cn

TS:   // 同 JS
来源：http://gg.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://di.chemitech.net.cn

Go:   go f()
来源：http://dv.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://gu.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ed.shtwfgs.cn

[O02] 使用线程池
来源：http://hn.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rl.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lp.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://kr.lnxyls.cn


<!-- 参考信息 -->