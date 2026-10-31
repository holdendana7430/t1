代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ta.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gy.lnxyls.cn

[J09] 时区处理
来源：http://jo.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nr.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sk.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bu.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wl.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qe.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ed.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rm.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mj.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://rr.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ep.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nn.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://by.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cc.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xc.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bz.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ix.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oq.haigaiapp.cn

================================================================================
来源：http://kl.bookmarksfly.cn

K. JSON 与序列化
来源：http://vc.521024.cn

================================================================================
来源：http://us.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://wv.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://of.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fa.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://jh.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://ol.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tl.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://ny.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://by.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zq.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://fl.colortex.cn

Py:   json.loads(s)
来源：http://pw.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wd.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://dg.lnxyls.cn

TS:   JSON.parse(s)
来源：http://dy.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lw.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ne.newstarts.cn

Ruby: JSON.parse(s)
来源：http://dg.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zt.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://lr.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nd.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gg.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xn.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gk.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://em.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aq.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ty.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ay.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://py.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hb.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qo.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cy.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sf.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yo.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qk.nszjky.cn

[K05] 深拷贝对象
来源：http://ed.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://xx.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://qb.asd995.cn

JS:   structuredClone(obj)
来源：http://hc.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://gi.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ux.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qv.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://px.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rn.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://da.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wq.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ei.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bh.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pp.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yp.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lp.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jy.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xh.colortex.cn

[K07] 进制转换
来源：http://bc.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hc.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hp.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hr.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://px.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mm.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zy.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pv.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yu.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ea.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://dn.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ex.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://jr.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://zc.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wk.lnxyls.cn

Go:   encoding/gob
来源：http://jq.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://du.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iy.gzmigu.cn

================================================================================
来源：http://gd.nicolike.cn

L. 网络请求
来源：http://ql.muxihuayi.cn

================================================================================
来源：http://fc.newstarts.cn

[L01] 发送 GET 请求
来源：http://rv.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ts.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kn.huixiangedu.cn

JS:   await fetch(url)
来源：http://ds.hnjuh.cn

TS:   await fetch(url)
来源：http://cd.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sw.521024.cn

Go:   resp, err := http.Get(url)
来源：http://vn.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zb.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ti.nicolike.cn

[L02] 发送 POST JSON
来源：http://rn.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jg.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kp.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oz.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://du.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nz.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wr.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sd.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nq.panjiajie.cn

[L03] 设置自定义请求头
来源：http://ix.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dr.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ry.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fw.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ll.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nv.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ye.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tn.szsharing.cn

[L04] 设置超时
来源：http://pv.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://bq.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uf.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pq.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mi.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bh.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rd.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cf.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eg.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ps.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ro.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uw.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ne.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qb.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kw.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://to.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cg.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dd.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://ul.chemitech.net.cn

Py:   resp.json()
来源：http://sk.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://iv.521024.cn

JS:   await resp.json()
来源：http://ir.huanxung.cn

TS:   await resp.json()
来源：http://gb.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sg.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vq.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://mk.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wb.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://nx.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://za.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vy.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://hp.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://yw.szsharing.cn

Java: resp.statusCode()
来源：http://pe.panjiajie.cn

Go:   resp.StatusCode
来源：http://fo.asd995.cn

Ruby: resp.code.to_i
来源：http://ma.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ey.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ip.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yn.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://re.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://li.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ii.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qr.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hm.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ia.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xy.hahajie.cn

================================================================================
来源：http://os.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://rs.gzmigu.cn

================================================================================
来源：http://bm.yuexingan06.cn

[M01] 读取命令行参数
来源：http://yo.521024.cn

Py:   sys.argv[1:]
来源：http://ez.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://hy.asd995.cn

JS:   process.argv.slice(2)
来源：http://cc.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://qk.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://gr.gzmigu.cn

Go:   os.Args[1:]
来源：http://un.hnjuh.cn

Ruby: ARGV
来源：http://xr.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://lp.asd995.cn

[M02] 读取环境变量
来源：http://mu.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://gl.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ul.shxzskj.cn

JS:   process.env.HOME
来源：http://gf.hahajie.cn

TS:   process.env.HOME
来源：http://tn.gzmigu.cn

Java: System.getenv("HOME")
来源：http://zk.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ya.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://hh.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iv.asd995.cn

[M03] 执行外部命令
来源：http://ee.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wv.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dv.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uz.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://db.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mn.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ia.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ts.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://wo.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://zo.asd995.cn

Py:   os.getcwd()
来源：http://bf.521024.cn

PHP:  getcwd();
来源：http://xw.huixiangedu.cn

JS:   process.cwd()
来源：http://gg.bookmarksfly.cn

TS:   process.cwd()
来源：http://wg.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://em.shxzukj.cn

Go:   os.Getwd()
来源：http://cp.newstarts.cn

Ruby: Dir.pwd
来源：http://lx.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bw.hahajie.cn

[M05] 设置退出码
来源：http://kr.shxzskj.cn

Py:   sys.exit(1)
来源：http://vs.haigaiapp.cn

PHP:  exit(1);
来源：http://ec.lnxyls.cn

JS:   process.exit(1)
来源：http://dx.szsharing.cn

TS:   process.exit(1)
来源：http://wz.jianghongdianzi.cn

Java: System.exit(1)
来源：http://av.jctech888.com.cn

Go:   os.Exit(1)
来源：http://wi.shxzskj.cn

Ruby: exit 1
来源：http://un.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tu.panjiajie.cn

[M06] 向标准错误输出
来源：http://pr.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://mx.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vp.muxihuayi.cn

JS:   console.error("err")
来源：http://yh.asd995.cn

TS:   console.error("err")
来源：http://pd.lnxyls.cn

Java: System.err.println("err")
来源：http://ve.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rq.huixinmuqiang.cn

Ruby: warn "err"
来源：http://zq.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://jx.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://gl.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://yp.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vy.colortex.cn

JS:   require.main === module
来源：http://wm.panjiajie.cn

TS:   require.main === module
来源：http://tx.shxzskj.cn

Java: public static void main(String[] args)
来源：http://ks.gzmigu.cn

Go:   func main()
来源：http://xb.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wv.nszjky.cn

C#:   static void Main(string[] args)
来源：http://mf.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://qp.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ir.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://ao.gzmigu.cn

JS:   process.platform;  process.version
来源：http://nv.panjiajie.cn

TS:   process.platform;  process.version
来源：http://ul.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fp.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vn.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xv.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vc.lnxyls.cn

================================================================================
来源：http://dv.shxzukj.cn

N. 数据结构与算法
来源：http://yr.newstarts.cn

================================================================================
来源：http://ei.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://wb.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qh.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ek.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yv.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rm.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gp.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ji.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fn.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mk.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zb.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zx.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vs.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gp.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gv.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ur.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://vn.panjiajie.cn

Ruby: arr.sort
来源：http://mk.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sd.asd995.cn

[N03] 快速排序（分治示例）
来源：http://gq.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fe.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://em.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ac.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sq.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://er.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bo.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fd.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jf.szsharing.cn

[N04] 斐波那契数列
来源：http://yc.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gg.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sw.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://im.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ot.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oa.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nu.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hl.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tf.haigaiapp.cn

[N05] 最大公约数
来源：http://vh.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://gj.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qw.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bb.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mt.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gu.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cw.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://xt.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gu.lnxyls.cn

[N06] 判断回文字符串
来源：http://lt.jctech888.com.cn

Py:   s == s[::-1]
来源：http://go.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://te.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://mm.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://il.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aq.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://cb.hnjuh.cn


<!-- 参考信息 -->