代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://my.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ge.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://dd.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://wc.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fi.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fa.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sx.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ml.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://yo.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uw.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xs.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pj.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ha.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ua.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wo.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gn.bookmarksfly.cn

[K07] 进制转换
来源：http://sl.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jx.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ve.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tv.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vq.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ha.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://go.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pz.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jg.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://bw.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://ve.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mh.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://we.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://hj.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://id.shtwfgs.cn

Go:   encoding/gob
来源：http://ib.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://zf.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oj.asd995.cn

================================================================================
来源：http://pi.chemitech.net.cn

L. 网络请求
来源：http://ub.yuexingan06.cn

================================================================================
来源：http://rt.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://bw.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ok.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ed.haigaiapp.cn

JS:   await fetch(url)
来源：http://vn.bjjhwx.cn

TS:   await fetch(url)
来源：http://ww.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zu.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ix.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eq.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pm.shxzskj.cn

[L02] 发送 POST JSON
来源：http://tc.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ec.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ym.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jv.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rb.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nh.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vw.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ot.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ye.asd995.cn

[L03] 设置自定义请求头
来源：http://dc.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bs.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://af.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wq.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://po.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xk.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://td.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hm.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vf.gzmigu.cn

[L04] 设置超时
来源：http://us.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ml.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yt.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pu.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ml.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://me.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uu.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mi.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cn.asd995.cn

[L05] 上传文件（multipart）
来源：http://sz.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eo.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bk.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tg.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ex.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jq.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nc.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mj.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yr.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://rc.szxytkj.cn

Py:   resp.json()
来源：http://hs.asd995.cn

PHP:  json_decode($body, true);
来源：http://ov.521024.cn

JS:   await resp.json()
来源：http://pa.9csxet.cn

TS:   await resp.json()
来源：http://cz.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dk.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sa.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://gd.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kz.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://hk.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zh.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://io.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://qa.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://tg.9csxet.cn

Java: resp.statusCode()
来源：http://hs.bjjhwx.cn

Go:   resp.StatusCode
来源：http://aa.hnjuh.cn

Ruby: resp.code.to_i
来源：http://tg.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://lx.szxytkj.cn

[L08] 并发请求多个地址
来源：http://rj.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://km.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://ru.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://td.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://da.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eh.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xb.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sk.huanxung.cn

================================================================================
来源：http://et.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ap.gzmigu.cn

================================================================================
来源：http://av.nicolike.cn

[M01] 读取命令行参数
来源：http://jm.shxzskj.cn

Py:   sys.argv[1:]
来源：http://eq.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://vo.huanxung.cn

JS:   process.argv.slice(2)
来源：http://yr.asd995.cn

TS:   process.argv.slice(2)
来源：http://fm.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://xh.colortex.cn

Go:   os.Args[1:]
来源：http://df.newstarts.cn

Ruby: ARGV
来源：http://jp.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://wi.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://st.521024.cn

Py:   os.environ.get("HOME")
来源：http://ve.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jn.hnjuh.cn

JS:   process.env.HOME
来源：http://wg.huanxung.cn

TS:   process.env.HOME
来源：http://gb.shxzukj.cn

Java: System.getenv("HOME")
来源：http://rd.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fy.521024.cn

Ruby: ENV["HOME"]
来源：http://ah.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://op.hahajie.cn

[M03] 执行外部命令
来源：http://ox.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bb.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ur.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://up.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://no.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ei.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://na.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lb.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://sq.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://yx.huanxung.cn

Py:   os.getcwd()
来源：http://ca.yuntaijiaju.cn

PHP:  getcwd();
来源：http://qd.yuexingan06.cn

JS:   process.cwd()
来源：http://rj.hahajie.cn

TS:   process.cwd()
来源：http://gq.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://xt.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://xl.jctech888.com.cn

Ruby: Dir.pwd
来源：http://qf.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qj.gzmigu.cn

[M05] 设置退出码
来源：http://cf.szsharing.cn

Py:   sys.exit(1)
来源：http://kg.bookmarksfly.cn

PHP:  exit(1);
来源：http://bu.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://bp.panjiajie.cn

TS:   process.exit(1)
来源：http://nl.jctech888.com.cn

Java: System.exit(1)
来源：http://ys.shxzukj.cn

Go:   os.Exit(1)
来源：http://fp.huixinmuqiang.cn

Ruby: exit 1
来源：http://ge.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ca.lnxyls.cn

[M06] 向标准错误输出
来源：http://yo.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://nc.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ob.lnxyls.cn

JS:   console.error("err")
来源：http://sh.gzmigu.cn

TS:   console.error("err")
来源：http://ki.nicolike.cn

Java: System.err.println("err")
来源：http://rz.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ge.huanxung.cn

Ruby: warn "err"
来源：http://mk.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://yk.lnxyls.cn

[M07] 判断是否为主入口
来源：http://ey.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://qw.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xt.huixinmuqiang.cn

JS:   require.main === module
来源：http://kw.yuexingan06.cn

TS:   require.main === module
来源：http://ld.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://mx.jianghongdianzi.cn

Go:   func main()
来源：http://gu.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bg.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://iy.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://ed.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://qz.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://wd.nszjky.cn

JS:   process.platform;  process.version
来源：http://uu.521024.cn

TS:   process.platform;  process.version
来源：http://lr.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nv.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zq.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nw.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wb.hnjuh.cn

================================================================================
来源：http://zf.asd995.cn

N. 数据结构与算法
来源：http://kj.huanxung.cn

================================================================================
来源：http://fn.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://pd.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xb.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://db.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ag.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gy.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qf.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ef.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uv.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dk.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://oi.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://hp.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gb.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xj.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xl.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ac.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://gb.yuntaijiaju.cn

Ruby: arr.sort
来源：http://va.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ud.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://fb.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tk.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ti.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ev.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zw.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://do.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ou.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sc.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://an.shxzukj.cn

[N04] 斐波那契数列
来源：http://zs.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qe.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rn.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zf.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tb.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vx.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sa.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rd.huanxung.cn

[N05] 最大公约数
来源：http://vl.521024.cn

Py:   math.gcd(a, b)
来源：http://fm.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vu.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fe.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vf.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ud.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yx.gzmigu.cn

Ruby: a.gcd(b)
来源：http://il.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yk.asd995.cn

[N06] 判断回文字符串
来源：http://yl.hnjuh.cn

Py:   s == s[::-1]
来源：http://ww.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://nf.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://od.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://bn.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yb.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://cl.szsharing.cn

Ruby: s == s.reverse
来源：http://zi.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://no.colortex.cn

[N07] 两数之和（返回下标）
来源：http://en.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lz.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hl.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ox.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://uy.muxihuayi.cn

Java: // 手写 HashMap
来源：http://bx.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://xy.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://nz.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jy.wgjwhj.cn

[N08] 生成全排列
来源：http://zv.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://ev.9csxet.cn

PHP:  // 手写递归交换
来源：http://dn.newstarts.cn

JS:   // 手写回溯递归
来源：http://do.asd995.cn

TS:   // 手写回溯递归
来源：http://kf.szxytkj.cn

Java: // 手写回溯递归
来源：http://qd.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://eq.521024.cn

Ruby: arr.permutation.to_a
来源：http://by.shxzskj.cn

C#:   // 手写回溯递归
来源：http://qb.yuntaijiaju.cn

[N09] 栈与队列
来源：http://ei.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ie.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uq.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vc.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hp.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ui.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ng.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xx.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dn.shxzukj.cn

[N10] 链表节点定义
来源：http://uk.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://be.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xf.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zh.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zg.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://dz.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xo.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ju.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://lv.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ct.shxzukj.cn

PHP:  // 手写递归函数
来源：http://qr.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fk.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dp.gzmigu.cn

Java: // 手写递归
来源：http://ip.panjiajie.cn

Go:   // 手写递归
来源：http://yt.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iu.nicolike.cn

C#:   // 手写递归
来源：http://is.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qq.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dm.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rn.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://il.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yx.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tz.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vf.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ip.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vu.nszjky.cn

================================================================================
来源：http://pf.newstarts.cn

O. 并发与异步
来源：http://qw.newstarts.cn

================================================================================
来源：http://pc.asd995.cn

[O01] 启动一个线程
来源：http://rb.lnxyls.cn


<!-- 参考信息 -->