代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://ju.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vt.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dj.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lr.newstarts.cn

[K06] 解析 URL 查询串
来源：http://qk.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://or.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kw.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://on.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xs.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pu.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ek.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://go.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vz.nszjky.cn

[K07] 进制转换
来源：http://fk.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jk.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fs.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ju.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mf.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vy.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dv.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pb.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ie.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://fw.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://bx.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ap.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://oh.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ge.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fn.lnxyls.cn

Go:   encoding/gob
来源：http://vn.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://jn.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://el.huixiangedu.cn

================================================================================
来源：http://vq.hnjuh.cn

L. 网络请求
来源：http://tg.chemitech.net.cn

================================================================================
来源：http://bq.nszjky.cn

[L01] 发送 GET 请求
来源：http://yn.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gz.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rw.hahajie.cn

JS:   await fetch(url)
来源：http://md.newstarts.cn

TS:   await fetch(url)
来源：http://ha.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gk.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://ru.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ic.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://do.colortex.cn

[L02] 发送 POST JSON
来源：http://cw.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cb.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ry.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jk.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kr.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lo.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zp.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://la.hahajie.cn

[L03] 设置自定义请求头
来源：http://rp.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yg.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dp.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mh.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zv.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ac.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gq.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ew.jctech888.com.cn

[L04] 设置超时
来源：http://ou.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://jb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ew.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gi.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://az.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zh.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kp.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xq.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bo.nicolike.cn

[L05] 上传文件（multipart）
来源：http://ie.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gt.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tk.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sl.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uk.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tg.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://is.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ra.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qk.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://gr.nicolike.cn

Py:   resp.json()
来源：http://ji.huanxung.cn

PHP:  json_decode($body, true);
来源：http://mk.newstarts.cn

JS:   await resp.json()
来源：http://op.shxzukj.cn

TS:   await resp.json()
来源：http://ln.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nu.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ov.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dd.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://mm.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ht.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hs.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://wq.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://kj.hnjuh.cn

Java: resp.statusCode()
来源：http://tp.nicolike.cn

Go:   resp.StatusCode
来源：http://rt.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://rb.521024.cn

C#:   (int)resp.StatusCode
来源：http://xh.panjiajie.cn

[L08] 并发请求多个地址
来源：http://bf.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wq.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://fm.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ep.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gb.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ee.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yt.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ag.521024.cn

================================================================================
来源：http://xf.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://ys.jianghongdianzi.cn

================================================================================
来源：http://lq.shxzukj.cn

[M01] 读取命令行参数
来源：http://qy.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://um.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://rx.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://zj.hahajie.cn

TS:   process.argv.slice(2)
来源：http://qv.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://eb.huanxung.cn

Go:   os.Args[1:]
来源：http://ub.lnxyls.cn

Ruby: ARGV
来源：http://vi.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ca.asd995.cn

[M02] 读取环境变量
来源：http://dw.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://ut.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wh.newstarts.cn

JS:   process.env.HOME
来源：http://ey.hnjuh.cn

TS:   process.env.HOME
来源：http://vj.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://rd.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sb.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://uk.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bc.bjjhwx.cn

[M03] 执行外部命令
来源：http://wm.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rf.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ww.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ph.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oo.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qt.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oa.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hj.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://ew.panjiajie.cn

[M04] 获取当前工作目录
来源：http://xj.newstarts.cn

Py:   os.getcwd()
来源：http://kn.chemitech.net.cn

PHP:  getcwd();
来源：http://tb.521024.cn

JS:   process.cwd()
来源：http://bk.shtwfgs.cn

TS:   process.cwd()
来源：http://mh.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://wo.9csxet.cn

Go:   os.Getwd()
来源：http://ow.9csxet.cn

Ruby: Dir.pwd
来源：http://at.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eo.shtwfgs.cn

[M05] 设置退出码
来源：http://gc.haigaiapp.cn

Py:   sys.exit(1)
来源：http://dy.shxzskj.cn

PHP:  exit(1);
来源：http://hx.bookmarksfly.cn

JS:   process.exit(1)
来源：http://cs.nicolike.cn

TS:   process.exit(1)
来源：http://xt.yuexingan06.cn

Java: System.exit(1)
来源：http://nr.nicolike.cn

Go:   os.Exit(1)
来源：http://hz.newstarts.cn

Ruby: exit 1
来源：http://pc.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ev.nicolike.cn

[M06] 向标准错误输出
来源：http://nl.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://sd.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rz.chemitech.net.cn

JS:   console.error("err")
来源：http://pp.9csxet.cn

TS:   console.error("err")
来源：http://te.nszjky.cn

Java: System.err.println("err")
来源：http://ew.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nb.huixinmuqiang.cn

Ruby: warn "err"
来源：http://ce.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://gp.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://qx.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://zz.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://el.shxzukj.cn

JS:   require.main === module
来源：http://we.gzmigu.cn

TS:   require.main === module
来源：http://jy.hahajie.cn

Java: public static void main(String[] args)
来源：http://gm.hnjuh.cn

Go:   func main()
来源：http://fd.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wq.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://xl.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://rj.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ow.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://qn.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://rn.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://li.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ey.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bb.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wg.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ay.panjiajie.cn

================================================================================
来源：http://pv.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ly.muxihuayi.cn

================================================================================
来源：http://bz.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://ja.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ta.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ul.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vz.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yg.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ty.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://kz.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lk.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fb.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://mk.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ej.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yf.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ag.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zq.huanxung.cn

Go:   slices.Sort(arr)
来源：http://su.shtwfgs.cn

Ruby: arr.sort
来源：http://ba.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dd.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://bd.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vk.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://fs.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://te.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uj.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ya.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qf.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ae.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://vq.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zd.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ff.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sw.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nu.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fm.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jt.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kw.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iq.gzmigu.cn

[N05] 最大公约数
来源：http://tu.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ay.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://va.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tb.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zd.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://if.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gj.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://rp.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ip.bjjhwx.cn

[N06] 判断回文字符串
来源：http://qi.nicolike.cn

Py:   s == s[::-1]
来源：http://cu.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://us.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://cj.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://dv.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ug.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://nf.huixiangedu.cn

Ruby: s == s.reverse
来源：http://eu.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ph.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://nz.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iv.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ou.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://le.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://te.haigaiapp.cn

Java: // 手写 HashMap
来源：http://ye.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://dz.shxzukj.cn

Ruby: // 手写 Hash
来源：http://he.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wt.gzmigu.cn

[N08] 生成全排列
来源：http://bt.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://aj.shxzukj.cn

PHP:  // 手写递归交换
来源：http://cd.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://nu.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://co.521024.cn

Java: // 手写回溯递归
来源：http://ml.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://di.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://ni.asd995.cn

C#:   // 手写回溯递归
来源：http://bk.huixiangedu.cn

[N09] 栈与队列
来源：http://ob.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eo.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fr.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kx.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jw.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xi.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qi.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vv.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uq.yuexingan06.cn

[N10] 链表节点定义
来源：http://tj.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gc.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ch.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://po.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jh.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://qp.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://au.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rk.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jq.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://fh.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fx.hahajie.cn

PHP:  // 手写递归函数
来源：http://db.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bn.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.gzmigu.cn

Java: // 手写递归
来源：http://vq.bjjhwx.cn

Go:   // 手写递归
来源：http://mh.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fd.nszjky.cn

C#:   // 手写递归
来源：http://tp.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zx.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lf.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tl.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gp.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zu.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ds.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iy.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mi.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cm.wgjwhj.cn

================================================================================
来源：http://zm.shxzukj.cn

O. 并发与异步
来源：http://gq.9csxet.cn

================================================================================
来源：http://bu.nszjky.cn

[O01] 启动一个线程
来源：http://tp.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mt.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ep.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ou.hahajie.cn

TS:   // 同 JS
来源：http://bb.shxzskj.cn


<!-- 参考信息 -->