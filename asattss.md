代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://oo.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uk.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fy.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ya.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iz.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://jr.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kn.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://sh.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ol.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://zt.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ux.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://st.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oj.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://oz.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://dl.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://zb.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://mv.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://gb.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fr.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://an.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oe.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ox.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yv.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bf.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://xi.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://wu.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jp.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ns.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mp.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bn.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cb.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hn.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rz.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://go.shtwfgs.cn

[J09] 时区处理
来源：http://yj.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vn.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dw.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://br.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qm.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://an.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pi.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nl.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vb.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://oa.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hv.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cg.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://da.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cz.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zi.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ec.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://st.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iw.panjiajie.cn

================================================================================
来源：http://mg.haigaiapp.cn

K. JSON 与序列化
来源：http://hz.521024.cn

================================================================================
来源：http://se.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://fz.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wb.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ds.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://dm.521024.cn

TS:   JSON.stringify(obj)
来源：http://ze.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ao.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://oh.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qr.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wk.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://qi.haigaiapp.cn

Py:   json.loads(s)
来源：http://rn.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rl.newstarts.cn

JS:   JSON.parse(s)
来源：http://cg.9csxet.cn

TS:   JSON.parse(s)
来源：http://ab.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ys.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://vy.huanxung.cn

Ruby: JSON.parse(s)
来源：http://ex.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qg.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ee.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dl.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rq.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://by.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gg.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bt.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vu.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jd.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://uz.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ex.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sy.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xt.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fg.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uw.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wl.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ie.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hs.nicolike.cn

[K05] 深拷贝对象
来源：http://lu.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://nh.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://il.gzmigu.cn

JS:   structuredClone(obj)
来源：http://tr.szsharing.cn

TS:   structuredClone(obj)
来源：http://dq.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qg.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bb.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ac.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ug.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://tm.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tb.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fm.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sk.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ne.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ce.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sz.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lr.jctech888.com.cn

[K07] 进制转换
来源：http://vc.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zq.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ga.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sn.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jk.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vl.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://px.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vn.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vp.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://uc.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://wg.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nu.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://ij.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://db.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fu.asd995.cn

Go:   encoding/gob
来源：http://cz.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://cy.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xz.yuntaijiaju.cn

================================================================================
来源：http://uy.muxihuayi.cn

L. 网络请求
来源：http://fv.wgjwhj.cn

================================================================================
来源：http://ab.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://tb.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uu.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bn.huixiangedu.cn

JS:   await fetch(url)
来源：http://eh.muxihuayi.cn

TS:   await fetch(url)
来源：http://xr.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ge.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://we.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bk.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wn.szxytkj.cn

[L02] 发送 POST JSON
来源：http://za.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ur.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ti.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://di.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xn.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fm.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jq.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nj.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tb.nicolike.cn

[L03] 设置自定义请求头
来源：http://oy.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yf.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hw.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://le.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dy.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gs.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kr.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qe.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uq.lnxyls.cn

[L04] 设置超时
来源：http://wk.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://dy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bm.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yp.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mc.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jr.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jl.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eg.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qq.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://bk.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ir.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ev.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rx.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qm.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eg.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sw.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sq.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cd.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://vg.hahajie.cn

Py:   resp.json()
来源：http://hd.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ec.huixiangedu.cn

JS:   await resp.json()
来源：http://yk.asd995.cn

TS:   await resp.json()
来源：http://hl.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rn.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tq.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://tp.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fr.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://wk.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pi.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mt.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://fp.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://qq.yuexingan06.cn

Java: resp.statusCode()
来源：http://om.bjjhwx.cn

Go:   resp.StatusCode
来源：http://cn.asd995.cn

Ruby: resp.code.to_i
来源：http://kj.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://fy.szsharing.cn

[L08] 并发请求多个地址
来源：http://lr.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sj.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ht.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gd.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kq.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qt.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bb.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ec.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qo.asd995.cn

================================================================================
来源：http://ov.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://lh.wgjwhj.cn

================================================================================
来源：http://mv.shtwfgs.cn

[M01] 读取命令行参数
来源：http://bt.newstarts.cn

Py:   sys.argv[1:]
来源：http://nm.9csxet.cn

PHP:  $argv;  $argc;
来源：http://qn.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://be.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ur.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://ng.colortex.cn

Go:   os.Args[1:]
来源：http://hv.asd995.cn

Ruby: ARGV
来源：http://po.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://av.9csxet.cn

[M02] 读取环境变量
来源：http://sn.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://qj.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mf.szxytkj.cn

JS:   process.env.HOME
来源：http://xs.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://jw.panjiajie.cn

Java: System.getenv("HOME")
来源：http://of.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iu.colortex.cn

Ruby: ENV["HOME"]
来源：http://lg.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lb.hahajie.cn

[M03] 执行外部命令
来源：http://av.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ro.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uv.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://js.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qn.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dd.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yk.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kn.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ee.9csxet.cn

[M04] 获取当前工作目录
来源：http://md.9csxet.cn

Py:   os.getcwd()
来源：http://un.shxzukj.cn

PHP:  getcwd();
来源：http://jn.bjjhwx.cn

JS:   process.cwd()
来源：http://pr.nszjky.cn

TS:   process.cwd()
来源：http://nl.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://li.nicolike.cn

Go:   os.Getwd()
来源：http://wa.9csxet.cn

Ruby: Dir.pwd
来源：http://xl.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ej.hnjuh.cn

[M05] 设置退出码
来源：http://ju.szsharing.cn

Py:   sys.exit(1)
来源：http://yz.lnxyls.cn

PHP:  exit(1);
来源：http://en.lnxyls.cn

JS:   process.exit(1)
来源：http://bh.newstarts.cn

TS:   process.exit(1)
来源：http://ot.nicolike.cn

Java: System.exit(1)
来源：http://qi.wgjwhj.cn

Go:   os.Exit(1)
来源：http://rs.haigaiapp.cn

Ruby: exit 1
来源：http://qm.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ka.nszjky.cn

[M06] 向标准错误输出
来源：http://xc.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://ce.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oq.shtwfgs.cn

JS:   console.error("err")
来源：http://ip.lnxyls.cn

TS:   console.error("err")
来源：http://bh.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://tg.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yj.9csxet.cn

Ruby: warn "err"
来源：http://yo.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://eu.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://qt.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ad.jianghongdianzi.cn

JS:   require.main === module
来源：http://wt.bookmarksfly.cn

TS:   require.main === module
来源：http://hc.9csxet.cn

Java: public static void main(String[] args)
来源：http://yw.huixinmuqiang.cn

Go:   func main()
来源：http://dt.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jc.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://cv.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://cl.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://ze.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://dn.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://uk.lnxyls.cn

TS:   process.platform;  process.version
来源：http://zq.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hn.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://th.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vu.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oi.yuexingan06.cn

================================================================================
来源：http://us.muxihuayi.cn

N. 数据结构与算法
来源：http://gz.szxytkj.cn

================================================================================
来源：http://he.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://is.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dl.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bp.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sa.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ug.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lf.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://hi.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://se.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ed.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://lt.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mq.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xv.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ta.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hy.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hp.newstarts.cn

Go:   slices.Sort(arr)
来源：http://xx.yuntaijiaju.cn

Ruby: arr.sort
来源：http://zu.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nw.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://fe.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nk.huixiangedu.cn


<!-- 参考信息 -->