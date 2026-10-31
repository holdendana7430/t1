代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qs.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jj.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xa.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lm.muxihuayi.cn

[K07] 进制转换
来源：http://el.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kq.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qn.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qv.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rs.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pj.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yn.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mx.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sq.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://cf.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://on.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dl.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://uq.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://gx.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ns.521024.cn

Go:   encoding/gob
来源：http://qb.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://pf.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ng.jctech888.com.cn

================================================================================
来源：http://ty.lnxyls.cn

L. 网络请求
来源：http://wn.panjiajie.cn

================================================================================
来源：http://zp.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://az.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cp.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gl.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://uo.shxzskj.cn

TS:   await fetch(url)
来源：http://aj.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jy.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://bq.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sm.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nm.521024.cn

[L02] 发送 POST JSON
来源：http://na.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://db.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dh.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qt.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oj.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bw.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tg.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hh.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wn.nicolike.cn

[L03] 设置自定义请求头
来源：http://dg.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qq.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jo.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://px.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zh.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ga.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jz.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://du.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hm.yuexingan06.cn

[L04] 设置超时
来源：http://pw.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ya.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jp.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uo.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dn.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://df.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uw.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://um.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://kx.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nx.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ez.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cv.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rp.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ys.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oa.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://io.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ba.hahajie.cn

[L06] 解析响应为 JSON
来源：http://gf.panjiajie.cn

Py:   resp.json()
来源：http://eb.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ha.yuexingan06.cn

JS:   await resp.json()
来源：http://fs.yuntaijiaju.cn

TS:   await resp.json()
来源：http://cs.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ac.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pm.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://cx.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ap.521024.cn

[L07] 处理 HTTP 状态码
来源：http://sk.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cr.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ip.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://wr.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://gz.521024.cn

Java: resp.statusCode()
来源：http://pb.lnxyls.cn

Go:   resp.StatusCode
来源：http://ns.hnjuh.cn

Ruby: resp.code.to_i
来源：http://kb.521024.cn

C#:   (int)resp.StatusCode
来源：http://jw.gzmigu.cn

[L08] 并发请求多个地址
来源：http://zg.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ke.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://uk.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vn.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aj.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cz.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gy.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://me.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dz.nszjky.cn

================================================================================
来源：http://oe.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ao.muxihuayi.cn

================================================================================
来源：http://cu.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://jy.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ik.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ef.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://cg.9csxet.cn

TS:   process.argv.slice(2)
来源：http://ab.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://ic.newstarts.cn

Go:   os.Args[1:]
来源：http://fu.jctech888.com.cn

Ruby: ARGV
来源：http://sn.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://wm.shxzukj.cn

[M02] 读取环境变量
来源：http://so.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://oh.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://un.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://lw.nicolike.cn

TS:   process.env.HOME
来源：http://kx.huanxung.cn

Java: System.getenv("HOME")
来源：http://hw.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ra.nicolike.cn

Ruby: ENV["HOME"]
来源：http://vb.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://do.9csxet.cn

[M03] 执行外部命令
来源：http://xo.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tx.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rg.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sp.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dc.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ec.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jw.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://un.colortex.cn

[M04] 获取当前工作目录
来源：http://qh.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://wd.9csxet.cn

PHP:  getcwd();
来源：http://mf.jianghongdianzi.cn

JS:   process.cwd()
来源：http://pt.panjiajie.cn

TS:   process.cwd()
来源：http://pg.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://kd.9csxet.cn

Go:   os.Getwd()
来源：http://hj.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://gx.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qt.colortex.cn

[M05] 设置退出码
来源：http://en.lnxyls.cn

Py:   sys.exit(1)
来源：http://kf.shxzskj.cn

PHP:  exit(1);
来源：http://jx.nszjky.cn

JS:   process.exit(1)
来源：http://xn.szsharing.cn

TS:   process.exit(1)
来源：http://kz.shxzskj.cn

Java: System.exit(1)
来源：http://fc.lnxyls.cn

Go:   os.Exit(1)
来源：http://ya.bookmarksfly.cn

Ruby: exit 1
来源：http://rk.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ra.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ch.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://gf.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xd.huanxung.cn

JS:   console.error("err")
来源：http://qi.haigaiapp.cn

TS:   console.error("err")
来源：http://jz.nicolike.cn

Java: System.err.println("err")
来源：http://ag.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dt.jianghongdianzi.cn

Ruby: warn "err"
来源：http://ef.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://sv.hnjuh.cn

[M07] 判断是否为主入口
来源：http://uy.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://aa.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ib.shxzskj.cn

JS:   require.main === module
来源：http://fo.panjiajie.cn

TS:   require.main === module
来源：http://le.hahajie.cn

Java: public static void main(String[] args)
来源：http://ds.yuexingan06.cn

Go:   func main()
来源：http://vl.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ug.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://on.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://rd.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://xj.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://yl.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://bs.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://ap.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wm.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ew.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fy.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pe.shxzskj.cn

================================================================================
来源：http://ha.yuexingan06.cn

N. 数据结构与算法
来源：http://mm.chemitech.net.cn

================================================================================
来源：http://fs.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://yy.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kd.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dz.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mi.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://no.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://au.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://lh.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://va.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ee.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://yf.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://cz.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wz.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mb.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gu.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://zv.newstarts.cn

Ruby: arr.sort
来源：http://ss.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ym.521024.cn

[N03] 快速排序（分治示例）
来源：http://xw.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://so.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://by.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fq.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ir.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ja.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xv.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nm.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cy.szxytkj.cn

[N04] 斐波那契数列
来源：http://wj.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fm.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pe.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pm.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ta.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jw.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ja.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bn.shxzskj.cn

[N05] 最大公约数
来源：http://jh.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://gk.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rn.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ia.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rx.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sg.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ko.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://oj.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pe.colortex.cn

[N06] 判断回文字符串
来源：http://la.szxytkj.cn

Py:   s == s[::-1]
来源：http://xh.asd995.cn

PHP:  $s === strrev($s);
来源：http://hd.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://yh.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://sw.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wu.colortex.cn

Go:   // 双指针从两端比较
来源：http://yi.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://rs.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cg.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://hp.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lt.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fz.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://oz.shxzukj.cn

Java: // 手写 HashMap
来源：http://mq.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://zo.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://ib.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bc.gzmigu.cn

[N08] 生成全排列
来源：http://fq.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://bs.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://yg.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://ar.huanxung.cn

TS:   // 手写回溯递归
来源：http://vd.nszjky.cn

Java: // 手写回溯递归
来源：http://vg.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://jm.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://dt.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://uf.shxzskj.cn

[N09] 栈与队列
来源：http://st.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pk.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://la.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fj.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ze.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wq.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vu.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sz.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nt.chemitech.net.cn

[N10] 链表节点定义
来源：http://fj.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tf.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://br.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dw.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://st.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://ic.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://up.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cm.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kv.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://cq.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wq.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ky.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nn.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.colortex.cn

Java: // 手写递归
来源：http://ub.colortex.cn

Go:   // 手写递归
来源：http://of.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tg.panjiajie.cn

C#:   // 手写递归
来源：http://rp.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hq.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rv.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hr.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ar.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bc.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mn.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sq.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kp.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ns.haigaiapp.cn

================================================================================
来源：http://yk.shxzskj.cn

O. 并发与异步
来源：http://lg.jianghongdianzi.cn

================================================================================
来源：http://ia.muxihuayi.cn

[O01] 启动一个线程
来源：http://ow.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wo.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ru.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pn.jianghongdianzi.cn

TS:   // 同 JS
来源：http://iu.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://gp.colortex.cn

Go:   go f()
来源：http://hc.shxzskj.cn

Ruby: Thread.new { f }
来源：http://mo.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://uu.nszjky.cn

[O02] 使用线程池
来源：http://zp.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ha.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jl.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://mp.nicolike.cn


<!-- 参考信息 -->