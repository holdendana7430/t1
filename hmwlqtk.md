代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://gz.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lc.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vh.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xw.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://ig.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yr.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mz.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fs.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lt.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gc.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mm.huixinmuqiang.cn

[K07] 进制转换
来源：http://bg.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ru.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ob.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yd.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vj.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dt.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gc.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ch.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gj.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://wm.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://tn.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nw.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://tg.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://lv.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://on.shxzskj.cn

Go:   encoding/gob
来源：http://zl.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://pw.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qz.huanxung.cn

================================================================================
来源：http://ls.bookmarksfly.cn

L. 网络请求
来源：http://by.szsharing.cn

================================================================================
来源：http://ru.colortex.cn

[L01] 发送 GET 请求
来源：http://cw.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jq.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dp.hahajie.cn

JS:   await fetch(url)
来源：http://ba.bjjhwx.cn

TS:   await fetch(url)
来源：http://lz.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://af.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://xb.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://er.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ch.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://mk.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qh.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mr.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mg.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jd.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iw.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://na.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zf.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xx.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://ln.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fq.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xo.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ts.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zu.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xu.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sr.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fe.shtwfgs.cn

[L04] 设置超时
来源：http://yj.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://fh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ai.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lu.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hr.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zh.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://in.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rz.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xz.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://jn.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fa.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xk.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rc.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://us.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ll.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ga.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://if.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jm.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://cd.jctech888.com.cn

Py:   resp.json()
来源：http://vi.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://yi.jianghongdianzi.cn

JS:   await resp.json()
来源：http://vp.huixinmuqiang.cn

TS:   await resp.json()
来源：http://ej.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kr.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xz.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://uw.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kr.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://ql.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wd.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sr.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://st.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://mp.asd995.cn

Java: resp.statusCode()
来源：http://mq.yuexingan06.cn

Go:   resp.StatusCode
来源：http://qm.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://hj.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://tp.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://xk.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pf.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ue.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jg.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nc.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xp.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ex.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tq.nszjky.cn

================================================================================
来源：http://nl.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://gn.shxzukj.cn

================================================================================
来源：http://bj.colortex.cn

[M01] 读取命令行参数
来源：http://dl.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://zc.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://me.521024.cn

JS:   process.argv.slice(2)
来源：http://gx.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://hg.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://sp.huanxung.cn

Go:   os.Args[1:]
来源：http://cn.hahajie.cn

Ruby: ARGV
来源：http://sa.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://mt.haigaiapp.cn

[M02] 读取环境变量
来源：http://bs.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://rt.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sy.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://iw.nicolike.cn

TS:   process.env.HOME
来源：http://jz.521024.cn

Java: System.getenv("HOME")
来源：http://eg.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xp.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://zl.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ae.nszjky.cn

[M03] 执行外部命令
来源：http://hn.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bi.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zi.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ve.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ah.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://at.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://an.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fu.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://nj.asd995.cn

[M04] 获取当前工作目录
来源：http://uo.bjjhwx.cn

Py:   os.getcwd()
来源：http://bt.huanxung.cn

PHP:  getcwd();
来源：http://aq.yuntaijiaju.cn

JS:   process.cwd()
来源：http://pb.newstarts.cn

TS:   process.cwd()
来源：http://sr.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kc.chemitech.net.cn

Go:   os.Getwd()
来源：http://nw.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://st.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jn.yuntaijiaju.cn

[M05] 设置退出码
来源：http://de.gzmigu.cn

Py:   sys.exit(1)
来源：http://xk.hahajie.cn

PHP:  exit(1);
来源：http://oy.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://mv.9csxet.cn

TS:   process.exit(1)
来源：http://ac.9csxet.cn

Java: System.exit(1)
来源：http://cl.chemitech.net.cn

Go:   os.Exit(1)
来源：http://na.newstarts.cn

Ruby: exit 1
来源：http://hh.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oz.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://vs.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://do.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bp.jianghongdianzi.cn

JS:   console.error("err")
来源：http://at.wgjwhj.cn

TS:   console.error("err")
来源：http://aw.nszjky.cn

Java: System.err.println("err")
来源：http://ns.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tv.lnxyls.cn

Ruby: warn "err"
来源：http://tw.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://zr.nicolike.cn

[M07] 判断是否为主入口
来源：http://tf.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://xh.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yu.colortex.cn

JS:   require.main === module
来源：http://fj.huixinmuqiang.cn

TS:   require.main === module
来源：http://dm.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ze.szxytkj.cn

Go:   func main()
来源：http://sn.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aj.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ck.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://up.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://wz.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://tl.9csxet.cn

JS:   process.platform;  process.version
来源：http://aw.panjiajie.cn

TS:   process.platform;  process.version
来源：http://bw.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ne.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ad.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qk.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://of.hahajie.cn

================================================================================
来源：http://op.yuntaijiaju.cn

N. 数据结构与算法
来源：http://gc.jianghongdianzi.cn

================================================================================
来源：http://wz.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://wf.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ta.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uv.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sz.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pl.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ju.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ih.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cj.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ee.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://co.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ae.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qs.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ko.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sr.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mo.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://uh.huanxung.cn

Ruby: arr.sort
来源：http://sc.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://am.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://ts.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ym.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://ty.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gw.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ri.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lj.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hv.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bk.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mm.lnxyls.cn

[N04] 斐波那契数列
来源：http://su.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xp.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gd.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vj.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ui.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oy.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rh.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wr.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ln.lnxyls.cn

[N05] 最大公约数
来源：http://hp.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://lv.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sp.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rk.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hs.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ld.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tv.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://xs.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vj.bjjhwx.cn

[N06] 判断回文字符串
来源：http://fl.szsharing.cn

Py:   s == s[::-1]
来源：http://qm.9csxet.cn

PHP:  $s === strrev($s);
来源：http://na.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://zf.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://fx.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gu.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://gm.asd995.cn

Ruby: s == s.reverse
来源：http://ju.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kj.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://qt.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nk.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yv.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gv.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://vg.shxzukj.cn

Java: // 手写 HashMap
来源：http://fv.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://bj.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://se.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dk.yuexingan06.cn

[N08] 生成全排列
来源：http://pc.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://qw.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://te.colortex.cn

JS:   // 手写回溯递归
来源：http://ph.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://ii.szsharing.cn

Java: // 手写回溯递归
来源：http://cc.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://cp.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://ws.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ik.chemitech.net.cn

[N09] 栈与队列
来源：http://nd.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qe.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jc.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ns.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://az.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cc.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vd.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nc.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fn.nszjky.cn

[N10] 链表节点定义
来源：http://lp.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jz.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bp.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pj.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uz.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://wl.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oc.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://so.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://os.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://us.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qs.huanxung.cn

PHP:  // 手写递归函数
来源：http://nz.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rw.nszjky.cn

Java: // 手写递归
来源：http://yy.huanxung.cn

Go:   // 手写递归
来源：http://xe.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vb.521024.cn

C#:   // 手写递归
来源：http://pw.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zo.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zb.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bs.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zm.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fo.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ef.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hn.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://et.nszjky.cn

================================================================================
来源：http://rq.521024.cn

O. 并发与异步
来源：http://el.hnjuh.cn

================================================================================
来源：http://rg.bjjhwx.cn

[O01] 启动一个线程
来源：http://wa.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jq.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hs.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ni.lnxyls.cn

TS:   // 同 JS
来源：http://bt.huixinmuqiang.cn


<!-- 参考信息 -->