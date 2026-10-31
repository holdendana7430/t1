代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wk.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hc.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qx.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://an.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cn.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oe.wgjwhj.cn

[K05] 深拷贝对象
来源：http://mi.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://nv.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ss.colortex.cn

JS:   structuredClone(obj)
来源：http://tv.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://gv.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tr.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gc.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://br.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gc.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://zq.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bq.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xm.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tv.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kj.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oa.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ly.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gy.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://po.nszjky.cn

[K07] 进制转换
来源：http://gb.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mp.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dn.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pc.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bh.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dr.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ez.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xu.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vw.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://lq.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://io.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rr.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://tl.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://jh.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gy.9csxet.cn

Go:   encoding/gob
来源：http://eu.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://bk.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ki.nicolike.cn

================================================================================
来源：http://ri.bookmarksfly.cn

L. 网络请求
来源：http://az.colortex.cn

================================================================================
来源：http://sl.lnxyls.cn

[L01] 发送 GET 请求
来源：http://eh.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ic.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yq.newstarts.cn

JS:   await fetch(url)
来源：http://sq.9csxet.cn

TS:   await fetch(url)
来源：http://wj.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dx.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://qb.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dr.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zo.shxzskj.cn

[L02] 发送 POST JSON
来源：http://cm.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wo.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qc.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ba.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fw.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xa.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://be.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ha.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://eo.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uh.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ug.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uc.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pn.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qu.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ey.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://db.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vg.muxihuayi.cn

[L04] 设置超时
来源：http://lw.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://le.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cj.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ng.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yl.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fh.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://el.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vd.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ho.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hi.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://da.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://av.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ub.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tn.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gb.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ig.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mz.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://kn.yuntaijiaju.cn

Py:   resp.json()
来源：http://eu.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://vv.chemitech.net.cn

JS:   await resp.json()
来源：http://ev.szxytkj.cn

TS:   await resp.json()
来源：http://wh.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ug.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qm.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://sl.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ra.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://mc.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lu.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fy.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://sh.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ey.shxzukj.cn

Java: resp.statusCode()
来源：http://mt.nicolike.cn

Go:   resp.StatusCode
来源：http://ke.shxzukj.cn

Ruby: resp.code.to_i
来源：http://ib.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://gd.newstarts.cn

[L08] 并发请求多个地址
来源：http://cl.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ea.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://pi.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rc.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yq.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lf.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wt.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ww.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oe.szsharing.cn

================================================================================
来源：http://mh.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://bj.nszjky.cn

[M01] 读取命令行参数
来源：http://pc.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://lj.hahajie.cn

PHP:  $argv;  $argc;
来源：http://vz.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://hi.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://vl.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yd.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://dl.9csxet.cn

Ruby: ARGV
来源：http://jq.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://gv.bjjhwx.cn

[M02] 读取环境变量
来源：http://ez.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://sl.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xs.chemitech.net.cn

JS:   process.env.HOME
来源：http://hl.yuexingan06.cn

TS:   process.env.HOME
来源：http://ue.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://zg.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tf.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://qk.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ms.newstarts.cn

[M03] 执行外部命令
来源：http://re.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://on.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://la.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kk.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gb.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yq.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fh.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rr.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ca.nicolike.cn

[M04] 获取当前工作目录
来源：http://tu.wgjwhj.cn

Py:   os.getcwd()
来源：http://og.szsharing.cn

PHP:  getcwd();
来源：http://pt.haigaiapp.cn

JS:   process.cwd()
来源：http://cx.szxytkj.cn

TS:   process.cwd()
来源：http://zx.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://sa.521024.cn

Go:   os.Getwd()
来源：http://yz.haigaiapp.cn

Ruby: Dir.pwd
来源：http://xx.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yb.jctech888.com.cn

[M05] 设置退出码
来源：http://xc.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://jd.szxytkj.cn

PHP:  exit(1);
来源：http://qg.szxytkj.cn

JS:   process.exit(1)
来源：http://ov.huixiangedu.cn

TS:   process.exit(1)
来源：http://ik.9csxet.cn

Java: System.exit(1)
来源：http://ei.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://pm.bjjhwx.cn

Ruby: exit 1
来源：http://no.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wn.shxzskj.cn

[M06] 向标准错误输出
来源：http://wv.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ki.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rx.bookmarksfly.cn

JS:   console.error("err")
来源：http://uk.szxytkj.cn

TS:   console.error("err")
来源：http://uo.yuexingan06.cn

Java: System.err.println("err")
来源：http://ee.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pi.wgjwhj.cn

Ruby: warn "err"
来源：http://tx.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://dy.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://go.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://zd.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://do.muxihuayi.cn

JS:   require.main === module
来源：http://cp.jianghongdianzi.cn

TS:   require.main === module
来源：http://rc.nszjky.cn

Java: public static void main(String[] args)
来源：http://qg.nicolike.cn

Go:   func main()
来源：http://ev.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://px.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://zd.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://ft.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://co.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://px.nszjky.cn

JS:   process.platform;  process.version
来源：http://di.gzmigu.cn

TS:   process.platform;  process.version
来源：http://vh.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bm.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wl.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sh.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qn.panjiajie.cn

================================================================================
来源：http://ys.lnxyls.cn

N. 数据结构与算法
来源：http://ab.yuexingan06.cn

================================================================================
来源：http://ea.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://op.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bt.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://il.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bv.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uf.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dy.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://cm.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mq.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iu.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://od.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vn.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rb.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fq.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dt.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zc.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ng.panjiajie.cn

Ruby: arr.sort
来源：http://tv.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rr.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://ta.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pr.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://th.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rp.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gl.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lt.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sg.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mk.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://am.nicolike.cn

[N04] 斐波那契数列
来源：http://cf.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fx.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mc.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fz.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pv.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ff.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lf.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://in.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bd.yuexingan06.cn

[N05] 最大公约数
来源：http://xq.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://hc.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ck.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://di.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://io.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://to.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gb.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://xr.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jb.panjiajie.cn

[N06] 判断回文字符串
来源：http://qw.lnxyls.cn

Py:   s == s[::-1]
来源：http://zr.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://qt.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://sg.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://cr.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://du.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://jq.szxytkj.cn

Ruby: s == s.reverse
来源：http://pm.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rm.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ve.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://af.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rn.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ci.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ja.colortex.cn

Java: // 手写 HashMap
来源：http://rm.newstarts.cn

Go:   // 手写 map[int]int
来源：http://pr.lnxyls.cn

Ruby: // 手写 Hash
来源：http://as.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mf.lnxyls.cn

[N08] 生成全排列
来源：http://pq.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://xc.huanxung.cn

PHP:  // 手写递归交换
来源：http://nx.szxytkj.cn

JS:   // 手写回溯递归
来源：http://ku.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ku.shtwfgs.cn

Java: // 手写回溯递归
来源：http://vg.9csxet.cn

Go:   // 手写回溯递归
来源：http://jd.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://qa.szsharing.cn

C#:   // 手写回溯递归
来源：http://hn.newstarts.cn

[N09] 栈与队列
来源：http://ma.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ok.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://an.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nu.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nw.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tz.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lh.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://en.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jw.huixiangedu.cn

[N10] 链表节点定义
来源：http://wy.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xh.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mp.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qv.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://af.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://kk.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gw.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://au.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hx.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://kf.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ze.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://na.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://es.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://za.jianghongdianzi.cn

Java: // 手写递归
来源：http://mx.haigaiapp.cn

Go:   // 手写递归
来源：http://wz.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pz.shxzskj.cn

C#:   // 手写递归
来源：http://le.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mo.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qc.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bh.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nv.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wk.wgjwhj.cn


<!-- 参考信息 -->