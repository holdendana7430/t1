代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://op.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ld.nicolike.cn

[K04] 读取 JSON 文件
来源：http://vs.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wo.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ww.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zi.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://an.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vr.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rr.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zh.wgjwhj.cn

[K05] 深拷贝对象
来源：http://aa.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ao.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://cd.hahajie.cn

JS:   structuredClone(obj)
来源：http://ci.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ch.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qo.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bv.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://es.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://on.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://jp.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sb.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yn.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gv.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dr.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sr.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kp.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://da.hahajie.cn

[K07] 进制转换
来源：http://oh.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uv.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bf.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ry.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vr.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dk.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jm.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pj.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hg.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://ir.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://db.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ja.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://up.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://dx.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://or.haigaiapp.cn

Go:   encoding/gob
来源：http://uv.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://vv.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qx.wgjwhj.cn

================================================================================
来源：http://jw.huanxung.cn

L. 网络请求
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://ej.nszjky.cn

[L01] 发送 GET 请求
来源：http://wa.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yk.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ws.shxzukj.cn

JS:   await fetch(url)
来源：http://ix.nszjky.cn

TS:   await fetch(url)
来源：http://zm.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://he.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://is.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sy.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dd.szxytkj.cn

[L02] 发送 POST JSON
来源：http://bd.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wo.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ko.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rs.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jf.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mh.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qf.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pp.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rs.newstarts.cn

[L03] 设置自定义请求头
来源：http://by.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yx.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hf.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zj.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kv.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sq.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hk.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qc.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ij.newstarts.cn

[L04] 设置超时
来源：http://og.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://zr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kz.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wp.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bb.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pw.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://km.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://om.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sz.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://ef.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dl.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ze.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ep.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rz.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kh.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eo.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://na.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rk.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://wl.chemitech.net.cn

Py:   resp.json()
来源：http://du.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://fp.szxytkj.cn

JS:   await resp.json()
来源：http://ur.panjiajie.cn

TS:   await resp.json()
来源：http://ux.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qg.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://md.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://ir.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zn.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://fy.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ar.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lw.colortex.cn

JS:   resp.ok;  resp.status
来源：http://aa.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://wa.shtwfgs.cn

Java: resp.statusCode()
来源：http://id.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://rk.hahajie.cn

Ruby: resp.code.to_i
来源：http://ty.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://fe.nicolike.cn

[L08] 并发请求多个地址
来源：http://jf.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jt.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://kj.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vy.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yd.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wb.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ts.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bo.hnjuh.cn

================================================================================
来源：http://bw.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://tk.shtwfgs.cn

================================================================================
来源：http://xn.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://st.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://ia.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://mx.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://jr.nicolike.cn

TS:   process.argv.slice(2)
来源：http://rw.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://zs.szxytkj.cn

Go:   os.Args[1:]
来源：http://an.jctech888.com.cn

Ruby: ARGV
来源：http://iu.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ku.9csxet.cn

[M02] 读取环境变量
来源：http://et.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://dx.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yx.huixiangedu.cn

JS:   process.env.HOME
来源：http://rh.bookmarksfly.cn

TS:   process.env.HOME
来源：http://vl.colortex.cn

Java: System.getenv("HOME")
来源：http://mz.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vo.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://hv.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fl.muxihuayi.cn

[M03] 执行外部命令
来源：http://jv.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cg.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lq.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jp.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mz.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yu.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lz.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wm.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://bz.szsharing.cn

[M04] 获取当前工作目录
来源：http://ee.nicolike.cn

Py:   os.getcwd()
来源：http://hs.shxzukj.cn

PHP:  getcwd();
来源：http://vg.nicolike.cn

JS:   process.cwd()
来源：http://dh.bookmarksfly.cn

TS:   process.cwd()
来源：http://ja.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://jl.hahajie.cn

Go:   os.Getwd()
来源：http://ku.muxihuayi.cn

Ruby: Dir.pwd
来源：http://co.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tf.shxzukj.cn

[M05] 设置退出码
来源：http://jp.shxzukj.cn

Py:   sys.exit(1)
来源：http://pf.asd995.cn

PHP:  exit(1);
来源：http://bm.szsharing.cn

JS:   process.exit(1)
来源：http://vf.muxihuayi.cn

TS:   process.exit(1)
来源：http://cn.hnjuh.cn

Java: System.exit(1)
来源：http://bo.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://xu.huanxung.cn

Ruby: exit 1
来源：http://qo.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oy.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://vx.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://cf.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hi.jctech888.com.cn

JS:   console.error("err")
来源：http://cz.jctech888.com.cn

TS:   console.error("err")
来源：http://jx.szxytkj.cn

Java: System.err.println("err")
来源：http://xq.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://md.shxzukj.cn

Ruby: warn "err"
来源：http://ym.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://bh.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://ar.asd995.cn

Py:   if __name__ == "__main__":
来源：http://fl.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vh.gzmigu.cn

JS:   require.main === module
来源：http://yg.9csxet.cn

TS:   require.main === module
来源：http://sx.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://wi.shxzskj.cn

Go:   func main()
来源：http://wm.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hf.asd995.cn

C#:   static void Main(string[] args)
来源：http://dv.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://nk.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://cg.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://bs.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ym.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://lc.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gu.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yz.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://al.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yy.9csxet.cn

================================================================================
来源：http://gd.asd995.cn

N. 数据结构与算法
来源：http://xa.9csxet.cn

================================================================================
来源：http://me.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://fh.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iy.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xj.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://th.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sk.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fk.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://rj.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jd.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wn.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://yr.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://hr.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rv.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fn.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rx.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://am.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ru.asd995.cn

Ruby: arr.sort
来源：http://ih.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mi.521024.cn

[N03] 快速排序（分治示例）
来源：http://tf.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gc.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://tr.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qn.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bf.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tw.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://po.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://is.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qy.nszjky.cn

[N04] 斐波那契数列
来源：http://xv.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ej.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ei.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kk.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ry.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ci.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bp.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gx.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fv.jianghongdianzi.cn

[N05] 最大公约数
来源：http://fr.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ba.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ic.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rb.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ea.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nc.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ys.gzmigu.cn

Ruby: a.gcd(b)
来源：http://vr.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fe.jctech888.com.cn

[N06] 判断回文字符串
来源：http://di.wgjwhj.cn

Py:   s == s[::-1]
来源：http://on.newstarts.cn

PHP:  $s === strrev($s);
来源：http://jp.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ww.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://sm.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xt.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://tb.hnjuh.cn

Ruby: s == s.reverse
来源：http://qt.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://se.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://ih.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gv.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cz.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://he.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://mc.shtwfgs.cn

Java: // 手写 HashMap
来源：http://da.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://ye.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://zc.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rn.huixinmuqiang.cn

[N08] 生成全排列
来源：http://aw.521024.cn

Py:   itertools.permutations(arr)
来源：http://ct.gzmigu.cn

PHP:  // 手写递归交换
来源：http://tl.nszjky.cn

JS:   // 手写回溯递归
来源：http://ia.9csxet.cn

TS:   // 手写回溯递归
来源：http://op.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://al.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://oi.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://sg.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://qt.szsharing.cn

[N09] 栈与队列
来源：http://ep.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cm.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ii.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oo.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ic.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yq.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jc.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ok.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.yuexingan06.cn

[N10] 链表节点定义
来源：http://pz.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://na.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://im.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lv.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xq.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://jt.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gl.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ds.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sr.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://bj.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://el.shxzskj.cn

PHP:  // 手写递归函数
来源：http://pn.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sc.hnjuh.cn

Java: // 手写递归
来源：http://uh.nszjky.cn

Go:   // 手写递归
来源：http://tu.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qj.panjiajie.cn

C#:   // 手写递归
来源：http://sd.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjjhwx.cn


<!-- 参考信息 -->