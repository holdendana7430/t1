代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ql.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://jn.asd995.cn

JS:   structuredClone(obj)
来源：http://gi.521024.cn

TS:   structuredClone(obj)
来源：http://qg.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ny.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zv.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bf.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wi.9csxet.cn

[K06] 解析 URL 查询串
来源：http://lt.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xh.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pl.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://st.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ad.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qb.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jr.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pw.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bf.shtwfgs.cn

[K07] 进制转换
来源：http://hn.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pc.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dn.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bm.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rp.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wt.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ww.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lj.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oj.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://fr.colortex.cn

Py:   pickle.dumps(obj)
来源：http://te.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sn.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://rd.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://hb.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tt.bjjhwx.cn

Go:   encoding/gob
来源：http://lm.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://lk.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jt.nicolike.cn

================================================================================
来源：http://rc.wgjwhj.cn

L. 网络请求
来源：http://mn.bookmarksfly.cn

================================================================================
来源：http://pu.colortex.cn

[L01] 发送 GET 请求
来源：http://wa.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aq.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://es.9csxet.cn

JS:   await fetch(url)
来源：http://ck.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://cw.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vr.521024.cn

Go:   resp, err := http.Get(url)
来源：http://dr.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vy.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cu.szsharing.cn

[L02] 发送 POST JSON
来源：http://ca.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yp.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dk.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tk.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fj.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tn.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qf.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://xy.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qf.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://io.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cw.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ki.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ir.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ph.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://my.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yw.gzmigu.cn

[L04] 设置超时
来源：http://kx.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://ba.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nf.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ye.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cg.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ne.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ta.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pd.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gn.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://pm.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gw.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tn.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dk.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hc.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vj.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bq.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kl.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xv.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://lr.chemitech.net.cn

Py:   resp.json()
来源：http://do.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://hd.gzmigu.cn

JS:   await resp.json()
来源：http://nr.huixiangedu.cn

TS:   await resp.json()
来源：http://dk.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nh.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vx.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://ob.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ud.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://ke.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aw.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qo.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://tx.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://xa.asd995.cn

Java: resp.statusCode()
来源：http://ld.bjjhwx.cn

Go:   resp.StatusCode
来源：http://yv.hahajie.cn

Ruby: resp.code.to_i
来源：http://xr.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://xy.gzmigu.cn

[L08] 并发请求多个地址
来源：http://zw.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gx.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://xx.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tt.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jl.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qh.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dh.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zn.nszjky.cn

================================================================================
来源：http://wo.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://af.colortex.cn

================================================================================
来源：http://oq.wgjwhj.cn

[M01] 读取命令行参数
来源：http://kj.colortex.cn

Py:   sys.argv[1:]
来源：http://dn.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ok.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://nf.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://ia.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://yz.hahajie.cn

Go:   os.Args[1:]
来源：http://kv.huixiangedu.cn

Ruby: ARGV
来源：http://bi.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ft.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://rw.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://lx.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qg.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://iv.asd995.cn

TS:   process.env.HOME
来源：http://ki.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://mm.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://on.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://mi.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kb.hnjuh.cn

[M03] 执行外部命令
来源：http://lh.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ba.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cm.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qn.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yi.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xf.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://az.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vk.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://bj.colortex.cn

[M04] 获取当前工作目录
来源：http://xa.asd995.cn

Py:   os.getcwd()
来源：http://ts.9csxet.cn

PHP:  getcwd();
来源：http://nl.colortex.cn

JS:   process.cwd()
来源：http://gu.gzmigu.cn

TS:   process.cwd()
来源：http://zq.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://jl.szsharing.cn

Go:   os.Getwd()
来源：http://mh.huanxung.cn

Ruby: Dir.pwd
来源：http://ik.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ya.huixinmuqiang.cn

[M05] 设置退出码
来源：http://rj.haigaiapp.cn

Py:   sys.exit(1)
来源：http://rq.shtwfgs.cn

PHP:  exit(1);
来源：http://fc.yuexingan06.cn

JS:   process.exit(1)
来源：http://bu.yuexingan06.cn

TS:   process.exit(1)
来源：http://gc.shxzskj.cn

Java: System.exit(1)
来源：http://kj.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://dr.nszjky.cn

Ruby: exit 1
来源：http://aw.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rf.huanxung.cn

[M06] 向标准错误输出
来源：http://av.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://nl.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lb.bjjhwx.cn

JS:   console.error("err")
来源：http://ah.hnjuh.cn

TS:   console.error("err")
来源：http://re.szsharing.cn

Java: System.err.println("err")
来源：http://wn.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sx.wgjwhj.cn

Ruby: warn "err"
来源：http://jv.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://wl.asd995.cn

[M07] 判断是否为主入口
来源：http://bz.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://ly.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nd.jctech888.com.cn

JS:   require.main === module
来源：http://zj.haigaiapp.cn

TS:   require.main === module
来源：http://kg.newstarts.cn

Java: public static void main(String[] args)
来源：http://pi.shxzskj.cn

Go:   func main()
来源：http://vr.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ph.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ie.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://wm.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://vy.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://dq.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://um.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://dv.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uw.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ln.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wg.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mc.bjjhwx.cn

================================================================================
来源：http://fn.huixiangedu.cn

N. 数据结构与算法
来源：http://nk.jianghongdianzi.cn

================================================================================
来源：http://uw.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://ag.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bx.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wb.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://su.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jb.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rt.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://px.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pa.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kk.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ab.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://eu.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://au.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jz.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kg.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iq.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://cf.bjjhwx.cn

Ruby: arr.sort
来源：http://vp.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://it.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://ro.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fq.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://jl.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://so.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vb.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yi.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zi.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fd.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ck.colortex.cn

[N04] 斐波那契数列
来源：http://ey.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ak.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ve.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://br.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ed.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eb.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oy.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oc.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ae.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://bk.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kt.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ae.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://us.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vk.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bt.nszjky.cn

Ruby: a.gcd(b)
来源：http://mb.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cw.hnjuh.cn

[N06] 判断回文字符串
来源：http://vk.nszjky.cn

Py:   s == s[::-1]
来源：http://zs.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://gf.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ee.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://rl.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vl.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://jx.jctech888.com.cn

Ruby: s == s.reverse
来源：http://mo.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jk.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://jt.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vm.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ns.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jx.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://po.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ip.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://vl.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://vk.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dy.colortex.cn

[N08] 生成全排列
来源：http://hb.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://tj.hahajie.cn

PHP:  // 手写递归交换
来源：http://uw.shxzukj.cn

JS:   // 手写回溯递归
来源：http://uc.nszjky.cn

TS:   // 手写回溯递归
来源：http://oy.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://px.panjiajie.cn

Go:   // 手写回溯递归
来源：http://vy.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://ja.hnjuh.cn

C#:   // 手写回溯递归
来源：http://uj.colortex.cn

[N09] 栈与队列
来源：http://li.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fn.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cm.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lw.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hr.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ub.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://be.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xf.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bd.bjjhwx.cn

[N10] 链表节点定义
来源：http://sc.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qs.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fx.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ir.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://px.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://kr.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dm.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cn.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zz.asd995.cn

[N11] 二叉树中序遍历
来源：http://qd.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lm.lnxyls.cn

PHP:  // 手写递归函数
来源：http://yc.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://es.jctech888.com.cn

Java: // 手写递归
来源：http://rb.wgjwhj.cn

Go:   // 手写递归
来源：http://im.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wg.muxihuayi.cn

C#:   // 手写递归
来源：http://in.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ng.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qx.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kb.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kl.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vf.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ko.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wy.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rt.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://et.szxytkj.cn

================================================================================
来源：http://jt.huixiangedu.cn

O. 并发与异步
来源：http://hs.huixinmuqiang.cn

================================================================================
来源：http://mg.shxzukj.cn

[O01] 启动一个线程
来源：http://ex.shxzskj.cn


<!-- 参考信息 -->