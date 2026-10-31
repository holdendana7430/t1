代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://za.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gl.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kh.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zg.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sg.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xx.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fd.szxytkj.cn

[K05] 深拷贝对象
来源：http://hn.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://yy.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://fm.gzmigu.cn

JS:   structuredClone(obj)
来源：http://hu.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://jp.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mi.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cm.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://no.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ih.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://vv.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gd.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ad.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iw.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://se.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ab.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ux.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zc.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cb.hnjuh.cn

[K07] 进制转换
来源：http://vz.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rq.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ug.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fd.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gy.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ce.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xg.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zd.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://yt.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://rd.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vr.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://tx.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fl.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vb.jianghongdianzi.cn

Go:   encoding/gob
来源：http://if.521024.cn

Ruby: Marshal.dump(obj)
来源：http://vd.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qr.huixinmuqiang.cn

================================================================================
来源：http://nz.lnxyls.cn

L. 网络请求
来源：http://wv.huixiangedu.cn

================================================================================
来源：http://am.nicolike.cn

[L01] 发送 GET 请求
来源：http://gx.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bc.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ts.muxihuayi.cn

JS:   await fetch(url)
来源：http://fj.yuexingan06.cn

TS:   await fetch(url)
来源：http://gz.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ns.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://bo.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vt.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kz.colortex.cn

[L02] 发送 POST JSON
来源：http://fu.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jg.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sv.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ug.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cy.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zp.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ol.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iv.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mg.colortex.cn

[L03] 设置自定义请求头
来源：http://kl.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fc.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ko.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fe.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gs.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ay.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nr.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zp.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gk.muxihuayi.cn

[L04] 设置超时
来源：http://bf.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ih.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cg.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mj.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kc.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mg.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vm.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sn.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://fe.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gv.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vg.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yu.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jx.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fq.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://db.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rj.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ne.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://pa.yuntaijiaju.cn

Py:   resp.json()
来源：http://pg.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://jr.jctech888.com.cn

JS:   await resp.json()
来源：http://xx.hnjuh.cn

TS:   await resp.json()
来源：http://st.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yc.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ar.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://kn.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rb.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://bu.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ny.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oa.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://pq.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://xg.lnxyls.cn

Java: resp.statusCode()
来源：http://xj.shxzskj.cn

Go:   resp.StatusCode
来源：http://ld.nszjky.cn

Ruby: resp.code.to_i
来源：http://hf.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://sk.9csxet.cn

[L08] 并发请求多个地址
来源：http://vn.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cu.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://or.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rc.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lo.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qn.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qp.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://am.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sq.muxihuayi.cn

================================================================================
来源：http://oj.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://uo.szxytkj.cn

================================================================================
来源：http://yp.9csxet.cn

[M01] 读取命令行参数
来源：http://gs.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://bm.nicolike.cn

PHP:  $argv;  $argc;
来源：http://zf.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://ni.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://ts.521024.cn

Java: args 数组（main 方法参数）
来源：http://is.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ks.521024.cn

Ruby: ARGV
来源：http://pl.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://lc.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://jv.521024.cn

Py:   os.environ.get("HOME")
来源：http://nj.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hg.lnxyls.cn

JS:   process.env.HOME
来源：http://xs.asd995.cn

TS:   process.env.HOME
来源：http://ay.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://go.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://in.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ba.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://md.asd995.cn

[M03] 执行外部命令
来源：http://tb.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pt.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gy.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://an.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bv.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fh.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://au.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fm.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://ei.newstarts.cn

[M04] 获取当前工作目录
来源：http://fs.nicolike.cn

Py:   os.getcwd()
来源：http://lb.huixiangedu.cn

PHP:  getcwd();
来源：http://eg.yuntaijiaju.cn

JS:   process.cwd()
来源：http://me.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ke.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://rt.nicolike.cn

Go:   os.Getwd()
来源：http://tm.nicolike.cn

Ruby: Dir.pwd
来源：http://sz.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://km.huanxung.cn

[M05] 设置退出码
来源：http://mm.wgjwhj.cn

Py:   sys.exit(1)
来源：http://sk.newstarts.cn

PHP:  exit(1);
来源：http://dr.huanxung.cn

JS:   process.exit(1)
来源：http://ov.shxzskj.cn

TS:   process.exit(1)
来源：http://qb.wgjwhj.cn

Java: System.exit(1)
来源：http://xj.colortex.cn

Go:   os.Exit(1)
来源：http://pw.nszjky.cn

Ruby: exit 1
来源：http://hq.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sm.nicolike.cn

[M06] 向标准错误输出
来源：http://oh.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://wz.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ec.nicolike.cn

JS:   console.error("err")
来源：http://qs.muxihuayi.cn

TS:   console.error("err")
来源：http://dl.chemitech.net.cn

Java: System.err.println("err")
来源：http://ly.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mn.haigaiapp.cn

Ruby: warn "err"
来源：http://ge.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://yx.asd995.cn

[M07] 判断是否为主入口
来源：http://fz.521024.cn

Py:   if __name__ == "__main__":
来源：http://rr.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bs.huixinmuqiang.cn

JS:   require.main === module
来源：http://wx.newstarts.cn

TS:   require.main === module
来源：http://zf.asd995.cn

Java: public static void main(String[] args)
来源：http://gt.shxzskj.cn

Go:   func main()
来源：http://bh.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://md.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://xj.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://un.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://rm.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://cq.521024.cn

JS:   process.platform;  process.version
来源：http://sr.nicolike.cn

TS:   process.platform;  process.version
来源：http://nf.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gl.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mz.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://io.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aa.hnjuh.cn

================================================================================
来源：http://if.shxzskj.cn

N. 数据结构与算法
来源：http://nq.shxzukj.cn

================================================================================
来源：http://qe.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://sr.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zp.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nk.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cz.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zc.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ex.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://un.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qz.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bm.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://bj.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://uv.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iu.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ah.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uk.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lg.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://ss.huixiangedu.cn

Ruby: arr.sort
来源：http://hg.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pz.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://rp.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pq.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://bx.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uf.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kn.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wy.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qt.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dt.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ui.nszjky.cn

[N04] 斐波那契数列
来源：http://bg.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zt.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hu.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wu.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://se.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xx.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zs.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cm.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gc.bookmarksfly.cn

[N05] 最大公约数
来源：http://lu.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://ck.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vj.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tg.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kx.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zu.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dy.hahajie.cn

Ruby: a.gcd(b)
来源：http://zj.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rr.bjjhwx.cn

[N06] 判断回文字符串
来源：http://zm.szxytkj.cn

Py:   s == s[::-1]
来源：http://cc.9csxet.cn

PHP:  $s === strrev($s);
来源：http://wf.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://gs.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://na.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hi.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://na.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://ih.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oe.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://rx.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zh.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gx.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iz.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://gg.lnxyls.cn

Java: // 手写 HashMap
来源：http://mt.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://sl.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://qg.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mx.chemitech.net.cn

[N08] 生成全排列
来源：http://ta.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://mn.asd995.cn

PHP:  // 手写递归交换
来源：http://pc.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://iu.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://kf.lnxyls.cn

Java: // 手写回溯递归
来源：http://mf.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://oq.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://bb.newstarts.cn

C#:   // 手写回溯递归
来源：http://nj.yuntaijiaju.cn

[N09] 栈与队列
来源：http://ae.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ku.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ns.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ef.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ro.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nf.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dp.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nn.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://by.shtwfgs.cn

[N10] 链表节点定义
来源：http://ya.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ua.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kd.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tl.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qu.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://nc.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ii.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xp.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wg.colortex.cn

[N11] 二叉树中序遍历
来源：http://we.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ro.shxzukj.cn

PHP:  // 手写递归函数
来源：http://co.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://te.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rg.huixiangedu.cn

Java: // 手写递归
来源：http://or.szsharing.cn

Go:   // 手写递归
来源：http://yt.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aj.szsharing.cn

C#:   // 手写递归
来源：http://kk.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zg.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wu.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ag.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ca.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.hahajie.cn


<!-- 参考信息 -->