代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dn.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mb.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nx.lnxyls.cn

[K05] 深拷贝对象
来源：http://jf.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://dj.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://vi.hahajie.cn

JS:   structuredClone(obj)
来源：http://qn.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://eu.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wj.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://in.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ce.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lj.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://pn.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://im.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sk.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ol.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ff.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ld.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ld.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ar.nicolike.cn

[K07] 进制转换
来源：http://ng.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ac.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bp.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ec.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fp.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gf.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kx.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ks.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://uf.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://oo.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dx.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://dz.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://yn.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pf.huixiangedu.cn

Go:   encoding/gob
来源：http://cd.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://fu.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wh.wgjwhj.cn

================================================================================
来源：http://ow.chemitech.net.cn

L. 网络请求
来源：http://tp.nicolike.cn

================================================================================
来源：http://dh.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://di.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vy.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aw.huixiangedu.cn

JS:   await fetch(url)
来源：http://fz.haigaiapp.cn

TS:   await fetch(url)
来源：http://pu.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xp.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://jt.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ci.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ip.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://bb.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gs.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ij.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xi.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yw.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bb.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qy.nicolike.cn

[L03] 设置自定义请求头
来源：http://nt.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ym.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gs.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://da.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vz.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ml.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hc.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://db.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wm.huixiangedu.cn

[L04] 设置超时
来源：http://eh.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://qb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aw.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ox.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xk.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://el.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ww.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sb.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ul.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://eb.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jr.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pj.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mw.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rt.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://af.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ww.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mi.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xm.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://mx.nszjky.cn

Py:   resp.json()
来源：http://ox.asd995.cn

PHP:  json_decode($body, true);
来源：http://yw.newstarts.cn

JS:   await resp.json()
来源：http://ob.muxihuayi.cn

TS:   await resp.json()
来源：http://ge.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wg.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fg.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://bo.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rt.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://nj.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://of.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hm.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://vg.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://fx.bjjhwx.cn

Java: resp.statusCode()
来源：http://te.newstarts.cn

Go:   resp.StatusCode
来源：http://ti.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://vu.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://za.shxzskj.cn

[L08] 并发请求多个地址
来源：http://um.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vc.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://tg.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ox.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gt.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sj.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jl.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uh.bjjhwx.cn

================================================================================
来源：http://yd.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://kg.colortex.cn

================================================================================
来源：http://xr.lnxyls.cn

[M01] 读取命令行参数
来源：http://qy.huanxung.cn

Py:   sys.argv[1:]
来源：http://xo.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://fw.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://bf.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://fx.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://zz.gzmigu.cn

Go:   os.Args[1:]
来源：http://ku.huixinmuqiang.cn

Ruby: ARGV
来源：http://gf.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://lx.panjiajie.cn

[M02] 读取环境变量
来源：http://mo.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://dv.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gt.colortex.cn

JS:   process.env.HOME
来源：http://qz.szsharing.cn

TS:   process.env.HOME
来源：http://uu.hahajie.cn

Java: System.getenv("HOME")
来源：http://ir.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://br.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://zk.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iu.bookmarksfly.cn

[M03] 执行外部命令
来源：http://xl.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://em.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hd.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kx.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wk.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zi.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://on.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ai.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://up.shxzskj.cn

[M04] 获取当前工作目录
来源：http://up.shtwfgs.cn

Py:   os.getcwd()
来源：http://yg.huixiangedu.cn

PHP:  getcwd();
来源：http://kp.wgjwhj.cn

JS:   process.cwd()
来源：http://hq.yuntaijiaju.cn

TS:   process.cwd()
来源：http://pc.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://di.yuexingan06.cn

Go:   os.Getwd()
来源：http://vh.colortex.cn

Ruby: Dir.pwd
来源：http://nn.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tq.9csxet.cn

[M05] 设置退出码
来源：http://nb.9csxet.cn

Py:   sys.exit(1)
来源：http://ng.huanxung.cn

PHP:  exit(1);
来源：http://bc.hahajie.cn

JS:   process.exit(1)
来源：http://ff.szxytkj.cn

TS:   process.exit(1)
来源：http://ae.521024.cn

Java: System.exit(1)
来源：http://go.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://cw.colortex.cn

Ruby: exit 1
来源：http://zn.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://da.szxytkj.cn

[M06] 向标准错误输出
来源：http://yk.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ql.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vb.lnxyls.cn

JS:   console.error("err")
来源：http://bp.9csxet.cn

TS:   console.error("err")
来源：http://rm.colortex.cn

Java: System.err.println("err")
来源：http://ps.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jn.hahajie.cn

Ruby: warn "err"
来源：http://ry.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://yl.nicolike.cn

[M07] 判断是否为主入口
来源：http://in.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://ss.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iu.colortex.cn

JS:   require.main === module
来源：http://jk.huixinmuqiang.cn

TS:   require.main === module
来源：http://hm.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://et.lnxyls.cn

Go:   func main()
来源：http://je.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ur.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://oy.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://rw.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://yg.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://fe.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ej.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://pr.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tf.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://py.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gr.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jn.szsharing.cn

================================================================================
来源：http://eo.huixinmuqiang.cn

N. 数据结构与算法
来源：http://tx.haigaiapp.cn

================================================================================
来源：http://nl.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://rl.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cn.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ze.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mf.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cj.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mc.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://yr.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gf.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tf.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://nh.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lr.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lm.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vr.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cy.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ow.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://wc.huixinmuqiang.cn

Ruby: arr.sort
来源：http://vd.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sj.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://eq.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://th.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://ta.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xd.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tf.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://op.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mk.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rx.gzmigu.cn

[N04] 斐波那契数列
来源：http://wb.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bp.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uk.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mp.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bs.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ru.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ca.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vq.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zl.szxytkj.cn

[N05] 最大公约数
来源：http://rl.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://ir.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nh.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://af.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hd.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ov.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ac.newstarts.cn

Ruby: a.gcd(b)
来源：http://zi.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pk.newstarts.cn

[N06] 判断回文字符串
来源：http://mb.shxzskj.cn

Py:   s == s[::-1]
来源：http://vv.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://rm.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ow.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://qn.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ft.nicolike.cn

Go:   // 双指针从两端比较
来源：http://xz.haigaiapp.cn

Ruby: s == s.reverse
来源：http://ug.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pv.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://cy.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kb.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://od.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ib.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://la.lnxyls.cn

Java: // 手写 HashMap
来源：http://rt.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://lz.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://on.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ne.colortex.cn

[N08] 生成全排列
来源：http://dx.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ya.9csxet.cn

PHP:  // 手写递归交换
来源：http://tn.9csxet.cn

JS:   // 手写回溯递归
来源：http://vk.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://ss.haigaiapp.cn

Java: // 手写回溯递归
来源：http://vs.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://cj.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ud.521024.cn

C#:   // 手写回溯递归
来源：http://vy.gzmigu.cn

[N09] 栈与队列
来源：http://sv.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zy.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eq.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mx.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ay.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jq.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ss.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pw.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xe.nicolike.cn

[N10] 链表节点定义
来源：http://az.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://be.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ss.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qd.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hl.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://ll.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wl.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uw.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ei.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://wp.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yf.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://yz.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ju.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jh.huanxung.cn

Java: // 手写递归
来源：http://wt.asd995.cn

Go:   // 手写递归
来源：http://vx.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rg.521024.cn

C#:   // 手写递归
来源：http://nc.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dt.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zm.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bd.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cw.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tm.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lj.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bm.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hb.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iv.shtwfgs.cn


<!-- 参考信息 -->