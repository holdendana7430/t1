代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nb.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://my.colortex.cn

[J09] 时区处理
来源：http://vl.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zw.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vb.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xr.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fe.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zd.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rv.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cs.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://on.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://kw.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ks.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kt.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ja.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://or.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lv.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bf.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kn.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gn.huanxung.cn

================================================================================
来源：http://ve.asd995.cn

K. JSON 与序列化
来源：http://lw.huixiangedu.cn

================================================================================
来源：http://ad.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://zw.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ot.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fh.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://zs.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://ik.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ag.asd995.cn

Go:   json.Marshal(obj)
来源：http://fl.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oh.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ey.newstarts.cn

[K02] JSON 字符串转对象
来源：http://vp.yuexingan06.cn

Py:   json.loads(s)
来源：http://dc.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://je.panjiajie.cn

JS:   JSON.parse(s)
来源：http://og.nszjky.cn

TS:   JSON.parse(s)
来源：http://zv.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ku.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://df.521024.cn

Ruby: JSON.parse(s)
来源：http://vr.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jp.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://oy.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nm.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bi.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wc.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sy.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wk.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jr.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://od.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gc.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://ca.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tx.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vb.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://as.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://si.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uf.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pk.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kj.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ho.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ik.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ch.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://yj.szxytkj.cn

JS:   structuredClone(obj)
来源：http://rc.asd995.cn

TS:   structuredClone(obj)
来源：http://hq.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vp.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bp.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bg.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yx.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://jf.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xr.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rq.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qf.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tv.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pr.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cr.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ji.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wu.huixiangedu.cn

[K07] 进制转换
来源：http://qe.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ot.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://by.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://au.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ev.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bh.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ui.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wy.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ed.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://cv.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://fe.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://au.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://gv.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://az.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rj.hnjuh.cn

Go:   encoding/gob
来源：http://uz.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://vw.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xy.chemitech.net.cn

================================================================================
来源：http://qt.hnjuh.cn

L. 网络请求
来源：http://uo.newstarts.cn

================================================================================
来源：http://uq.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://qv.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ko.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cy.yuexingan06.cn

JS:   await fetch(url)
来源：http://wx.shtwfgs.cn

TS:   await fetch(url)
来源：http://yz.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://so.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ze.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zg.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oa.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://uu.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pp.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://es.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yn.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sc.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fh.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zq.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ni.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tw.colortex.cn

[L03] 设置自定义请求头
来源：http://po.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uf.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hl.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xr.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dl.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://st.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nv.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zn.bjjhwx.cn

[L04] 设置超时
来源：http://hy.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://li.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://en.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qz.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sf.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jz.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fh.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vf.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rd.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://eg.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yn.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ob.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kg.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rp.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hd.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qu.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://al.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nr.szsharing.cn

[L06] 解析响应为 JSON
来源：http://eq.hnjuh.cn

Py:   resp.json()
来源：http://so.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://cj.huixinmuqiang.cn

JS:   await resp.json()
来源：http://oh.hnjuh.cn

TS:   await resp.json()
来源：http://zl.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cq.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ag.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://vs.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bb.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://cw.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://it.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://um.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://yt.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://sd.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://xw.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://bi.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ys.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://kr.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://bf.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ol.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://zr.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://us.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://af.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yr.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://th.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dr.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gt.szsharing.cn

================================================================================
来源：http://gj.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://he.yuexingan06.cn

================================================================================
来源：http://hn.jctech888.com.cn

[M01] 读取命令行参数
来源：http://pt.panjiajie.cn

Py:   sys.argv[1:]
来源：http://nl.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://on.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://eu.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://xv.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://ag.chemitech.net.cn

Go:   os.Args[1:]
来源：http://re.shxzukj.cn

Ruby: ARGV
来源：http://qs.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://qi.bjjhwx.cn

[M02] 读取环境变量
来源：http://bx.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://ng.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cs.hahajie.cn

JS:   process.env.HOME
来源：http://ug.newstarts.cn

TS:   process.env.HOME
来源：http://xi.lnxyls.cn

Java: System.getenv("HOME")
来源：http://ge.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wk.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://lk.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dd.yuexingan06.cn

[M03] 执行外部命令
来源：http://bm.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yb.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jh.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ix.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ja.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ql.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://br.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ia.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://ko.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://hr.yuexingan06.cn

Py:   os.getcwd()
来源：http://er.panjiajie.cn

PHP:  getcwd();
来源：http://nh.shtwfgs.cn

JS:   process.cwd()
来源：http://if.nszjky.cn

TS:   process.cwd()
来源：http://yx.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://yf.hnjuh.cn

Go:   os.Getwd()
来源：http://ya.huixiangedu.cn

Ruby: Dir.pwd
来源：http://qb.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ba.huanxung.cn

[M05] 设置退出码
来源：http://py.shxzukj.cn

Py:   sys.exit(1)
来源：http://ke.szsharing.cn

PHP:  exit(1);
来源：http://aj.colortex.cn

JS:   process.exit(1)
来源：http://rx.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://vi.szsharing.cn

Java: System.exit(1)
来源：http://pc.huanxung.cn

Go:   os.Exit(1)
来源：http://ly.jctech888.com.cn

Ruby: exit 1
来源：http://cp.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bk.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ro.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://lw.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xf.bookmarksfly.cn

JS:   console.error("err")
来源：http://eh.lnxyls.cn

TS:   console.error("err")
来源：http://ov.jctech888.com.cn

Java: System.err.println("err")
来源：http://bk.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://im.shxzskj.cn

Ruby: warn "err"
来源：http://yk.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ty.panjiajie.cn

[M07] 判断是否为主入口
来源：http://ch.colortex.cn

Py:   if __name__ == "__main__":
来源：http://nn.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yu.bjjhwx.cn

JS:   require.main === module
来源：http://un.huixinmuqiang.cn

TS:   require.main === module
来源：http://ap.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://pv.nicolike.cn

Go:   func main()
来源：http://wz.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://ht.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://af.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://aw.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://os.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://qh.521024.cn

TS:   process.platform;  process.version
来源：http://yx.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ln.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ws.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tw.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vv.bookmarksfly.cn

================================================================================
来源：http://ij.nszjky.cn

N. 数据结构与算法
来源：http://ar.gzmigu.cn

================================================================================
来源：http://mx.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://qr.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gl.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pw.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rm.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dh.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pa.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://hk.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cc.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dp.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://au.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://bv.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lr.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xv.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jt.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lh.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://ei.bookmarksfly.cn

Ruby: arr.sort
来源：http://zy.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yw.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://hy.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ab.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ns.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nw.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zx.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wr.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mf.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wp.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wl.gzmigu.cn

[N04] 斐波那契数列
来源：http://fp.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bh.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ch.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nn.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vi.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://te.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dy.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://og.yuexingan06.cn

[N05] 最大公约数
来源：http://iz.huanxung.cn

Py:   math.gcd(a, b)
来源：http://gs.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ts.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ck.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nt.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qu.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zn.huanxung.cn

Ruby: a.gcd(b)
来源：http://dd.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wo.shxzskj.cn

[N06] 判断回文字符串
来源：http://yk.gzmigu.cn

Py:   s == s[::-1]
来源：http://oq.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ts.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://rg.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://bn.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fe.huanxung.cn

Go:   // 双指针从两端比较
来源：http://bi.jianghongdianzi.cn


<!-- 参考信息 -->