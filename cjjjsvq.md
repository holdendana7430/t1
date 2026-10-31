代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://va.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uh.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://hn.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zy.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hh.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nc.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dm.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://be.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wz.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://da.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bt.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ka.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://mt.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://xt.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://tt.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://go.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ou.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wz.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bs.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ad.hahajie.cn

[K06] 解析 URL 查询串
来源：http://fk.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uf.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fd.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pg.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://br.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yw.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vb.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hy.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qt.gzmigu.cn

[K07] 进制转换
来源：http://cv.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gb.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vq.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yw.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://su.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nv.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gn.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hl.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ib.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://lr.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://dc.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pq.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ti.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://cr.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gc.szsharing.cn

Go:   encoding/gob
来源：http://ab.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://nw.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aw.yuexingan06.cn

================================================================================
来源：http://ye.chemitech.net.cn

L. 网络请求
来源：http://un.hahajie.cn

================================================================================
来源：http://xb.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://va.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ov.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://id.huanxung.cn

JS:   await fetch(url)
来源：http://me.asd995.cn

TS:   await fetch(url)
来源：http://ht.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kt.521024.cn

Go:   resp, err := http.Get(url)
来源：http://di.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jx.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fx.panjiajie.cn

[L02] 发送 POST JSON
来源：http://ag.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zh.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uf.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bt.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ar.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bv.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kv.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jd.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://bo.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hx.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lg.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wu.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qw.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gc.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mg.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ba.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://re.bookmarksfly.cn

[L04] 设置超时
来源：http://ez.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://li.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lz.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hj.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gs.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rz.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ek.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mb.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wm.nszjky.cn

[L05] 上传文件（multipart）
来源：http://md.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sv.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sz.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oi.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wd.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ro.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nv.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ly.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hq.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://nv.521024.cn

Py:   resp.json()
来源：http://hk.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://yc.newstarts.cn

JS:   await resp.json()
来源：http://gr.hahajie.cn

TS:   await resp.json()
来源：http://px.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vd.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kx.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://wv.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gi.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://kj.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ya.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qj.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://bh.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://nn.nicolike.cn

Java: resp.statusCode()
来源：http://hf.muxihuayi.cn

Go:   resp.StatusCode
来源：http://yz.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://fr.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://nq.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ds.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mc.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://hj.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qh.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pp.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bv.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vs.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ek.huixinmuqiang.cn

================================================================================
来源：http://ts.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://tj.shtwfgs.cn

================================================================================
来源：http://re.szsharing.cn

[M01] 读取命令行参数
来源：http://ou.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://hi.521024.cn

PHP:  $argv;  $argc;
来源：http://ja.nszjky.cn

JS:   process.argv.slice(2)
来源：http://sz.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://cc.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://rs.lnxyls.cn

Go:   os.Args[1:]
来源：http://th.bjjhwx.cn

Ruby: ARGV
来源：http://og.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://yq.hnjuh.cn

[M02] 读取环境变量
来源：http://dn.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ao.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nx.shtwfgs.cn

JS:   process.env.HOME
来源：http://hp.colortex.cn

TS:   process.env.HOME
来源：http://uw.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://cg.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lr.hahajie.cn

Ruby: ENV["HOME"]
来源：http://de.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jm.shxzskj.cn

[M03] 执行外部命令
来源：http://ec.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gx.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ru.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cc.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wt.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hq.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gi.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://au.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://wd.9csxet.cn

[M04] 获取当前工作目录
来源：http://oy.szsharing.cn

Py:   os.getcwd()
来源：http://wf.nicolike.cn

PHP:  getcwd();
来源：http://ss.bookmarksfly.cn

JS:   process.cwd()
来源：http://zq.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ja.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://fh.nicolike.cn

Go:   os.Getwd()
来源：http://fy.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://zc.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ef.chemitech.net.cn

[M05] 设置退出码
来源：http://nf.yuexingan06.cn

Py:   sys.exit(1)
来源：http://uo.szsharing.cn

PHP:  exit(1);
来源：http://qp.huanxung.cn

JS:   process.exit(1)
来源：http://ry.huixiangedu.cn

TS:   process.exit(1)
来源：http://uy.9csxet.cn

Java: System.exit(1)
来源：http://zv.jctech888.com.cn

Go:   os.Exit(1)
来源：http://pr.colortex.cn

Ruby: exit 1
来源：http://du.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://th.gzmigu.cn

[M06] 向标准错误输出
来源：http://sw.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://gi.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xw.bookmarksfly.cn

JS:   console.error("err")
来源：http://uf.huixinmuqiang.cn

TS:   console.error("err")
来源：http://ta.asd995.cn

Java: System.err.println("err")
来源：http://bu.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gh.nicolike.cn

Ruby: warn "err"
来源：http://ao.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ik.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://ln.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://qj.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://do.nicolike.cn

JS:   require.main === module
来源：http://wt.szsharing.cn

TS:   require.main === module
来源：http://xf.szsharing.cn

Java: public static void main(String[] args)
来源：http://nq.asd995.cn

Go:   func main()
来源：http://yn.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qu.hahajie.cn

C#:   static void Main(string[] args)
来源：http://rz.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://yv.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://oa.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://uv.hnjuh.cn

JS:   process.platform;  process.version
来源：http://lm.newstarts.cn

TS:   process.platform;  process.version
来源：http://rj.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xg.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://px.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://op.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xq.szsharing.cn

================================================================================
来源：http://rv.yuntaijiaju.cn

N. 数据结构与算法
来源：http://uq.chemitech.net.cn

================================================================================
来源：http://cd.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://zw.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ug.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lo.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hg.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tx.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lo.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://sp.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wg.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qk.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://tx.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://uw.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://as.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ol.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fn.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dl.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://du.colortex.cn

Ruby: arr.sort
来源：http://sm.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rb.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://mv.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ar.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://js.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ym.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qd.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://af.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rp.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zl.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vy.hnjuh.cn

[N04] 斐波那契数列
来源：http://du.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tm.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cr.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rj.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://as.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rr.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iv.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tr.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://de.wgjwhj.cn

[N05] 最大公约数
来源：http://ja.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://qj.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jk.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://il.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dm.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xh.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://mf.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zf.newstarts.cn

[N06] 判断回文字符串
来源：http://sz.szxytkj.cn

Py:   s == s[::-1]
来源：http://cy.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://qv.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://fc.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://vm.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ev.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://gj.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://ke.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hw.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://uf.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eh.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ih.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hl.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://uu.chemitech.net.cn

Java: // 手写 HashMap
来源：http://lv.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://qj.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://fb.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kq.szxytkj.cn

[N08] 生成全排列
来源：http://mu.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://mv.huanxung.cn

PHP:  // 手写递归交换
来源：http://fn.nicolike.cn

JS:   // 手写回溯递归
来源：http://nl.shxzskj.cn

TS:   // 手写回溯递归
来源：http://jy.chemitech.net.cn

Java: // 手写回溯递归
来源：http://nz.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://rv.521024.cn

Ruby: arr.permutation.to_a
来源：http://un.9csxet.cn

C#:   // 手写回溯递归
来源：http://zs.muxihuayi.cn

[N09] 栈与队列
来源：http://jm.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bb.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zq.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ra.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jt.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lg.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mx.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zx.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gh.gzmigu.cn

[N10] 链表节点定义
来源：http://qa.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ey.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ec.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://et.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fd.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://yk.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xk.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ff.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zb.nszjky.cn

[N11] 二叉树中序遍历
来源：http://tu.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zt.panjiajie.cn

PHP:  // 手写递归函数
来源：http://cv.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eq.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://of.9csxet.cn

Java: // 手写递归
来源：http://na.newstarts.cn

Go:   // 手写递归
来源：http://dt.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rs.jctech888.com.cn

C#:   // 手写递归
来源：http://wy.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eu.nicolike.cn


<!-- 参考信息 -->