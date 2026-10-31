代发 wailian999

TS:   JSON.parse(s)
来源：http://cw.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://th.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://vo.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://lw.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nt.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://eu.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yt.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ot.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iq.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eg.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kz.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tm.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xt.521024.cn

[K04] 读取 JSON 文件
来源：http://sp.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://no.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tj.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cq.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wh.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mm.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pf.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nf.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tv.haigaiapp.cn

[K05] 深拷贝对象
来源：http://te.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://pc.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://uo.shxzskj.cn

JS:   structuredClone(obj)
来源：http://vn.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://rm.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://px.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tv.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sg.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fx.huanxung.cn

[K06] 解析 URL 查询串
来源：http://hp.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fn.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zp.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iy.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fj.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ap.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kt.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gi.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ty.panjiajie.cn

[K07] 进制转换
来源：http://ls.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dw.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eb.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ux.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wa.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ek.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qc.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xa.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jh.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://yi.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://gg.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://br.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://or.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://uh.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ly.521024.cn

Go:   encoding/gob
来源：http://nf.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://bn.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qc.huanxung.cn

================================================================================
来源：http://xu.newstarts.cn

L. 网络请求
来源：http://mv.szsharing.cn

================================================================================
来源：http://vn.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://jy.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ow.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://os.jctech888.com.cn

JS:   await fetch(url)
来源：http://pe.huixiangedu.cn

TS:   await fetch(url)
来源：http://ok.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jn.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://dg.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tx.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rb.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://mk.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fr.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wu.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ja.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gt.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://km.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jq.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ri.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jv.nszjky.cn

[L03] 设置自定义请求头
来源：http://rd.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fm.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fw.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ik.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kb.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yc.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oi.shtwfgs.cn

[L04] 设置超时
来源：http://nn.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://du.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://af.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wa.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://un.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ha.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ni.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ex.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jw.521024.cn

[L05] 上传文件（multipart）
来源：http://xf.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ct.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ub.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xj.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ag.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zr.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eh.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iq.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jc.colortex.cn

[L06] 解析响应为 JSON
来源：http://nf.newstarts.cn

Py:   resp.json()
来源：http://tg.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://en.521024.cn

JS:   await resp.json()
来源：http://de.lnxyls.cn

TS:   await resp.json()
来源：http://kj.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qy.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://xp.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wk.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://rx.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vw.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hv.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://gp.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://jb.bjjhwx.cn

Java: resp.statusCode()
来源：http://qn.jctech888.com.cn

Go:   resp.StatusCode
来源：http://vj.gzmigu.cn

Ruby: resp.code.to_i
来源：http://wu.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://cq.asd995.cn

[L08] 并发请求多个地址
来源：http://zf.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kf.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://tg.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nm.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ha.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yq.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vx.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ws.wgjwhj.cn

================================================================================
来源：http://wg.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://aw.jctech888.com.cn

================================================================================
来源：http://wm.huanxung.cn

[M01] 读取命令行参数
来源：http://hx.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://rg.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://rx.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ty.521024.cn

TS:   process.argv.slice(2)
来源：http://vj.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://wx.asd995.cn

Go:   os.Args[1:]
来源：http://oh.jianghongdianzi.cn

Ruby: ARGV
来源：http://bp.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://oc.521024.cn

[M02] 读取环境变量
来源：http://yr.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://vc.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sj.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://dg.newstarts.cn

TS:   process.env.HOME
来源：http://uw.shxzukj.cn

Java: System.getenv("HOME")
来源：http://ri.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ns.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://hj.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pv.hnjuh.cn

[M03] 执行外部命令
来源：http://sh.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yw.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jy.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cm.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vz.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wr.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ru.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qq.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://tz.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://uy.newstarts.cn

Py:   os.getcwd()
来源：http://nn.nszjky.cn

PHP:  getcwd();
来源：http://ur.gzmigu.cn

JS:   process.cwd()
来源：http://pz.shxzukj.cn

TS:   process.cwd()
来源：http://qv.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://vs.hahajie.cn

Go:   os.Getwd()
来源：http://eq.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://fw.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wa.jianghongdianzi.cn

[M05] 设置退出码
来源：http://yn.huixiangedu.cn

Py:   sys.exit(1)
来源：http://ni.huixinmuqiang.cn

PHP:  exit(1);
来源：http://gn.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://bm.lnxyls.cn

TS:   process.exit(1)
来源：http://xp.hnjuh.cn

Java: System.exit(1)
来源：http://zi.haigaiapp.cn

Go:   os.Exit(1)
来源：http://vi.wgjwhj.cn

Ruby: exit 1
来源：http://fs.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gs.bjjhwx.cn

[M06] 向标准错误输出
来源：http://tp.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://fc.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ez.huanxung.cn

JS:   console.error("err")
来源：http://ib.521024.cn

TS:   console.error("err")
来源：http://xd.szsharing.cn

Java: System.err.println("err")
来源：http://id.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rc.hnjuh.cn

Ruby: warn "err"
来源：http://yi.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://za.colortex.cn

[M07] 判断是否为主入口
来源：http://xx.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://fg.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dy.szxytkj.cn

JS:   require.main === module
来源：http://yj.jianghongdianzi.cn

TS:   require.main === module
来源：http://lu.szxytkj.cn

Java: public static void main(String[] args)
来源：http://my.lnxyls.cn

Go:   func main()
来源：http://yt.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jb.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://cm.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://tc.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://mv.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://fi.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://ug.9csxet.cn

TS:   process.platform;  process.version
来源：http://tf.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gx.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gh.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rm.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vu.gzmigu.cn

================================================================================
来源：http://lh.huixiangedu.cn

N. 数据结构与算法
来源：http://ky.lnxyls.cn

================================================================================
来源：http://ys.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://sf.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nh.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ln.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://re.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ki.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ct.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://wo.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nx.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kl.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://jy.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://bl.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jv.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ri.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yd.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hn.9csxet.cn

Go:   slices.Sort(arr)
来源：http://fo.521024.cn

Ruby: arr.sort
来源：http://ir.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sf.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://cj.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://im.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://eh.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ji.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kn.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oo.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://me.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kk.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sk.jctech888.com.cn

[N04] 斐波那契数列
来源：http://oo.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ui.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ac.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fi.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xs.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gg.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fs.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xc.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://un.asd995.cn

[N05] 最大公约数
来源：http://zf.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ey.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zo.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bk.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nq.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qi.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sz.huanxung.cn

Ruby: a.gcd(b)
来源：http://dg.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uj.hnjuh.cn

[N06] 判断回文字符串
来源：http://bp.521024.cn

Py:   s == s[::-1]
来源：http://aw.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://pq.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://pt.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://dz.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rf.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://jq.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://bi.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cc.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://mh.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iy.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zt.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ke.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://qy.huanxung.cn

Java: // 手写 HashMap
来源：http://rn.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://lz.szxytkj.cn

Ruby: // 手写 Hash
来源：http://si.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tw.muxihuayi.cn

[N08] 生成全排列
来源：http://on.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://jq.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://ba.9csxet.cn

JS:   // 手写回溯递归
来源：http://le.521024.cn

TS:   // 手写回溯递归
来源：http://mj.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://if.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://mr.colortex.cn

Ruby: arr.permutation.to_a
来源：http://kh.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://rv.gzmigu.cn

[N09] 栈与队列
来源：http://zk.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rj.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yc.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yx.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wc.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qj.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rh.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wj.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dg.haigaiapp.cn

[N10] 链表节点定义
来源：http://lu.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bd.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tl.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tz.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ll.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ug.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tv.haigaiapp.cn


<!-- 参考信息 -->