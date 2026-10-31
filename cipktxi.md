代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://de.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qk.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rr.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tq.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bp.jctech888.com.cn

[K07] 进制转换
来源：http://ci.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nb.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wh.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://no.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://en.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jn.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://in.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yw.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sp.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ae.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://jz.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ba.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://ql.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ti.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ox.shxzskj.cn

Go:   encoding/gob
来源：http://cc.521024.cn

Ruby: Marshal.dump(obj)
来源：http://yi.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ao.bookmarksfly.cn

================================================================================
来源：http://rm.521024.cn

L. 网络请求
来源：http://jw.huanxung.cn

================================================================================
来源：http://ca.hahajie.cn

[L01] 发送 GET 请求
来源：http://eq.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nf.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ar.shxzukj.cn

JS:   await fetch(url)
来源：http://lx.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://re.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://en.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://ba.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cb.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://st.hahajie.cn

[L02] 发送 POST JSON
来源：http://fp.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rw.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://te.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cr.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ej.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oo.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uu.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eg.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jh.szsharing.cn

[L03] 设置自定义请求头
来源：http://se.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ka.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://up.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rb.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gd.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://le.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mx.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nn.lnxyls.cn

[L04] 设置超时
来源：http://nt.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://fw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bc.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dl.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rf.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iy.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gp.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dc.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pe.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://zs.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ff.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://td.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tw.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iq.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nb.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aa.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ib.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://mi.huixiangedu.cn

Py:   resp.json()
来源：http://im.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://tz.szxytkj.cn

JS:   await resp.json()
来源：http://xp.wgjwhj.cn

TS:   await resp.json()
来源：http://lr.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dm.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tb.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://uu.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xo.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://ld.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lk.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://by.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://yk.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://nk.huanxung.cn

Java: resp.statusCode()
来源：http://ri.521024.cn

Go:   resp.StatusCode
来源：http://dz.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://tv.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://hh.panjiajie.cn

[L08] 并发请求多个地址
来源：http://cz.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zp.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://ej.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yd.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vx.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ha.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://se.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sg.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://px.jctech888.com.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://mh.9csxet.cn

================================================================================
来源：http://nc.wgjwhj.cn

[M01] 读取命令行参数
来源：http://pv.szxytkj.cn

Py:   sys.argv[1:]
来源：http://qq.hahajie.cn

PHP:  $argv;  $argc;
来源：http://yf.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://io.nicolike.cn

TS:   process.argv.slice(2)
来源：http://eg.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://sc.huixiangedu.cn

Go:   os.Args[1:]
来源：http://bz.newstarts.cn

Ruby: ARGV
来源：http://ix.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ns.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://pe.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://gq.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ad.9csxet.cn

JS:   process.env.HOME
来源：http://xz.nicolike.cn

TS:   process.env.HOME
来源：http://cw.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://gy.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yv.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ya.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mp.yuexingan06.cn

[M03] 执行外部命令
来源：http://ib.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tv.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dy.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pb.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ue.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hx.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ir.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ai.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://cx.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://sq.shxzukj.cn

Py:   os.getcwd()
来源：http://cb.bjjhwx.cn

PHP:  getcwd();
来源：http://yv.jianghongdianzi.cn

JS:   process.cwd()
来源：http://sy.hnjuh.cn

TS:   process.cwd()
来源：http://px.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://gh.huixiangedu.cn

Go:   os.Getwd()
来源：http://me.huanxung.cn

Ruby: Dir.pwd
来源：http://hr.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ah.yuntaijiaju.cn

[M05] 设置退出码
来源：http://ft.newstarts.cn

Py:   sys.exit(1)
来源：http://ao.szsharing.cn

PHP:  exit(1);
来源：http://si.lnxyls.cn

JS:   process.exit(1)
来源：http://uc.muxihuayi.cn

TS:   process.exit(1)
来源：http://rx.yuexingan06.cn

Java: System.exit(1)
来源：http://yk.shtwfgs.cn

Go:   os.Exit(1)
来源：http://cx.jianghongdianzi.cn

Ruby: exit 1
来源：http://da.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yp.521024.cn

[M06] 向标准错误输出
来源：http://tp.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://qi.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vd.huixiangedu.cn

JS:   console.error("err")
来源：http://px.lnxyls.cn

TS:   console.error("err")
来源：http://ms.haigaiapp.cn

Java: System.err.println("err")
来源：http://rv.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ik.colortex.cn

Ruby: warn "err"
来源：http://xc.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ch.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://lh.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://vr.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nu.9csxet.cn

JS:   require.main === module
来源：http://sc.huanxung.cn

TS:   require.main === module
来源：http://ep.lnxyls.cn

Java: public static void main(String[] args)
来源：http://ko.jctech888.com.cn

Go:   func main()
来源：http://jb.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bv.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://qx.colortex.cn

[M08] 获取系统与运行时信息
来源：http://rn.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://vz.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://pz.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ey.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://ei.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pe.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dt.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bu.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fh.shxzukj.cn

================================================================================
来源：http://hc.wgjwhj.cn

N. 数据结构与算法
来源：http://bl.jctech888.com.cn

================================================================================
来源：http://uv.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://ix.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mq.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zy.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://io.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rk.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mj.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://tl.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ic.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zt.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://fo.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://dx.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uz.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fb.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://au.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ls.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://uj.hnjuh.cn

Ruby: arr.sort
来源：http://qa.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ci.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://fb.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rr.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://pk.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mh.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ux.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ip.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tc.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kq.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://xb.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rf.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zh.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bl.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kn.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xy.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://op.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yf.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hi.hnjuh.cn

[N05] 最大公约数
来源：http://og.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://kt.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dg.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cj.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xc.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://so.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oc.hahajie.cn

Ruby: a.gcd(b)
来源：http://dq.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wf.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://mq.huanxung.cn

Py:   s == s[::-1]
来源：http://rc.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://qt.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://lf.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://fq.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rk.huanxung.cn

Go:   // 双指针从两端比较
来源：http://lq.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://ou.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jy.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://ez.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fd.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aa.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ot.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://zx.asd995.cn

Java: // 手写 HashMap
来源：http://lr.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ya.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://dz.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ge.hnjuh.cn

[N08] 生成全排列
来源：http://uq.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://pv.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://zv.521024.cn

JS:   // 手写回溯递归
来源：http://bt.shxzskj.cn

TS:   // 手写回溯递归
来源：http://kf.nicolike.cn

Java: // 手写回溯递归
来源：http://we.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://zz.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://fc.szsharing.cn

C#:   // 手写回溯递归
来源：http://ku.jctech888.com.cn

[N09] 栈与队列
来源：http://rp.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fv.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mo.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zl.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lx.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nf.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zz.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rl.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ke.huixiangedu.cn

[N10] 链表节点定义
来源：http://pc.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yn.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xo.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ht.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wk.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ds.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sl.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xm.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ze.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://wl.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://su.szxytkj.cn

PHP:  // 手写递归函数
来源：http://pf.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nb.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sn.chemitech.net.cn

Java: // 手写递归
来源：http://ev.yuexingan06.cn

Go:   // 手写递归
来源：http://hr.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pj.gzmigu.cn

C#:   // 手写递归
来源：http://ck.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fm.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://de.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ml.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dc.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cf.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yv.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://af.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jz.nicolike.cn

================================================================================
来源：http://km.gzmigu.cn

O. 并发与异步
来源：http://gu.haigaiapp.cn

================================================================================
来源：http://li.panjiajie.cn

[O01] 启动一个线程
来源：http://zs.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ux.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tb.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://va.shxzskj.cn

TS:   // 同 JS
来源：http://ad.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://fn.asd995.cn

Go:   go f()
来源：http://ky.shxzukj.cn

Ruby: Thread.new { f }
来源：http://ov.szsharing.cn

C#:   Task.Run(() => F());
来源：http://bk.lnxyls.cn

[O02] 使用线程池
来源：http://dk.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ia.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zo.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://ob.newstarts.cn


<!-- 参考信息 -->