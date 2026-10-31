代发 wailian999

[K06] 解析 URL 查询串
来源：http://um.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://da.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ii.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cj.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jo.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ss.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ba.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ka.szsharing.cn

[K07] 进制转换
来源：http://kt.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aj.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gt.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lp.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://im.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rj.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hq.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ov.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rz.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ky.colortex.cn

Py:   pickle.dumps(obj)
来源：http://sn.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pm.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ao.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://oc.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://li.521024.cn

Go:   encoding/gob
来源：http://qx.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://fi.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vs.hahajie.cn

================================================================================
来源：http://nr.newstarts.cn

L. 网络请求
来源：http://qc.jctech888.com.cn

================================================================================
来源：http://es.shxzukj.cn

[L01] 发送 GET 请求
来源：http://py.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ru.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ar.asd995.cn

JS:   await fetch(url)
来源：http://yu.haigaiapp.cn

TS:   await fetch(url)
来源：http://sv.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vj.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://sg.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://if.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sh.nicolike.cn

[L02] 发送 POST JSON
来源：http://cw.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ff.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rv.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jt.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zm.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ej.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ep.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uf.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pf.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://eh.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mi.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aa.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pm.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ge.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cp.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fr.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://er.huanxung.cn

[L04] 设置超时
来源：http://jf.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ul.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vh.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ke.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qr.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bj.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ir.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mt.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fn.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ml.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://od.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qo.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kr.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mm.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zx.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pm.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nm.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ys.nszjky.cn

[L06] 解析响应为 JSON
来源：http://xt.szsharing.cn

Py:   resp.json()
来源：http://yo.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://cq.yuntaijiaju.cn

JS:   await resp.json()
来源：http://hz.nicolike.cn

TS:   await resp.json()
来源：http://ap.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cl.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://ng.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wd.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ne.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mn.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sl.521024.cn

JS:   resp.ok;  resp.status
来源：http://yb.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://gi.panjiajie.cn

Java: resp.statusCode()
来源：http://bs.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ma.szsharing.cn

Ruby: resp.code.to_i
来源：http://sd.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://dx.hahajie.cn

[L08] 并发请求多个地址
来源：http://qf.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ia.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://cu.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://na.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ep.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jc.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://de.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wn.hahajie.cn

================================================================================
来源：http://so.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://iy.wgjwhj.cn

================================================================================
来源：http://du.yuexingan06.cn

[M01] 读取命令行参数
来源：http://iq.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ve.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://cf.nicolike.cn

JS:   process.argv.slice(2)
来源：http://dx.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://vm.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://ma.wgjwhj.cn

Go:   os.Args[1:]
来源：http://ew.huixinmuqiang.cn

Ruby: ARGV
来源：http://wa.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://lz.hnjuh.cn

[M02] 读取环境变量
来源：http://ai.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://xi.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uq.lnxyls.cn

JS:   process.env.HOME
来源：http://gn.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://fl.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://pi.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lr.nicolike.cn

Ruby: ENV["HOME"]
来源：http://xh.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://na.lnxyls.cn

[M03] 执行外部命令
来源：http://va.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qt.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mm.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wl.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aw.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xk.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mu.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tw.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://xp.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://gt.wgjwhj.cn

Py:   os.getcwd()
来源：http://sn.szsharing.cn

PHP:  getcwd();
来源：http://jy.huixiangedu.cn

JS:   process.cwd()
来源：http://lz.wgjwhj.cn

TS:   process.cwd()
来源：http://va.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://vk.shxzukj.cn

Go:   os.Getwd()
来源：http://vp.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://zb.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mg.bookmarksfly.cn

[M05] 设置退出码
来源：http://zx.huanxung.cn

Py:   sys.exit(1)
来源：http://on.szxytkj.cn

PHP:  exit(1);
来源：http://zr.shxzukj.cn

JS:   process.exit(1)
来源：http://ri.nicolike.cn

TS:   process.exit(1)
来源：http://ci.hahajie.cn

Java: System.exit(1)
来源：http://aq.bjjhwx.cn

Go:   os.Exit(1)
来源：http://tz.jctech888.com.cn

Ruby: exit 1
来源：http://og.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lh.hahajie.cn

[M06] 向标准错误输出
来源：http://fj.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://zm.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ii.bjjhwx.cn

JS:   console.error("err")
来源：http://ik.haigaiapp.cn

TS:   console.error("err")
来源：http://qd.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ug.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lk.asd995.cn

Ruby: warn "err"
来源：http://yl.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://fr.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://cf.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://fw.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aw.jctech888.com.cn

JS:   require.main === module
来源：http://lj.huixinmuqiang.cn

TS:   require.main === module
来源：http://te.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://wc.chemitech.net.cn

Go:   func main()
来源：http://ba.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lb.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://go.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://fa.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ur.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://yy.gzmigu.cn

JS:   process.platform;  process.version
来源：http://pl.asd995.cn

TS:   process.platform;  process.version
来源：http://ux.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fo.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bj.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tw.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rc.szsharing.cn

================================================================================
来源：http://mo.panjiajie.cn

N. 数据结构与算法
来源：http://cf.wgjwhj.cn

================================================================================
来源：http://dl.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://ob.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mc.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aw.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jn.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://in.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oi.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://im.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ch.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ni.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kd.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ch.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nr.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ji.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ly.panjiajie.cn

Ruby: arr.sort
来源：http://rp.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ue.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://gd.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fz.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://qn.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zf.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jm.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ep.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qf.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hu.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jn.nicolike.cn

[N04] 斐波那契数列
来源：http://nd.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ay.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zt.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zd.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oc.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ns.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yb.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oz.521024.cn

[N05] 最大公约数
来源：http://cz.nicolike.cn

Py:   math.gcd(a, b)
来源：http://mw.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zp.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://io.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wj.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ne.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tu.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://ft.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yn.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://dy.shxzukj.cn

Py:   s == s[::-1]
来源：http://iw.nszjky.cn

PHP:  $s === strrev($s);
来源：http://oq.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://xp.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://vy.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uw.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://tz.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ri.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zu.asd995.cn

[N07] 两数之和（返回下标）
来源：http://mj.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ew.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ay.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sa.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://zi.colortex.cn

Java: // 手写 HashMap
来源：http://js.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://rp.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://kg.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ox.haigaiapp.cn

[N08] 生成全排列
来源：http://jo.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://sb.9csxet.cn

PHP:  // 手写递归交换
来源：http://eb.szxytkj.cn

JS:   // 手写回溯递归
来源：http://jp.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://it.colortex.cn

Java: // 手写回溯递归
来源：http://yo.szsharing.cn

Go:   // 手写回溯递归
来源：http://jy.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://iv.szsharing.cn

C#:   // 手写回溯递归
来源：http://dv.shtwfgs.cn

[N09] 栈与队列
来源：http://hr.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rz.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jr.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fu.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cx.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vw.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tw.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ke.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oe.szxytkj.cn

[N10] 链表节点定义
来源：http://aw.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rn.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mf.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tw.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mz.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://uh.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bi.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hj.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zn.newstarts.cn

[N11] 二叉树中序遍历
来源：http://xf.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rg.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://aj.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ch.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ma.yuntaijiaju.cn

Java: // 手写递归
来源：http://hc.asd995.cn

Go:   // 手写递归
来源：http://nz.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uk.huixiangedu.cn

C#:   // 手写递归
来源：http://jw.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bc.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ia.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://do.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hm.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mi.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zz.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oa.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fl.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vx.bjjhwx.cn

================================================================================
来源：http://md.9csxet.cn

O. 并发与异步
来源：http://yt.wgjwhj.cn

================================================================================
来源：http://tk.huixiangedu.cn

[O01] 启动一个线程
来源：http://gz.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oc.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pt.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xg.nicolike.cn

TS:   // 同 JS
来源：http://az.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://ac.huanxung.cn

Go:   go f()
来源：http://zu.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://xj.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://ci.bookmarksfly.cn


<!-- 参考信息 -->