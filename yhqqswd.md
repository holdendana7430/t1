代发 wailian999

[K02] JSON 字符串转对象
来源：http://ob.shxzskj.cn

Py:   json.loads(s)
来源：http://dv.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mb.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://vc.colortex.cn

TS:   JSON.parse(s)
来源：http://oj.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hn.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://yn.nicolike.cn

Ruby: JSON.parse(s)
来源：http://cr.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sc.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ia.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rk.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bt.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tv.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hp.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hp.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kh.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hm.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fr.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://gc.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ho.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qa.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qt.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tb.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xm.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yr.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xt.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yk.panjiajie.cn

[K05] 深拷贝对象
来源：http://zz.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://go.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://rj.szxytkj.cn

JS:   structuredClone(obj)
来源：http://zc.nicolike.cn

TS:   structuredClone(obj)
来源：http://zn.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qg.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://na.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ij.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bd.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://an.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mj.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vu.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dc.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hm.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sz.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xl.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ji.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qx.haigaiapp.cn

[K07] 进制转换
来源：http://xb.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ru.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eb.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jv.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cq.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cz.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jg.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mb.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oq.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://xo.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://ik.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iq.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://bu.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://dz.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qg.521024.cn

Go:   encoding/gob
来源：http://kx.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://au.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ga.huanxung.cn

================================================================================
来源：http://mu.yuntaijiaju.cn

L. 网络请求
来源：http://rv.szsharing.cn

================================================================================
来源：http://mv.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://nt.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://px.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hq.colortex.cn

JS:   await fetch(url)
来源：http://ze.panjiajie.cn

TS:   await fetch(url)
来源：http://jc.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cz.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://tj.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qc.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ld.nszjky.cn

[L02] 发送 POST JSON
来源：http://mi.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fa.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ak.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fv.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ki.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://em.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tf.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vz.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://tu.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://al.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rn.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sz.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rd.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jc.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fp.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://px.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://js.9csxet.cn

[L04] 设置超时
来源：http://wh.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://yx.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://or.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qd.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wd.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xh.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kw.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bt.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ja.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://bh.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ou.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fi.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iu.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fo.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ct.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lo.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mc.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rc.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://dh.shxzukj.cn

Py:   resp.json()
来源：http://qj.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://zr.bookmarksfly.cn

JS:   await resp.json()
来源：http://mp.hnjuh.cn

TS:   await resp.json()
来源：http://ud.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oq.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qw.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://jq.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://op.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://np.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jx.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qw.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://em.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://bl.chemitech.net.cn

Java: resp.statusCode()
来源：http://li.haigaiapp.cn

Go:   resp.StatusCode
来源：http://dm.nszjky.cn

Ruby: resp.code.to_i
来源：http://wi.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://qx.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://os.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ud.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ts.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uy.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kp.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ge.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uf.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rj.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cr.huanxung.cn

================================================================================
来源：http://im.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://lr.yuexingan06.cn

================================================================================
来源：http://mj.huanxung.cn

[M01] 读取命令行参数
来源：http://ny.gzmigu.cn

Py:   sys.argv[1:]
来源：http://wv.hahajie.cn

PHP:  $argv;  $argc;
来源：http://qd.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://ct.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://gr.colortex.cn

Java: args 数组（main 方法参数）
来源：http://ba.gzmigu.cn

Go:   os.Args[1:]
来源：http://ni.jianghongdianzi.cn

Ruby: ARGV
来源：http://oz.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://is.521024.cn

[M02] 读取环境变量
来源：http://iu.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://gi.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wi.colortex.cn

JS:   process.env.HOME
来源：http://so.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://fc.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://ow.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oh.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://cl.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zc.newstarts.cn

[M03] 执行外部命令
来源：http://ov.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qb.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ci.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wy.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mt.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pk.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nh.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lw.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://qf.asd995.cn

[M04] 获取当前工作目录
来源：http://zm.jctech888.com.cn

Py:   os.getcwd()
来源：http://yk.yuntaijiaju.cn

PHP:  getcwd();
来源：http://cx.hahajie.cn

JS:   process.cwd()
来源：http://wg.9csxet.cn

TS:   process.cwd()
来源：http://yj.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://zm.gzmigu.cn

Go:   os.Getwd()
来源：http://ic.panjiajie.cn

Ruby: Dir.pwd
来源：http://rp.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://av.szxytkj.cn

[M05] 设置退出码
来源：http://xq.szsharing.cn

Py:   sys.exit(1)
来源：http://ly.newstarts.cn

PHP:  exit(1);
来源：http://ex.shxzskj.cn

JS:   process.exit(1)
来源：http://xk.panjiajie.cn

TS:   process.exit(1)
来源：http://eb.9csxet.cn

Java: System.exit(1)
来源：http://rq.colortex.cn

Go:   os.Exit(1)
来源：http://rt.shtwfgs.cn

Ruby: exit 1
来源：http://ox.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://we.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://br.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://be.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yu.yuexingan06.cn

JS:   console.error("err")
来源：http://po.shxzskj.cn

TS:   console.error("err")
来源：http://cj.lnxyls.cn

Java: System.err.println("err")
来源：http://ja.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ur.colortex.cn

Ruby: warn "err"
来源：http://lg.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://fx.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://sj.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://wu.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wq.colortex.cn

JS:   require.main === module
来源：http://rq.nicolike.cn

TS:   require.main === module
来源：http://gw.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://vz.hahajie.cn

Go:   func main()
来源：http://vi.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tk.colortex.cn

C#:   static void Main(string[] args)
来源：http://es.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://qr.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://oq.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://jm.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://rn.shxzukj.cn

TS:   process.platform;  process.version
来源：http://rc.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xi.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://td.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vi.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ou.huixiangedu.cn

================================================================================
来源：http://sm.jctech888.com.cn

N. 数据结构与算法
来源：http://xn.lnxyls.cn

================================================================================
来源：http://hv.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://km.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pn.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pr.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vv.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yz.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eh.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://vo.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aq.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cz.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ap.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ud.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://el.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wq.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qf.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xt.9csxet.cn

Go:   slices.Sort(arr)
来源：http://qs.bookmarksfly.cn

Ruby: arr.sort
来源：http://jr.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lr.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://sx.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kx.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://kp.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://im.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bx.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aq.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yl.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pg.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ph.wgjwhj.cn

[N04] 斐波那契数列
来源：http://qy.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ab.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kw.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wa.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pn.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hr.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yw.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fo.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gj.yuntaijiaju.cn

[N05] 最大公约数
来源：http://aq.szsharing.cn

Py:   math.gcd(a, b)
来源：http://bx.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mq.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hf.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ng.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fh.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rk.nicolike.cn

Ruby: a.gcd(b)
来源：http://ih.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vz.muxihuayi.cn

[N06] 判断回文字符串
来源：http://zp.hahajie.cn

Py:   s == s[::-1]
来源：http://sa.newstarts.cn

PHP:  $s === strrev($s);
来源：http://pu.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://kx.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://zt.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dz.szsharing.cn

Go:   // 双指针从两端比较
来源：http://ih.newstarts.cn

Ruby: s == s.reverse
来源：http://ph.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eh.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://cl.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xd.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://br.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rm.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://wc.gzmigu.cn

Java: // 手写 HashMap
来源：http://pq.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://jb.nszjky.cn

Ruby: // 手写 Hash
来源：http://ge.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rl.9csxet.cn

[N08] 生成全排列
来源：http://vk.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://cf.shxzukj.cn

PHP:  // 手写递归交换
来源：http://lu.szsharing.cn

JS:   // 手写回溯递归
来源：http://cj.lnxyls.cn

TS:   // 手写回溯递归
来源：http://jv.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://lk.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://zo.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://dt.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://up.chemitech.net.cn

[N09] 栈与队列
来源：http://vl.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dy.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vw.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jk.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yd.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zd.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mz.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ld.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ai.shxzukj.cn

[N10] 链表节点定义
来源：http://nm.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kk.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cf.yuexingan06.cn


<!-- 参考信息 -->