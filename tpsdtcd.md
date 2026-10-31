代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://iz.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://wo.hahajie.cn

JS:   structuredClone(obj)
来源：http://ni.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://vj.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ia.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ha.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bl.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://io.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ak.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uy.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://og.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xw.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zf.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://we.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vz.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://da.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tn.szsharing.cn

[K07] 进制转换
来源：http://ct.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rr.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://os.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sg.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dj.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rn.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qf.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iu.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hp.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://ae.colortex.cn

Py:   pickle.dumps(obj)
来源：http://ju.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tb.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://tf.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://ov.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vk.muxihuayi.cn

Go:   encoding/gob
来源：http://dy.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://kg.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cm.colortex.cn

================================================================================
来源：http://np.shxzukj.cn

L. 网络请求
来源：http://ka.chemitech.net.cn

================================================================================
来源：http://cs.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://jw.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nn.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://af.shxzskj.cn

JS:   await fetch(url)
来源：http://sm.szxytkj.cn

TS:   await fetch(url)
来源：http://xq.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ky.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://wu.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://to.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sh.shxzukj.cn

[L02] 发送 POST JSON
来源：http://zm.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ra.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xs.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gw.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lo.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bg.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oa.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qm.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://im.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://qg.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nh.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oy.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bf.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://da.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qa.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sl.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qk.yuntaijiaju.cn

[L04] 设置超时
来源：http://xm.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://wv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hs.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://by.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mq.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xe.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ei.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yk.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://si.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://tw.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wv.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jz.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://il.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zg.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hm.521024.cn

[L06] 解析响应为 JSON
来源：http://vj.huanxung.cn

Py:   resp.json()
来源：http://bq.huanxung.cn

PHP:  json_decode($body, true);
来源：http://pu.bookmarksfly.cn

JS:   await resp.json()
来源：http://rg.chemitech.net.cn

TS:   await resp.json()
来源：http://te.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://al.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qx.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://nt.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zh.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://pn.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ld.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yp.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ug.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://ii.bookmarksfly.cn

Java: resp.statusCode()
来源：http://fl.huanxung.cn

Go:   resp.StatusCode
来源：http://gd.521024.cn

Ruby: resp.code.to_i
来源：http://lf.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://cb.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://jy.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cv.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://bm.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nn.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cq.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lr.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xx.huanxung.cn

================================================================================
来源：http://nc.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://jj.chemitech.net.cn

================================================================================
来源：http://zw.hahajie.cn

[M01] 读取命令行参数
来源：http://fz.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://ae.hahajie.cn

PHP:  $argv;  $argc;
来源：http://nj.nicolike.cn

JS:   process.argv.slice(2)
来源：http://tj.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://ea.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://er.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ds.yuexingan06.cn

Ruby: ARGV
来源：http://cr.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://px.haigaiapp.cn

[M02] 读取环境变量
来源：http://wh.521024.cn

Py:   os.environ.get("HOME")
来源：http://lv.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ki.bjjhwx.cn

JS:   process.env.HOME
来源：http://kd.shxzukj.cn

TS:   process.env.HOME
来源：http://km.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://qy.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://lz.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hj.wgjwhj.cn

[M03] 执行外部命令
来源：http://zo.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vh.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://or.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tn.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qh.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lh.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qe.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://np.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://fl.shxzukj.cn

Py:   os.getcwd()
来源：http://bl.yuexingan06.cn

PHP:  getcwd();
来源：http://hu.jctech888.com.cn

JS:   process.cwd()
来源：http://pq.yuexingan06.cn

TS:   process.cwd()
来源：http://ii.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ip.jctech888.com.cn

Go:   os.Getwd()
来源：http://qz.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://fx.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xv.bookmarksfly.cn

[M05] 设置退出码
来源：http://lv.huixiangedu.cn

Py:   sys.exit(1)
来源：http://ig.asd995.cn

PHP:  exit(1);
来源：http://vb.nszjky.cn

JS:   process.exit(1)
来源：http://hw.lnxyls.cn

TS:   process.exit(1)
来源：http://wl.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ad.muxihuayi.cn

Go:   os.Exit(1)
来源：http://me.hnjuh.cn

Ruby: exit 1
来源：http://gz.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qx.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://do.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://wv.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ev.colortex.cn

JS:   console.error("err")
来源：http://zb.jianghongdianzi.cn

TS:   console.error("err")
来源：http://cv.jctech888.com.cn

Java: System.err.println("err")
来源：http://yu.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dr.bjjhwx.cn

Ruby: warn "err"
来源：http://jx.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://yb.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://ia.asd995.cn

Py:   if __name__ == "__main__":
来源：http://kl.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gi.lnxyls.cn

JS:   require.main === module
来源：http://vj.gzmigu.cn

TS:   require.main === module
来源：http://ta.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ae.yuntaijiaju.cn

Go:   func main()
来源：http://bx.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://du.9csxet.cn

C#:   static void Main(string[] args)
来源：http://vn.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://fr.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://sd.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://rg.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://xg.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://mh.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yg.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zt.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ez.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ej.colortex.cn

================================================================================
来源：http://to.nszjky.cn

N. 数据结构与算法
来源：http://uu.bookmarksfly.cn

================================================================================
来源：http://vm.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://rs.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ob.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://al.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mr.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jl.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bm.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://gc.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nw.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ie.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ep.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://qu.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kh.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gv.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ng.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pg.521024.cn

Go:   slices.Sort(arr)
来源：http://zn.jctech888.com.cn

Ruby: arr.sort
来源：http://gb.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xd.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ve.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ac.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://mc.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aj.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rw.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gl.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yz.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pq.huanxung.cn

[N04] 斐波那契数列
来源：http://gc.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rq.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tg.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jr.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ld.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://np.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jc.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ky.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hu.huixinmuqiang.cn

[N05] 最大公约数
来源：http://py.nszjky.cn

Py:   math.gcd(a, b)
来源：http://xk.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bl.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://db.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://za.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://re.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yk.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://yo.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ei.gzmigu.cn

[N06] 判断回文字符串
来源：http://il.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ql.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://rs.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://rn.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://ce.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xu.szsharing.cn

Go:   // 双指针从两端比较
来源：http://se.chemitech.net.cn

Ruby: s == s.reverse
来源：http://up.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yw.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://pn.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pq.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bj.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gd.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://xc.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://gk.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://mx.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://ul.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://st.yuexingan06.cn

[N08] 生成全排列
来源：http://io.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://yh.asd995.cn

PHP:  // 手写递归交换
来源：http://bg.shxzukj.cn

JS:   // 手写回溯递归
来源：http://lq.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://bp.panjiajie.cn

Java: // 手写回溯递归
来源：http://co.huanxung.cn

Go:   // 手写回溯递归
来源：http://ii.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://us.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://ya.nicolike.cn

[N09] 栈与队列
来源：http://yw.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xn.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ma.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://on.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xr.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tq.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rc.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dc.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.shxzskj.cn

[N10] 链表节点定义
来源：http://xu.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cq.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pa.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oq.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kj.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://gt.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://if.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ju.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iw.colortex.cn

[N11] 二叉树中序遍历
来源：http://ta.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://re.shxzskj.cn

PHP:  // 手写递归函数
来源：http://hq.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yf.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mr.colortex.cn

Java: // 手写递归
来源：http://gi.szsharing.cn

Go:   // 手写递归
来源：http://qu.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tp.bjjhwx.cn

C#:   // 手写递归
来源：http://lx.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pw.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rr.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yn.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oa.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wc.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zp.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xa.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uq.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vm.huixinmuqiang.cn

================================================================================
来源：http://vu.9csxet.cn

O. 并发与异步
来源：http://er.panjiajie.cn

================================================================================
来源：http://ak.nicolike.cn

[O01] 启动一个线程
来源：http://vt.haigaiapp.cn


<!-- 参考信息 -->