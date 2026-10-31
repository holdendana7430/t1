代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ck.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ns.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ve.hnjuh.cn

TS:   structuredClone(obj)
来源：http://ne.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lg.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qw.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ui.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://up.asd995.cn

[K06] 解析 URL 查询串
来源：http://sm.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ar.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fc.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fh.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zr.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hy.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nh.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aw.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jk.haigaiapp.cn

[K07] 进制转换
来源：http://fr.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xo.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qa.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fz.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lr.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ru.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ge.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://le.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qg.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://nx.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://ya.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pj.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nf.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://mp.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://em.9csxet.cn

Go:   encoding/gob
来源：http://gt.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://py.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nv.shxzskj.cn

================================================================================
来源：http://ve.huixinmuqiang.cn

L. 网络请求
来源：http://dk.bookmarksfly.cn

================================================================================
来源：http://xl.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://io.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sg.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aq.nszjky.cn

JS:   await fetch(url)
来源：http://xv.chemitech.net.cn

TS:   await fetch(url)
来源：http://oy.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yc.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://an.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lh.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qe.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://ed.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rh.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dh.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vu.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aj.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aw.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jt.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wd.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wo.szxytkj.cn

[L03] 设置自定义请求头
来源：http://ee.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hf.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bz.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zm.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qg.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://as.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wc.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ek.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tp.wgjwhj.cn

[L04] 设置超时
来源：http://yz.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://bp.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rl.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fx.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qc.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qe.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vo.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vj.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ww.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://tx.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fy.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fd.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sk.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qw.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ru.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iz.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fj.nicolike.cn

[L06] 解析响应为 JSON
来源：http://mo.huanxung.cn

Py:   resp.json()
来源：http://qs.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://cv.yuntaijiaju.cn

JS:   await resp.json()
来源：http://wq.newstarts.cn

TS:   await resp.json()
来源：http://kl.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ap.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qc.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://lb.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rl.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://jm.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fv.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bf.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ni.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://rf.bjjhwx.cn

Java: resp.statusCode()
来源：http://wv.szsharing.cn

Go:   resp.StatusCode
来源：http://ch.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://vr.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://zm.lnxyls.cn

[L08] 并发请求多个地址
来源：http://it.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wq.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://ma.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://px.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://st.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qq.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sv.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nn.huanxung.cn

================================================================================
来源：http://ab.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://qc.shxzukj.cn

================================================================================
来源：http://bo.jctech888.com.cn

[M01] 读取命令行参数
来源：http://es.huanxung.cn

Py:   sys.argv[1:]
来源：http://es.huanxung.cn

PHP:  $argv;  $argc;
来源：http://vt.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://fp.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://fn.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://vc.shxzukj.cn

Go:   os.Args[1:]
来源：http://sl.shtwfgs.cn

Ruby: ARGV
来源：http://xe.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://da.shtwfgs.cn

[M02] 读取环境变量
来源：http://ux.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ds.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dk.shtwfgs.cn

JS:   process.env.HOME
来源：http://kp.bjjhwx.cn

TS:   process.env.HOME
来源：http://hs.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://bk.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://av.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ku.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ke.huanxung.cn

[M03] 执行外部命令
来源：http://pr.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oe.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uy.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pl.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dm.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ac.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://df.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fo.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://aw.huanxung.cn

[M04] 获取当前工作目录
来源：http://kq.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://wn.huixinmuqiang.cn

PHP:  getcwd();
来源：http://aw.jctech888.com.cn

JS:   process.cwd()
来源：http://ne.bookmarksfly.cn

TS:   process.cwd()
来源：http://gc.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://jt.521024.cn

Go:   os.Getwd()
来源：http://vb.shxzskj.cn

Ruby: Dir.pwd
来源：http://kj.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ru.huixiangedu.cn

[M05] 设置退出码
来源：http://yq.shxzskj.cn

Py:   sys.exit(1)
来源：http://me.hahajie.cn

PHP:  exit(1);
来源：http://pj.shxzskj.cn

JS:   process.exit(1)
来源：http://eg.nicolike.cn

TS:   process.exit(1)
来源：http://yl.nszjky.cn

Java: System.exit(1)
来源：http://uw.panjiajie.cn

Go:   os.Exit(1)
来源：http://lk.9csxet.cn

Ruby: exit 1
来源：http://en.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wf.haigaiapp.cn

[M06] 向标准错误输出
来源：http://jk.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://yr.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jk.yuexingan06.cn

JS:   console.error("err")
来源：http://wo.huixiangedu.cn

TS:   console.error("err")
来源：http://mv.newstarts.cn

Java: System.err.println("err")
来源：http://vz.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gy.panjiajie.cn

Ruby: warn "err"
来源：http://um.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://hb.nicolike.cn

[M07] 判断是否为主入口
来源：http://pu.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://sn.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://up.bookmarksfly.cn

JS:   require.main === module
来源：http://uy.colortex.cn

TS:   require.main === module
来源：http://zg.gzmigu.cn

Java: public static void main(String[] args)
来源：http://wy.gzmigu.cn

Go:   func main()
来源：http://ji.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://li.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://ur.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://xl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://uq.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://qm.lnxyls.cn

JS:   process.platform;  process.version
来源：http://mj.nicolike.cn

TS:   process.platform;  process.version
来源：http://dj.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dh.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oy.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ep.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ey.nicolike.cn

================================================================================
来源：http://pd.huanxung.cn

N. 数据结构与算法
来源：http://fw.chemitech.net.cn

================================================================================
来源：http://ce.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://kp.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uo.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dc.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vo.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://el.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cy.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://so.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qr.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fk.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://by.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://rz.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gc.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ar.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ln.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://so.colortex.cn

Go:   slices.Sort(arr)
来源：http://ct.nszjky.cn

Ruby: arr.sort
来源：http://dk.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ax.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://vz.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lq.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://cg.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sd.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tn.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lg.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yo.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xf.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pv.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://ug.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gr.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pz.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rr.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lt.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ut.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yg.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qx.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://td.shxzukj.cn

[N05] 最大公约数
来源：http://jb.newstarts.cn

Py:   math.gcd(a, b)
来源：http://ba.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ng.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qr.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hq.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pc.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hr.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://vf.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://km.nicolike.cn

[N06] 判断回文字符串
来源：http://iv.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://ha.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://uj.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ce.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://rn.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wp.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://xh.huanxung.cn

Ruby: s == s.reverse
来源：http://ja.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vv.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://le.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ig.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rv.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qz.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://gb.huixiangedu.cn

Java: // 手写 HashMap
来源：http://gd.9csxet.cn

Go:   // 手写 map[int]int
来源：http://sc.asd995.cn

Ruby: // 手写 Hash
来源：http://zj.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ad.gzmigu.cn

[N08] 生成全排列
来源：http://ig.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://yv.shxzukj.cn

PHP:  // 手写递归交换
来源：http://tp.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://th.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://cj.shxzskj.cn

Java: // 手写回溯递归
来源：http://an.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://ki.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://pb.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://fy.asd995.cn

[N09] 栈与队列
来源：http://ji.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uw.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xe.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wt.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ft.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ix.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hx.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vs.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gy.hnjuh.cn

[N10] 链表节点定义
来源：http://bx.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mx.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mr.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ic.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ri.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ok.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tp.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://il.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kw.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://uc.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uz.panjiajie.cn

PHP:  // 手写递归函数
来源：http://hz.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zt.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.9csxet.cn

Java: // 手写递归
来源：http://pc.haigaiapp.cn

Go:   // 手写递归
来源：http://ax.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tz.shxzskj.cn

C#:   // 手写递归
来源：http://it.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mr.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vd.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wb.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xb.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sg.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gs.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://im.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tw.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gg.asd995.cn

================================================================================
来源：http://pn.yuexingan06.cn

O. 并发与异步
来源：http://ka.521024.cn

================================================================================
来源：http://zd.lnxyls.cn

[O01] 启动一个线程
来源：http://gj.yuntaijiaju.cn


<!-- 参考信息 -->