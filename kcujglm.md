代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hh.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hl.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://li.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oc.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xd.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jz.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xk.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fh.bjjhwx.cn

================================================================================
来源：http://gx.wgjwhj.cn

K. JSON 与序列化
来源：http://hd.jianghongdianzi.cn

================================================================================
来源：http://ge.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://la.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ah.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vi.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://cu.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://ww.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oa.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://lc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pw.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wy.asd995.cn

[K02] JSON 字符串转对象
来源：http://cr.wgjwhj.cn

Py:   json.loads(s)
来源：http://ou.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cr.colortex.cn

JS:   JSON.parse(s)
来源：http://em.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://rq.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xj.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://pq.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://tc.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ow.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://wu.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ec.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rl.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nl.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zz.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ia.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pc.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sp.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://fn.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zo.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qp.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lh.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iw.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://us.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rj.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rj.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ac.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://ut.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ra.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://hu.lnxyls.cn

TS:   structuredClone(obj)
来源：http://tj.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jg.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yu.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hl.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lr.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://xg.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oh.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qt.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hj.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tg.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lk.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://di.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ig.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://as.jianghongdianzi.cn

[K07] 进制转换
来源：http://ce.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dd.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ji.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ym.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xu.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wm.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://he.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iq.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fu.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://bt.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://lc.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dt.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ob.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://oc.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tq.shxzskj.cn

Go:   encoding/gob
来源：http://jb.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://xk.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ea.yuexingan06.cn

================================================================================
来源：http://oi.shxzukj.cn

L. 网络请求
来源：http://mg.9csxet.cn

================================================================================
来源：http://nl.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ou.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zi.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vc.huixiangedu.cn

JS:   await fetch(url)
来源：http://mi.hahajie.cn

TS:   await fetch(url)
来源：http://zk.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gt.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://fa.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qu.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ze.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://js.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ac.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://we.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qw.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kl.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jz.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ca.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ui.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pe.lnxyls.cn

[L03] 设置自定义请求头
来源：http://px.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xo.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jw.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eo.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xe.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ib.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ca.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bu.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cf.hnjuh.cn

[L04] 设置超时
来源：http://di.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://vr.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bq.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kf.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://li.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vr.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hh.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tz.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yd.hahajie.cn

[L05] 上传文件（multipart）
来源：http://ne.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gc.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://id.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://os.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ju.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wu.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://em.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ve.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dd.colortex.cn

[L06] 解析响应为 JSON
来源：http://pf.huanxung.cn

Py:   resp.json()
来源：http://xb.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://wu.nicolike.cn

JS:   await resp.json()
来源：http://gg.panjiajie.cn

TS:   await resp.json()
来源：http://pc.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mj.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vs.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://nr.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://xu.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vj.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xm.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://xp.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://cr.shxzukj.cn

Java: resp.statusCode()
来源：http://om.huixiangedu.cn

Go:   resp.StatusCode
来源：http://bi.nicolike.cn

Ruby: resp.code.to_i
来源：http://gg.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://ep.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://hu.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://af.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://rg.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mx.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lr.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oo.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wh.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vd.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jg.gzmigu.cn

================================================================================
来源：http://ey.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://da.yuexingan06.cn

================================================================================
来源：http://uw.nicolike.cn

[M01] 读取命令行参数
来源：http://wv.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://aj.colortex.cn

PHP:  $argv;  $argc;
来源：http://kx.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://sf.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://tj.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://wg.bjjhwx.cn

Go:   os.Args[1:]
来源：http://ze.szxytkj.cn

Ruby: ARGV
来源：http://eo.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://gs.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ka.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://jb.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.asd995.cn

JS:   process.env.HOME
来源：http://gl.nszjky.cn

TS:   process.env.HOME
来源：http://tq.szxytkj.cn

Java: System.getenv("HOME")
来源：http://sh.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vq.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://hs.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ya.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://nu.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nl.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ab.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://og.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nb.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cv.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pg.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bd.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://du.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ip.lnxyls.cn

Py:   os.getcwd()
来源：http://ja.huixinmuqiang.cn

PHP:  getcwd();
来源：http://sk.shtwfgs.cn

JS:   process.cwd()
来源：http://ij.gzmigu.cn

TS:   process.cwd()
来源：http://ks.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://sq.nszjky.cn

Go:   os.Getwd()
来源：http://rx.szsharing.cn

Ruby: Dir.pwd
来源：http://rm.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yj.shtwfgs.cn

[M05] 设置退出码
来源：http://vw.lnxyls.cn

Py:   sys.exit(1)
来源：http://hi.jctech888.com.cn

PHP:  exit(1);
来源：http://ec.521024.cn

JS:   process.exit(1)
来源：http://iv.jctech888.com.cn

TS:   process.exit(1)
来源：http://qw.gzmigu.cn

Java: System.exit(1)
来源：http://gn.nszjky.cn

Go:   os.Exit(1)
来源：http://pt.huixinmuqiang.cn

Ruby: exit 1
来源：http://uk.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nu.yuexingan06.cn

[M06] 向标准错误输出
来源：http://mu.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://uf.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yc.shxzskj.cn

JS:   console.error("err")
来源：http://xt.bookmarksfly.cn

TS:   console.error("err")
来源：http://wj.9csxet.cn

Java: System.err.println("err")
来源：http://jn.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jn.shtwfgs.cn

Ruby: warn "err"
来源：http://lr.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://rk.shxzukj.cn

[M07] 判断是否为主入口
来源：http://gi.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://jw.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ew.colortex.cn

JS:   require.main === module
来源：http://gw.colortex.cn

TS:   require.main === module
来源：http://gy.nszjky.cn

Java: public static void main(String[] args)
来源：http://ee.szsharing.cn

Go:   func main()
来源：http://vd.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fi.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://se.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://mo.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://zx.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://co.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://lc.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://tm.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rv.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dp.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qa.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ri.chemitech.net.cn

================================================================================
来源：http://ic.gzmigu.cn

N. 数据结构与算法
来源：http://tf.chemitech.net.cn

================================================================================
来源：http://es.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://bd.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jo.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dp.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://py.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fv.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cw.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ex.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dk.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wz.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://mx.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://uy.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pi.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ti.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ar.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yd.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://id.jctech888.com.cn

Ruby: arr.sort
来源：http://go.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gz.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://eg.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ic.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://yc.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kk.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wv.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vv.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fi.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://if.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tb.521024.cn

[N04] 斐波那契数列
来源：http://oz.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://io.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cx.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qc.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ff.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wl.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sz.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pv.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nszjky.cn

[N05] 最大公约数
来源：http://ev.colortex.cn

Py:   math.gcd(a, b)
来源：http://da.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://si.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xl.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tv.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lg.newstarts.cn

Ruby: a.gcd(b)
来源：http://hz.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sd.szxytkj.cn

[N06] 判断回文字符串
来源：http://pn.gzmigu.cn

Py:   s == s[::-1]
来源：http://lk.colortex.cn

PHP:  $s === strrev($s);
来源：http://qj.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://ux.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://so.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://na.szsharing.cn

Go:   // 双指针从两端比较
来源：http://fp.hahajie.cn

Ruby: s == s.reverse
来源：http://gw.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kz.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://qt.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://io.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mh.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xa.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://hu.szsharing.cn

Java: // 手写 HashMap
来源：http://ue.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://rk.panjiajie.cn

Ruby: // 手写 Hash
来源：http://dd.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zf.hnjuh.cn

[N08] 生成全排列
来源：http://xb.521024.cn


<!-- 参考信息 -->