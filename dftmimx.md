代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://zh.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mv.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://id.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cr.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://kl.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yt.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hq.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jt.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ys.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rr.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pc.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bo.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qt.nszjky.cn

[K07] 进制转换
来源：http://ce.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ow.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://na.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xt.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eo.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ox.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://as.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lb.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wp.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://kj.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://gb.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qm.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bg.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://ly.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qi.chemitech.net.cn

Go:   encoding/gob
来源：http://qt.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://zy.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uv.shxzukj.cn

================================================================================
来源：http://gi.shtwfgs.cn

L. 网络请求
来源：http://nx.hnjuh.cn

================================================================================
来源：http://da.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://pj.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aw.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yl.hnjuh.cn

JS:   await fetch(url)
来源：http://fj.nszjky.cn

TS:   await fetch(url)
来源：http://ub.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jn.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://oo.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iu.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gl.nszjky.cn

[L02] 发送 POST JSON
来源：http://kk.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yg.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xb.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jd.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ag.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lb.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://do.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yn.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fz.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://je.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://er.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://no.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yw.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ht.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ny.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ug.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ui.shxzukj.cn

[L04] 设置超时
来源：http://wm.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://st.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hc.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mz.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uu.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kx.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wd.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://us.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ds.szsharing.cn

[L05] 上传文件（multipart）
来源：http://wc.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ah.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lh.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xo.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pd.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mr.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lj.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qk.521024.cn

[L06] 解析响应为 JSON
来源：http://gs.jctech888.com.cn

Py:   resp.json()
来源：http://oa.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://wv.wgjwhj.cn

JS:   await resp.json()
来源：http://bs.hahajie.cn

TS:   await resp.json()
来源：http://oe.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tl.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qx.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://fb.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vs.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://xl.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yu.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kq.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://id.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://ii.huixiangedu.cn

Java: resp.statusCode()
来源：http://lx.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ur.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://jj.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://rb.szsharing.cn

[L08] 并发请求多个地址
来源：http://jt.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zv.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://mp.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bw.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sx.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://be.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cj.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rr.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zj.chemitech.net.cn

================================================================================
来源：http://cz.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://uh.yuexingan06.cn

================================================================================
来源：http://ok.wgjwhj.cn

[M01] 读取命令行参数
来源：http://zr.szxytkj.cn

Py:   sys.argv[1:]
来源：http://uc.asd995.cn

PHP:  $argv;  $argc;
来源：http://qw.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://na.521024.cn

TS:   process.argv.slice(2)
来源：http://gv.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://uk.hnjuh.cn

Go:   os.Args[1:]
来源：http://xk.jianghongdianzi.cn

Ruby: ARGV
来源：http://om.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://zo.bookmarksfly.cn

[M02] 读取环境变量
来源：http://aq.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://jv.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cc.szxytkj.cn

JS:   process.env.HOME
来源：http://bp.shtwfgs.cn

TS:   process.env.HOME
来源：http://mv.nicolike.cn

Java: System.getenv("HOME")
来源：http://gt.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bg.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ig.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://or.hahajie.cn

[M03] 执行外部命令
来源：http://bf.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kx.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://db.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uc.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wc.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xy.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ec.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://wd.asd995.cn

[M04] 获取当前工作目录
来源：http://su.huanxung.cn

Py:   os.getcwd()
来源：http://kz.shxzskj.cn

PHP:  getcwd();
来源：http://uq.newstarts.cn

JS:   process.cwd()
来源：http://wj.colortex.cn

TS:   process.cwd()
来源：http://ld.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://dz.wgjwhj.cn

Go:   os.Getwd()
来源：http://qe.wgjwhj.cn

Ruby: Dir.pwd
来源：http://kj.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ij.nszjky.cn

[M05] 设置退出码
来源：http://ho.hahajie.cn

Py:   sys.exit(1)
来源：http://kr.colortex.cn

PHP:  exit(1);
来源：http://cx.huanxung.cn

JS:   process.exit(1)
来源：http://dg.shxzskj.cn

TS:   process.exit(1)
来源：http://tg.9csxet.cn

Java: System.exit(1)
来源：http://nc.nicolike.cn

Go:   os.Exit(1)
来源：http://lb.nicolike.cn

Ruby: exit 1
来源：http://pj.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lz.huanxung.cn

[M06] 向标准错误输出
来源：http://og.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://jx.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mn.nicolike.cn

JS:   console.error("err")
来源：http://us.gzmigu.cn

TS:   console.error("err")
来源：http://jf.colortex.cn

Java: System.err.println("err")
来源：http://yj.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yq.jianghongdianzi.cn

Ruby: warn "err"
来源：http://by.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vy.hahajie.cn

[M07] 判断是否为主入口
来源：http://rh.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://lv.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gy.huixiangedu.cn

JS:   require.main === module
来源：http://de.gzmigu.cn

TS:   require.main === module
来源：http://kl.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://el.huixiangedu.cn

Go:   func main()
来源：http://ha.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mk.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://se.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://he.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://tp.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://xj.szsharing.cn

JS:   process.platform;  process.version
来源：http://zq.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://fk.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xn.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://at.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cq.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dr.panjiajie.cn

================================================================================
来源：http://fg.hahajie.cn

N. 数据结构与算法
来源：http://es.hahajie.cn

================================================================================
来源：http://mo.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://kn.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wl.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mv.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hx.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iy.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ho.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tx.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wc.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://hg.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://ja.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ty.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tx.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wb.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kt.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://mf.muxihuayi.cn

Ruby: arr.sort
来源：http://yz.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ng.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://em.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wb.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://zy.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dz.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gw.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wb.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dr.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fj.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kh.nicolike.cn

[N04] 斐波那契数列
来源：http://am.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zy.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uz.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fs.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xa.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mv.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lk.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lu.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://re.yuexingan06.cn

[N05] 最大公约数
来源：http://gi.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://yx.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ne.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ut.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bc.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ys.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uo.szsharing.cn

Ruby: a.gcd(b)
来源：http://mt.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://by.shxzskj.cn

[N06] 判断回文字符串
来源：http://rk.hahajie.cn

Py:   s == s[::-1]
来源：http://fp.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://vd.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://ll.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://gu.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cz.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://ss.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://jc.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ep.colortex.cn

[N07] 两数之和（返回下标）
来源：http://fd.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pi.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wn.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cg.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ch.panjiajie.cn

Java: // 手写 HashMap
来源：http://pn.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://wx.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://wb.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://to.jctech888.com.cn

[N08] 生成全排列
来源：http://gi.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://wl.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://zw.nszjky.cn

JS:   // 手写回溯递归
来源：http://kh.hnjuh.cn

TS:   // 手写回溯递归
来源：http://th.huanxung.cn

Java: // 手写回溯递归
来源：http://vn.colortex.cn

Go:   // 手写回溯递归
来源：http://wk.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://yl.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://fd.shxzukj.cn

[N09] 栈与队列
来源：http://ni.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hc.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qt.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bw.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qj.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vy.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vk.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nt.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kt.521024.cn

[N10] 链表节点定义
来源：http://rh.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ez.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yv.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tf.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sb.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://jh.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xo.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://py.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://su.521024.cn

[N11] 二叉树中序遍历
来源：http://fp.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kv.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://cq.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://su.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.bjjhwx.cn

Java: // 手写递归
来源：http://wl.wgjwhj.cn

Go:   // 手写递归
来源：http://ps.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qw.huixinmuqiang.cn

C#:   // 手写递归
来源：http://yq.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vx.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eb.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fn.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bs.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lz.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xb.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jv.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ib.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xe.haigaiapp.cn

================================================================================
来源：http://vd.lnxyls.cn

O. 并发与异步
来源：http://mb.gzmigu.cn

================================================================================
来源：http://uu.shxzukj.cn

[O01] 启动一个线程
来源：http://im.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ne.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wp.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cz.haigaiapp.cn

TS:   // 同 JS
来源：http://ar.haigaiapp.cn


<!-- 参考信息 -->