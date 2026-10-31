代发 wailian999

TS:   JSON.parse(s)
来源：http://sw.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xx.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://zd.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://pw.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jw.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://sh.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vz.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mx.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yq.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cc.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qy.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gc.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lu.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tr.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ol.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wc.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tc.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jm.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://js.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bd.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mu.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ix.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vb.yuexingan06.cn

[K05] 深拷贝对象
来源：http://ni.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://wk.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://sk.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://qm.hahajie.cn

TS:   structuredClone(obj)
来源：http://dk.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ph.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ax.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cn.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://me.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://oq.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tf.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eb.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://to.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bn.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mh.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tx.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ey.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cg.huixinmuqiang.cn

[K07] 进制转换
来源：http://ip.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ba.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tx.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ma.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ca.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jj.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fw.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ea.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cz.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ae.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://ky.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ml.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://zg.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ou.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ck.jctech888.com.cn

Go:   encoding/gob
来源：http://qo.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://lj.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://du.panjiajie.cn

================================================================================
来源：http://wg.panjiajie.cn

L. 网络请求
来源：http://lb.newstarts.cn

================================================================================
来源：http://ht.shxzukj.cn

[L01] 发送 GET 请求
来源：http://uo.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ap.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dp.szxytkj.cn

JS:   await fetch(url)
来源：http://yn.nszjky.cn

TS:   await fetch(url)
来源：http://vj.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wj.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://jl.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fv.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pe.521024.cn

[L02] 发送 POST JSON
来源：http://bz.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ye.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://di.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jg.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://au.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kx.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lq.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lh.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oy.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://uj.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fj.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wc.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qu.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ma.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dp.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ek.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ii.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fk.huixiangedu.cn

[L04] 设置超时
来源：http://dv.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://su.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rb.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kv.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zw.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sy.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pr.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xi.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ic.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bq.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ky.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qh.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fg.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://it.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zr.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vr.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zf.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://rb.szxytkj.cn

Py:   resp.json()
来源：http://xk.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://nq.yuntaijiaju.cn

JS:   await resp.json()
来源：http://tn.yuntaijiaju.cn

TS:   await resp.json()
来源：http://pv.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://id.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ir.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ds.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://io.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://gd.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pj.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hg.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://iz.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://qd.bjjhwx.cn

Java: resp.statusCode()
来源：http://jj.shtwfgs.cn

Go:   resp.StatusCode
来源：http://mv.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ka.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://zy.asd995.cn

[L08] 并发请求多个地址
来源：http://zs.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oo.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://bz.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eq.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xg.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mm.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sq.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sd.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wi.jianghongdianzi.cn

================================================================================
来源：http://xs.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://pt.jianghongdianzi.cn

================================================================================
来源：http://ep.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://om.9csxet.cn

Py:   sys.argv[1:]
来源：http://lu.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://gr.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://ky.nicolike.cn

TS:   process.argv.slice(2)
来源：http://il.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://vb.hahajie.cn

Go:   os.Args[1:]
来源：http://lg.muxihuayi.cn

Ruby: ARGV
来源：http://ev.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ro.521024.cn

[M02] 读取环境变量
来源：http://nf.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://vf.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ob.huixiangedu.cn

JS:   process.env.HOME
来源：http://mh.bookmarksfly.cn

TS:   process.env.HOME
来源：http://nx.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://hk.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bz.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://tw.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ad.521024.cn

[M03] 执行外部命令
来源：http://uy.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xa.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oh.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yk.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jl.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oq.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ao.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fu.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://wi.nicolike.cn

[M04] 获取当前工作目录
来源：http://pn.shxzskj.cn

Py:   os.getcwd()
来源：http://zd.bookmarksfly.cn

PHP:  getcwd();
来源：http://zp.szsharing.cn

JS:   process.cwd()
来源：http://cw.521024.cn

TS:   process.cwd()
来源：http://ic.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://vu.hnjuh.cn

Go:   os.Getwd()
来源：http://br.haigaiapp.cn

Ruby: Dir.pwd
来源：http://yq.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ug.haigaiapp.cn

[M05] 设置退出码
来源：http://qb.hahajie.cn

Py:   sys.exit(1)
来源：http://xv.lnxyls.cn

PHP:  exit(1);
来源：http://ej.haigaiapp.cn

JS:   process.exit(1)
来源：http://my.huixiangedu.cn

TS:   process.exit(1)
来源：http://mb.huanxung.cn

Java: System.exit(1)
来源：http://mz.521024.cn

Go:   os.Exit(1)
来源：http://ei.szxytkj.cn

Ruby: exit 1
来源：http://fi.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fr.haigaiapp.cn

[M06] 向标准错误输出
来源：http://ik.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://ja.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eb.nicolike.cn

JS:   console.error("err")
来源：http://oo.muxihuayi.cn

TS:   console.error("err")
来源：http://qy.newstarts.cn

Java: System.err.println("err")
来源：http://jl.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://po.nicolike.cn

Ruby: warn "err"
来源：http://nl.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://ly.newstarts.cn

[M07] 判断是否为主入口
来源：http://gj.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://bp.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ya.wgjwhj.cn

JS:   require.main === module
来源：http://eb.shxzskj.cn

TS:   require.main === module
来源：http://cr.newstarts.cn

Java: public static void main(String[] args)
来源：http://xo.asd995.cn

Go:   func main()
来源：http://qs.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cu.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://uh.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://zo.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://be.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ns.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ds.shxzukj.cn

TS:   process.platform;  process.version
来源：http://sh.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hy.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kb.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fx.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ai.bookmarksfly.cn

================================================================================
来源：http://dj.bjjhwx.cn

N. 数据结构与算法
来源：http://gs.haigaiapp.cn

================================================================================
来源：http://ca.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://df.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://up.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nw.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gi.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lm.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zo.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://iz.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://su.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bi.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://gu.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://wl.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cm.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mr.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hy.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hc.asd995.cn

Go:   slices.Sort(arr)
来源：http://rw.wgjwhj.cn

Ruby: arr.sort
来源：http://hr.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ky.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://bj.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sa.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://jh.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://db.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yo.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lo.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hh.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xf.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://to.yuexingan06.cn

[N04] 斐波那契数列
来源：http://uo.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yl.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wc.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qc.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zo.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://co.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cb.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ec.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ko.panjiajie.cn

[N05] 最大公约数
来源：http://eh.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://qo.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bd.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xs.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qz.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fs.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kv.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://gs.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ly.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://rq.9csxet.cn

Py:   s == s[::-1]
来源：http://jh.szsharing.cn

PHP:  $s === strrev($s);
来源：http://mg.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://wc.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://wa.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wf.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://cu.nicolike.cn

Ruby: s == s.reverse
来源：http://zq.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kz.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://tf.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ey.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xf.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vf.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://ap.huanxung.cn

Java: // 手写 HashMap
来源：http://rx.szsharing.cn

Go:   // 手写 map[int]int
来源：http://bd.nszjky.cn

Ruby: // 手写 Hash
来源：http://su.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jc.shxzskj.cn

[N08] 生成全排列
来源：http://jm.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ds.shxzskj.cn

PHP:  // 手写递归交换
来源：http://qg.colortex.cn

JS:   // 手写回溯递归
来源：http://dy.gzmigu.cn

TS:   // 手写回溯递归
来源：http://wq.shxzskj.cn

Java: // 手写回溯递归
来源：http://so.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://ou.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://qr.shxzskj.cn

C#:   // 手写回溯递归
来源：http://hk.szsharing.cn

[N09] 栈与队列
来源：http://my.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ji.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sf.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cq.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zt.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mc.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sp.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kj.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ae.shtwfgs.cn

[N10] 链表节点定义
来源：http://fk.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nu.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ym.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ui.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ap.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://ot.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://em.newstarts.cn


<!-- 参考信息 -->