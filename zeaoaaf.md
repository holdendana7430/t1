代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ne.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zk.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sf.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qr.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://wc.panjiajie.cn

[J08] 提取年月日与星期
来源：http://qi.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ic.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://id.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ww.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ez.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bn.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xg.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gx.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xo.hnjuh.cn

[J09] 时区处理
来源：http://et.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ny.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wa.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hl.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nn.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sg.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bb.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yt.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nx.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ci.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fg.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dl.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://si.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cn.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rj.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gb.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cz.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ps.haigaiapp.cn

================================================================================
来源：http://oj.szsharing.cn

K. JSON 与序列化
来源：http://zv.panjiajie.cn

================================================================================
来源：http://oe.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://an.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ie.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sp.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://pm.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://cu.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ja.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ua.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cp.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ih.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://bs.yuexingan06.cn

Py:   json.loads(s)
来源：http://ko.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pr.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://vc.shxzukj.cn

TS:   JSON.parse(s)
来源：http://hx.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uu.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://qj.szsharing.cn

Ruby: JSON.parse(s)
来源：http://qg.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://on.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ax.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sm.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jg.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mq.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tu.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tk.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wn.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wd.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lf.newstarts.cn

[K04] 读取 JSON 文件
来源：http://rs.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pg.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kz.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rm.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hv.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gt.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tx.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pa.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wo.shxzukj.cn

[K05] 深拷贝对象
来源：http://ri.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://dm.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://df.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://vi.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://iq.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tt.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qo.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ng.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rr.szsharing.cn

[K06] 解析 URL 查询串
来源：http://tg.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://db.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lh.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wk.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aj.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ay.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://op.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ac.colortex.cn

[K07] 进制转换
来源：http://uq.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cj.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ca.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://op.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zt.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pq.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lp.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ng.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nw.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://dt.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://ux.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nj.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://qn.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://kb.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jo.lnxyls.cn

Go:   encoding/gob
来源：http://ti.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://yd.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cy.colortex.cn

================================================================================
来源：http://fb.panjiajie.cn

L. 网络请求
来源：http://ma.haigaiapp.cn

================================================================================
来源：http://nf.hnjuh.cn

[L01] 发送 GET 请求
来源：http://sp.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zp.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ec.newstarts.cn

JS:   await fetch(url)
来源：http://yi.jctech888.com.cn

TS:   await fetch(url)
来源：http://aw.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lj.521024.cn

Go:   resp, err := http.Get(url)
来源：http://nb.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fb.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vj.nszjky.cn

[L02] 发送 POST JSON
来源：http://lb.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bm.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wm.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qk.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ic.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vd.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ps.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wu.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jy.asd995.cn

[L03] 设置自定义请求头
来源：http://tj.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ee.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dd.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pv.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qt.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tx.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ci.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rx.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zu.muxihuayi.cn

[L04] 设置超时
来源：http://ek.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://eh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bk.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sw.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://og.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gl.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tw.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nc.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ju.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://nz.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ar.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wo.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xm.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lf.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rs.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ei.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ln.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qs.9csxet.cn

[L06] 解析响应为 JSON
来源：http://og.bjjhwx.cn

Py:   resp.json()
来源：http://fr.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://hm.nicolike.cn

JS:   await resp.json()
来源：http://zy.wgjwhj.cn

TS:   await resp.json()
来源：http://ty.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vk.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sa.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://sh.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://om.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://fb.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://im.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://gu.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://lz.szxytkj.cn

Java: resp.statusCode()
来源：http://qv.huixiangedu.cn

Go:   resp.StatusCode
来源：http://ja.nszjky.cn

Ruby: resp.code.to_i
来源：http://na.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://hb.asd995.cn

[L08] 并发请求多个地址
来源：http://sg.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tw.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://kb.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://df.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vr.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ub.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bw.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sq.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://at.newstarts.cn

================================================================================
来源：http://jm.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://bx.521024.cn

================================================================================
来源：http://qg.asd995.cn

[M01] 读取命令行参数
来源：http://ek.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://tc.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://oy.nszjky.cn

JS:   process.argv.slice(2)
来源：http://ri.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://og.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://lr.hahajie.cn

Go:   os.Args[1:]
来源：http://lf.bookmarksfly.cn

Ruby: ARGV
来源：http://at.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://rr.huanxung.cn

[M02] 读取环境变量
来源：http://sv.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://rm.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qh.szxytkj.cn

JS:   process.env.HOME
来源：http://xd.9csxet.cn

TS:   process.env.HOME
来源：http://uy.nszjky.cn

Java: System.getenv("HOME")
来源：http://mt.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zp.nicolike.cn

Ruby: ENV["HOME"]
来源：http://dv.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jt.chemitech.net.cn

[M03] 执行外部命令
来源：http://mo.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://il.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fu.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dy.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dc.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fq.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://px.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bl.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://al.shxzskj.cn

[M04] 获取当前工作目录
来源：http://pu.colortex.cn

Py:   os.getcwd()
来源：http://lo.hnjuh.cn

PHP:  getcwd();
来源：http://fm.colortex.cn

JS:   process.cwd()
来源：http://ca.huixinmuqiang.cn

TS:   process.cwd()
来源：http://qj.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ry.huanxung.cn

Go:   os.Getwd()
来源：http://eq.huixiangedu.cn

Ruby: Dir.pwd
来源：http://lw.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ud.bjjhwx.cn

[M05] 设置退出码
来源：http://bc.yuexingan06.cn

Py:   sys.exit(1)
来源：http://ai.chemitech.net.cn

PHP:  exit(1);
来源：http://xt.shtwfgs.cn

JS:   process.exit(1)
来源：http://kw.wgjwhj.cn

TS:   process.exit(1)
来源：http://hw.bookmarksfly.cn

Java: System.exit(1)
来源：http://sw.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://mu.hahajie.cn

Ruby: exit 1
来源：http://qo.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ll.9csxet.cn

[M06] 向标准错误输出
来源：http://wf.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://kh.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tm.hnjuh.cn

JS:   console.error("err")
来源：http://zm.haigaiapp.cn

TS:   console.error("err")
来源：http://oa.newstarts.cn

Java: System.err.println("err")
来源：http://nj.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://az.jianghongdianzi.cn

Ruby: warn "err"
来源：http://ct.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ir.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://tm.asd995.cn

Py:   if __name__ == "__main__":
来源：http://mq.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ah.shtwfgs.cn

JS:   require.main === module
来源：http://qr.9csxet.cn

TS:   require.main === module
来源：http://up.nszjky.cn

Java: public static void main(String[] args)
来源：http://xh.muxihuayi.cn

Go:   func main()
来源：http://ab.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mj.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://mx.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://af.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://hh.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://ar.shxzskj.cn

JS:   process.platform;  process.version
来源：http://rs.asd995.cn

TS:   process.platform;  process.version
来源：http://qn.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://my.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rn.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gc.huixinmuqiang.cn

================================================================================
来源：http://pf.szsharing.cn

N. 数据结构与算法
来源：http://cs.hnjuh.cn

================================================================================
来源：http://jy.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://as.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sn.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://du.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://of.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ha.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wj.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://zz.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rb.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mr.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://sd.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://lq.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ze.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gu.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mv.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://td.colortex.cn

Go:   slices.Sort(arr)
来源：http://yg.shxzukj.cn

Ruby: arr.sort
来源：http://hu.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vm.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://lq.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tq.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://kb.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pp.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dx.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ns.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bc.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gi.wgjwhj.cn

[N04] 斐波那契数列
来源：http://rx.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mp.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://du.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nv.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gz.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ok.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fr.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kb.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qa.panjiajie.cn

[N05] 最大公约数
来源：http://dc.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ao.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fg.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zp.521024.cn


<!-- 参考信息 -->