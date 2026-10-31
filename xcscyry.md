代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vv.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ky.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rm.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sv.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ym.newstarts.cn

Py:   json.loads(s)
来源：http://vp.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uu.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://tk.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://lt.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rk.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://kh.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ta.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lp.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://rm.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xh.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jg.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://df.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vz.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://db.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://de.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tp.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zz.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ej.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ev.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rh.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zn.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://il.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://im.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lg.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ml.gzmigu.cn

[K05] 深拷贝对象
来源：http://ih.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://jo.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://yg.shxzukj.cn

JS:   structuredClone(obj)
来源：http://fo.shxzukj.cn

TS:   structuredClone(obj)
来源：http://op.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://al.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ia.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bx.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ao.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://yc.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ml.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yp.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tu.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kx.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xq.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ck.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sy.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ss.bjjhwx.cn

[K07] 进制转换
来源：http://un.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ox.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ca.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uj.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nu.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pt.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pi.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pa.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rb.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://hu.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://rp.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rf.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://nj.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://lg.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wh.chemitech.net.cn

Go:   encoding/gob
来源：http://tt.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://cv.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pa.nicolike.cn

================================================================================
来源：http://zc.huanxung.cn

L. 网络请求
来源：http://hj.hnjuh.cn

================================================================================
来源：http://dm.nszjky.cn

[L01] 发送 GET 请求
来源：http://gz.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hu.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ag.chemitech.net.cn

JS:   await fetch(url)
来源：http://vq.newstarts.cn

TS:   await fetch(url)
来源：http://pk.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pa.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://yt.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zh.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sq.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://vr.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ys.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jp.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://in.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://el.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kv.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gy.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wf.lnxyls.cn

[L03] 设置自定义请求头
来源：http://gj.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ym.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bt.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ph.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rg.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ux.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yg.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://it.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wk.jctech888.com.cn

[L04] 设置超时
来源：http://hz.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://xp.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zv.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://au.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ov.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xk.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://id.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://te.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fy.huanxung.cn

[L05] 上传文件（multipart）
来源：http://dw.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gy.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iw.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hc.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cv.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xr.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mn.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fx.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mk.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://or.hnjuh.cn

Py:   resp.json()
来源：http://yx.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://wa.521024.cn

JS:   await resp.json()
来源：http://hu.bjjhwx.cn

TS:   await resp.json()
来源：http://ms.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ld.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xz.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://tq.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sw.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://rk.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://no.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lr.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://dr.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://jg.nszjky.cn

Java: resp.statusCode()
来源：http://lp.szxytkj.cn

Go:   resp.StatusCode
来源：http://wp.lnxyls.cn

Ruby: resp.code.to_i
来源：http://wa.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://qg.szxytkj.cn

[L08] 并发请求多个地址
来源：http://kg.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kc.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://js.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bh.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jn.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xu.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://al.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://js.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bs.wgjwhj.cn

================================================================================
来源：http://ry.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://re.jctech888.com.cn

================================================================================
来源：http://dh.lnxyls.cn

[M01] 读取命令行参数
来源：http://gu.9csxet.cn

Py:   sys.argv[1:]
来源：http://ua.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://ya.asd995.cn

JS:   process.argv.slice(2)
来源：http://zx.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://pz.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://vr.gzmigu.cn

Go:   os.Args[1:]
来源：http://nf.shxzskj.cn

Ruby: ARGV
来源：http://nq.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://tw.bjjhwx.cn

[M02] 读取环境变量
来源：http://km.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://gr.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dp.colortex.cn

JS:   process.env.HOME
来源：http://tj.muxihuayi.cn

TS:   process.env.HOME
来源：http://nq.colortex.cn

Java: System.getenv("HOME")
来源：http://da.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bm.nszjky.cn

Ruby: ENV["HOME"]
来源：http://fa.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xp.hahajie.cn

[M03] 执行外部命令
来源：http://mj.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uy.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gi.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qf.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mk.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lb.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hs.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ny.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://nd.szxytkj.cn

[M04] 获取当前工作目录
来源：http://di.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://fh.muxihuayi.cn

PHP:  getcwd();
来源：http://vc.muxihuayi.cn

JS:   process.cwd()
来源：http://ox.nszjky.cn

TS:   process.cwd()
来源：http://mt.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://dh.panjiajie.cn

Go:   os.Getwd()
来源：http://av.shtwfgs.cn

Ruby: Dir.pwd
来源：http://oi.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://in.jctech888.com.cn

[M05] 设置退出码
来源：http://ba.huanxung.cn

Py:   sys.exit(1)
来源：http://un.hahajie.cn

PHP:  exit(1);
来源：http://zz.chemitech.net.cn

JS:   process.exit(1)
来源：http://ti.hahajie.cn

TS:   process.exit(1)
来源：http://ba.lnxyls.cn

Java: System.exit(1)
来源：http://pr.9csxet.cn

Go:   os.Exit(1)
来源：http://kb.nicolike.cn

Ruby: exit 1
来源：http://rn.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yd.haigaiapp.cn

[M06] 向标准错误输出
来源：http://nc.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://eb.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sk.wgjwhj.cn

JS:   console.error("err")
来源：http://tk.asd995.cn

TS:   console.error("err")
来源：http://lp.hnjuh.cn

Java: System.err.println("err")
来源：http://mq.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vh.jctech888.com.cn

Ruby: warn "err"
来源：http://qu.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ky.huanxung.cn

[M07] 判断是否为主入口
来源：http://un.asd995.cn

Py:   if __name__ == "__main__":
来源：http://bp.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cg.shtwfgs.cn

JS:   require.main === module
来源：http://fw.yuntaijiaju.cn

TS:   require.main === module
来源：http://dh.asd995.cn

Java: public static void main(String[] args)
来源：http://as.hahajie.cn

Go:   func main()
来源：http://qc.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qn.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://ln.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://fz.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://jt.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://eg.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://qv.newstarts.cn

TS:   process.platform;  process.version
来源：http://us.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lq.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tm.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ow.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dn.muxihuayi.cn

================================================================================
来源：http://ta.panjiajie.cn

N. 数据结构与算法
来源：http://zy.yuexingan06.cn

================================================================================
来源：http://ws.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://hc.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kn.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lz.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://id.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://da.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hs.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://gu.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eg.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wg.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://hl.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pw.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cj.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sm.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vr.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hp.asd995.cn

Go:   slices.Sort(arr)
来源：http://pe.haigaiapp.cn

Ruby: arr.sort
来源：http://jl.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ox.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://ab.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zj.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://te.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://at.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xb.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wc.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gs.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rn.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vk.shtwfgs.cn

[N04] 斐波那契数列
来源：http://xj.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yy.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://el.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gh.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://at.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ry.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ew.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ry.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wm.hahajie.cn

[N05] 最大公约数
来源：http://xq.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ji.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://th.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dz.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gl.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://if.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rp.nicolike.cn

Ruby: a.gcd(b)
来源：http://aj.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dr.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://pg.wgjwhj.cn

Py:   s == s[::-1]
来源：http://xv.szsharing.cn

PHP:  $s === strrev($s);
来源：http://is.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://py.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://wt.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wu.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://jt.haigaiapp.cn

Ruby: s == s.reverse
来源：http://ia.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ei.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://rq.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rj.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yf.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ja.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://uw.lnxyls.cn

Java: // 手写 HashMap
来源：http://jo.newstarts.cn

Go:   // 手写 map[int]int
来源：http://ov.newstarts.cn

Ruby: // 手写 Hash
来源：http://vm.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yf.huanxung.cn

[N08] 生成全排列
来源：http://ul.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://eu.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://be.shxzskj.cn

JS:   // 手写回溯递归
来源：http://gs.9csxet.cn

TS:   // 手写回溯递归
来源：http://ts.szxytkj.cn

Java: // 手写回溯递归
来源：http://bf.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://kj.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://zx.szxytkj.cn

C#:   // 手写回溯递归
来源：http://di.nicolike.cn

[N09] 栈与队列
来源：http://mt.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hu.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cd.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vj.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hn.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ox.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xv.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tm.colortex.cn


<!-- 参考信息 -->