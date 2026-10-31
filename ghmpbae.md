代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hl.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://jg.hnjuh.cn

JS:   structuredClone(obj)
来源：http://jp.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ez.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lq.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yh.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ya.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qt.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://bs.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pj.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://da.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uj.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wj.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ys.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ej.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hj.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://te.hahajie.cn

[K07] 进制转换
来源：http://ds.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ar.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tl.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pw.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wf.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lb.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vf.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sd.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://re.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://uy.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://mc.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iy.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://gr.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://cg.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rf.panjiajie.cn

Go:   encoding/gob
来源：http://kh.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://zp.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ep.yuexingan06.cn

================================================================================
来源：http://tm.gzmigu.cn

L. 网络请求
来源：http://yf.9csxet.cn

================================================================================
来源：http://xo.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ur.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wg.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ax.panjiajie.cn

JS:   await fetch(url)
来源：http://nf.gzmigu.cn

TS:   await fetch(url)
来源：http://du.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xx.521024.cn

Go:   resp, err := http.Get(url)
来源：http://sr.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://do.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jj.nszjky.cn

[L02] 发送 POST JSON
来源：http://nv.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ip.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ck.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qu.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yx.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dq.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xc.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xq.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://gd.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yj.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tq.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dq.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://df.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://au.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bh.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xc.jianghongdianzi.cn

[L04] 设置超时
来源：http://bd.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://fb.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://we.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pg.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kf.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jm.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dy.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zd.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://sn.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://me.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sq.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ji.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yt.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ge.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nh.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sq.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iv.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://vm.asd995.cn

Py:   resp.json()
来源：http://xx.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://jh.newstarts.cn

JS:   await resp.json()
来源：http://xa.lnxyls.cn

TS:   await resp.json()
来源：http://hz.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kl.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://or.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://gf.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yz.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://ls.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zl.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rp.colortex.cn

JS:   resp.ok;  resp.status
来源：http://fq.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://aq.jctech888.com.cn

Java: resp.statusCode()
来源：http://mc.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://qw.nszjky.cn

Ruby: resp.code.to_i
来源：http://uw.asd995.cn

C#:   (int)resp.StatusCode
来源：http://td.shxzukj.cn

[L08] 并发请求多个地址
来源：http://ay.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tq.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://bj.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ox.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gw.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ks.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wm.huixinmuqiang.cn

================================================================================
来源：http://en.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://dl.haigaiapp.cn

================================================================================
来源：http://dx.colortex.cn

[M01] 读取命令行参数
来源：http://bx.szsharing.cn

Py:   sys.argv[1:]
来源：http://sc.nicolike.cn

PHP:  $argv;  $argc;
来源：http://nq.nicolike.cn

JS:   process.argv.slice(2)
来源：http://yv.521024.cn

TS:   process.argv.slice(2)
来源：http://bo.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://xc.szsharing.cn

Go:   os.Args[1:]
来源：http://lv.szxytkj.cn

Ruby: ARGV
来源：http://tu.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://xy.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://ee.colortex.cn

Py:   os.environ.get("HOME")
来源：http://hi.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://je.newstarts.cn

JS:   process.env.HOME
来源：http://aq.hahajie.cn

TS:   process.env.HOME
来源：http://rm.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://gr.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zd.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://hc.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qj.521024.cn

[M03] 执行外部命令
来源：http://st.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://he.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ch.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kc.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ad.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lu.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jn.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://du.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://ef.huanxung.cn

[M04] 获取当前工作目录
来源：http://xb.bjjhwx.cn

Py:   os.getcwd()
来源：http://mt.huixinmuqiang.cn

PHP:  getcwd();
来源：http://yf.shtwfgs.cn

JS:   process.cwd()
来源：http://ym.szxytkj.cn

TS:   process.cwd()
来源：http://xh.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://nd.panjiajie.cn

Go:   os.Getwd()
来源：http://zf.521024.cn

Ruby: Dir.pwd
来源：http://tp.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kj.panjiajie.cn

[M05] 设置退出码
来源：http://lc.yuexingan06.cn

Py:   sys.exit(1)
来源：http://mk.haigaiapp.cn

PHP:  exit(1);
来源：http://il.wgjwhj.cn

JS:   process.exit(1)
来源：http://oe.yuexingan06.cn

TS:   process.exit(1)
来源：http://xs.shtwfgs.cn

Java: System.exit(1)
来源：http://th.gzmigu.cn

Go:   os.Exit(1)
来源：http://cb.shxzskj.cn

Ruby: exit 1
来源：http://zb.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yc.shxzskj.cn

[M06] 向标准错误输出
来源：http://be.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ze.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sx.chemitech.net.cn

JS:   console.error("err")
来源：http://lz.shxzukj.cn

TS:   console.error("err")
来源：http://wl.huanxung.cn

Java: System.err.println("err")
来源：http://zu.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mr.asd995.cn

Ruby: warn "err"
来源：http://rc.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://us.hnjuh.cn

[M07] 判断是否为主入口
来源：http://xp.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://yn.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ln.chemitech.net.cn

JS:   require.main === module
来源：http://ea.jctech888.com.cn

TS:   require.main === module
来源：http://ro.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://gv.jianghongdianzi.cn

Go:   func main()
来源：http://nh.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cd.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://rq.asd995.cn

[M08] 获取系统与运行时信息
来源：http://zs.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://qe.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://uw.huanxung.cn

JS:   process.platform;  process.version
来源：http://py.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ak.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kc.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vv.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vl.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sk.asd995.cn

================================================================================
来源：http://bk.nicolike.cn

N. 数据结构与算法
来源：http://nf.shxzskj.cn

================================================================================
来源：http://nb.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://il.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yq.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ax.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vq.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://la.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ny.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://lp.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qb.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qk.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://jp.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://oo.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://du.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fy.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yb.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gr.nszjky.cn

Go:   slices.Sort(arr)
来源：http://fo.nszjky.cn

Ruby: arr.sort
来源：http://wy.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gt.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://gd.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nl.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://po.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wm.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://at.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bm.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eg.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qq.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://de.nszjky.cn

[N04] 斐波那契数列
来源：http://mz.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://re.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ke.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://so.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tz.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ii.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sw.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://un.nicolike.cn

[N05] 最大公约数
来源：http://qc.521024.cn

Py:   math.gcd(a, b)
来源：http://vq.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qu.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kq.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vg.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zc.nicolike.cn

Ruby: a.gcd(b)
来源：http://hk.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ke.newstarts.cn

[N06] 判断回文字符串
来源：http://nc.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://si.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ny.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://vr.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://av.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gn.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://pr.haigaiapp.cn

Ruby: s == s.reverse
来源：http://os.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cx.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ti.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qz.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qx.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qe.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://hj.jctech888.com.cn

Java: // 手写 HashMap
来源：http://vm.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://ul.newstarts.cn

Ruby: // 手写 Hash
来源：http://ob.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://em.nszjky.cn

[N08] 生成全排列
来源：http://os.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://on.521024.cn

PHP:  // 手写递归交换
来源：http://sm.nicolike.cn

JS:   // 手写回溯递归
来源：http://jd.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://xn.huanxung.cn

Java: // 手写回溯递归
来源：http://er.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://gt.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://yc.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://sg.szsharing.cn

[N09] 栈与队列
来源：http://sz.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://di.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nf.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tx.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oy.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ib.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://td.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sz.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yl.9csxet.cn

[N10] 链表节点定义
来源：http://ox.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rg.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ke.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ka.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://is.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://zn.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ks.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ur.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xo.szsharing.cn

[N11] 二叉树中序遍历
来源：http://wh.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ae.panjiajie.cn

PHP:  // 手写递归函数
来源：http://jt.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dc.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jb.muxihuayi.cn

Java: // 手写递归
来源：http://nz.nicolike.cn

Go:   // 手写递归
来源：http://yc.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wn.colortex.cn

C#:   // 手写递归
来源：http://ju.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vg.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zw.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yk.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://he.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ql.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://os.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://po.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ul.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fb.jctech888.com.cn

================================================================================
来源：http://lv.bjjhwx.cn

O. 并发与异步
来源：http://vx.lnxyls.cn

================================================================================
来源：http://te.chemitech.net.cn

[O01] 启动一个线程
来源：http://mv.521024.cn


<!-- 参考信息 -->