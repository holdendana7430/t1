代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uo.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fd.521024.cn

[J10] 取今天 / 本月第一天
来源：http://kk.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wt.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rp.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://db.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qd.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qi.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pw.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ew.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zp.yuntaijiaju.cn

================================================================================
来源：http://js.newstarts.cn

K. JSON 与序列化
来源：http://zt.hnjuh.cn

================================================================================
来源：http://vj.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://uq.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uy.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://se.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://vi.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://kq.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fa.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://zb.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ud.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qx.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://uq.asd995.cn

Py:   json.loads(s)
来源：http://rq.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hm.hnjuh.cn

JS:   JSON.parse(s)
来源：http://pn.9csxet.cn

TS:   JSON.parse(s)
来源：http://zm.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://it.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://cq.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://oq.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oy.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zn.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lo.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lx.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dx.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cu.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ge.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rn.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://an.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bl.521024.cn

[K04] 读取 JSON 文件
来源：http://tf.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sv.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xd.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bo.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ze.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oj.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pl.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hn.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qx.nicolike.cn

[K05] 深拷贝对象
来源：http://an.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://dj.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://yo.asd995.cn

JS:   structuredClone(obj)
来源：http://bz.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://ht.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ho.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://la.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dy.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yz.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://jm.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://le.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nc.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hl.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hq.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sv.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ko.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://if.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sg.bjjhwx.cn

[K07] 进制转换
来源：http://iu.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ub.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sw.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bi.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lq.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cx.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nf.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dh.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://og.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://eu.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ok.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dn.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zx.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://fd.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ay.nicolike.cn

Go:   encoding/gob
来源：http://xj.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://oj.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ba.nszjky.cn

================================================================================
来源：http://lb.szsharing.cn

L. 网络请求
来源：http://xa.chemitech.net.cn

================================================================================
来源：http://po.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://qm.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pg.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kb.yuexingan06.cn

JS:   await fetch(url)
来源：http://nn.nszjky.cn

TS:   await fetch(url)
来源：http://cq.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kp.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://ba.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ix.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xz.szxytkj.cn

[L02] 发送 POST JSON
来源：http://af.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sy.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sf.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://so.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://co.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gg.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ux.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://si.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://po.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dx.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hi.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dq.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tx.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yr.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ro.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qs.szxytkj.cn

[L04] 设置超时
来源：http://qn.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://sf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nr.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rv.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uu.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kn.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ja.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dt.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yi.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://in.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ae.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://es.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ex.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ub.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jj.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cd.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ul.huanxung.cn

[L06] 解析响应为 JSON
来源：http://fd.jctech888.com.cn

Py:   resp.json()
来源：http://ht.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://gp.shtwfgs.cn

JS:   await resp.json()
来源：http://dh.jianghongdianzi.cn

TS:   await resp.json()
来源：http://gf.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://on.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tn.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://qf.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://au.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://gg.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uo.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lv.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ya.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ur.wgjwhj.cn

Java: resp.statusCode()
来源：http://vh.wgjwhj.cn

Go:   resp.StatusCode
来源：http://ix.asd995.cn

Ruby: resp.code.to_i
来源：http://hk.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://cn.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://iu.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oy.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://cb.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ob.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vl.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cz.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wc.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iw.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ii.hnjuh.cn

================================================================================
来源：http://nn.521024.cn

M. 命令行 / 进程 / 环境
来源：http://pe.muxihuayi.cn

================================================================================
来源：http://sc.shtwfgs.cn

[M01] 读取命令行参数
来源：http://vv.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://tu.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://up.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://fw.9csxet.cn

TS:   process.argv.slice(2)
来源：http://va.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://eo.haigaiapp.cn

Go:   os.Args[1:]
来源：http://zl.jianghongdianzi.cn

Ruby: ARGV
来源：http://ro.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ls.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://zg.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ck.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ya.yuexingan06.cn

JS:   process.env.HOME
来源：http://mq.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://dk.lnxyls.cn

Java: System.getenv("HOME")
来源：http://wq.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lm.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://jo.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://di.szxytkj.cn

[M03] 执行外部命令
来源：http://ow.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pt.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zp.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oz.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ew.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wi.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gv.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://oq.gzmigu.cn

[M04] 获取当前工作目录
来源：http://hf.shxzukj.cn

Py:   os.getcwd()
来源：http://lh.huanxung.cn

PHP:  getcwd();
来源：http://sx.nicolike.cn

JS:   process.cwd()
来源：http://ce.shxzskj.cn

TS:   process.cwd()
来源：http://wb.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://fv.colortex.cn

Go:   os.Getwd()
来源：http://qs.9csxet.cn

Ruby: Dir.pwd
来源：http://qf.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xu.jianghongdianzi.cn

[M05] 设置退出码
来源：http://yv.shxzukj.cn

Py:   sys.exit(1)
来源：http://rd.bjjhwx.cn

PHP:  exit(1);
来源：http://sw.hahajie.cn

JS:   process.exit(1)
来源：http://ol.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://nv.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ch.jctech888.com.cn

Go:   os.Exit(1)
来源：http://ah.szsharing.cn

Ruby: exit 1
来源：http://ab.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://as.shtwfgs.cn

[M06] 向标准错误输出
来源：http://nj.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://hi.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sw.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ql.9csxet.cn

TS:   console.error("err")
来源：http://fj.hnjuh.cn

Java: System.err.println("err")
来源：http://jz.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ai.panjiajie.cn

Ruby: warn "err"
来源：http://rr.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://xf.asd995.cn

[M07] 判断是否为主入口
来源：http://ib.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://cd.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tp.bjjhwx.cn

JS:   require.main === module
来源：http://ty.szxytkj.cn

TS:   require.main === module
来源：http://wx.9csxet.cn

Java: public static void main(String[] args)
来源：http://ji.huixiangedu.cn

Go:   func main()
来源：http://ny.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gz.colortex.cn

C#:   static void Main(string[] args)
来源：http://bi.521024.cn

[M08] 获取系统与运行时信息
来源：http://qz.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://jp.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://lg.hahajie.cn

JS:   process.platform;  process.version
来源：http://iu.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ae.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pw.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ml.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gq.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rz.yuexingan06.cn

================================================================================
来源：http://bn.haigaiapp.cn

N. 数据结构与算法
来源：http://tk.nicolike.cn

================================================================================
来源：http://vr.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://sb.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fu.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hx.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nk.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://il.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uw.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://gc.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vp.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://au.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://bt.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://ln.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nk.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mw.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nn.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gc.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://um.shxzskj.cn

Ruby: arr.sort
来源：http://hv.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zi.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://ko.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ts.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://cr.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yj.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bw.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xb.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ot.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ed.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gj.shxzskj.cn

[N04] 斐波那契数列
来源：http://fh.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cp.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xc.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://db.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pi.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ib.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dx.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mf.chemitech.net.cn

[N05] 最大公约数
来源：http://lo.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://mv.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jd.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aq.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dm.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gm.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ut.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://lm.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ki.gzmigu.cn

[N06] 判断回文字符串
来源：http://vp.hnjuh.cn

Py:   s == s[::-1]
来源：http://pz.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://il.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://dz.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://xl.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://do.nszjky.cn

Go:   // 双指针从两端比较
来源：http://nj.yuexingan06.cn

Ruby: s == s.reverse
来源：http://qz.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qm.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://iy.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qw.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tv.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lm.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://wz.nicolike.cn

Java: // 手写 HashMap
来源：http://ba.521024.cn


<!-- 参考信息 -->