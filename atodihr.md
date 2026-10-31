代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://ss.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uf.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jj.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ef.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ps.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://lo.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qx.colortex.cn

[J06] 计算两时间之差
来源：http://fo.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://cc.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://xn.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nr.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nq.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gd.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://fu.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://fo.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ud.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ss.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://we.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mk.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qv.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vd.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yj.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ig.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mh.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://bj.521024.cn

[J08] 提取年月日与星期
来源：http://vr.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ut.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yp.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lw.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dz.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fa.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tv.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yr.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ek.shxzskj.cn

[J09] 时区处理
来源：http://zn.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://az.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://am.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ju.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uh.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dl.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hy.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mb.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wv.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://me.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yr.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xm.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://in.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pv.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nj.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hx.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oj.colortex.cn

================================================================================
来源：http://pz.yuntaijiaju.cn

K. JSON 与序列化
来源：http://xi.yuntaijiaju.cn

================================================================================
来源：http://ed.521024.cn

[K01] 对象转 JSON 字符串
来源：http://we.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vr.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dy.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://yw.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://rh.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vr.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://rn.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ix.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://sj.shtwfgs.cn

Py:   json.loads(s)
来源：http://dl.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://st.szsharing.cn

JS:   JSON.parse(s)
来源：http://oi.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://vf.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tn.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://bl.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://cs.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tq.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ew.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://el.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lw.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sf.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fi.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dz.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ki.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fn.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://tu.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xd.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uv.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xi.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rm.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://li.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nw.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bd.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ri.huanxung.cn

[K05] 深拷贝对象
来源：http://ss.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://gk.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://vx.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://jg.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://sa.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ax.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://et.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lk.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ff.asd995.cn

[K06] 解析 URL 查询串
来源：http://jk.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ec.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mh.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xm.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lc.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ah.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xb.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ej.jianghongdianzi.cn

[K07] 进制转换
来源：http://wu.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hq.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fh.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lf.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dl.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://df.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tu.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://my.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://sy.521024.cn

Py:   pickle.dumps(obj)
来源：http://rk.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://if.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://te.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://zr.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rc.lnxyls.cn

Go:   encoding/gob
来源：http://xr.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://fb.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tk.huanxung.cn

================================================================================
来源：http://oo.yuntaijiaju.cn

L. 网络请求
来源：http://ib.muxihuayi.cn

================================================================================
来源：http://oe.szxytkj.cn

[L01] 发送 GET 请求
来源：http://zq.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xw.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nn.hahajie.cn

JS:   await fetch(url)
来源：http://vi.muxihuayi.cn

TS:   await fetch(url)
来源：http://lm.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sn.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://dg.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ib.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ay.lnxyls.cn

[L02] 发送 POST JSON
来源：http://rx.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wt.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oh.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vh.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rf.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ht.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lf.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ez.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sh.szsharing.cn

[L03] 设置自定义请求头
来源：http://oh.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://je.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vn.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uy.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pu.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zp.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dj.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://on.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ds.haigaiapp.cn

[L04] 设置超时
来源：http://tu.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://rv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xj.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sg.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oc.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xr.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ep.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zs.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pz.asd995.cn

[L05] 上传文件（multipart）
来源：http://wn.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gf.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oa.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bl.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xe.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lw.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vl.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kn.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nk.521024.cn

[L06] 解析响应为 JSON
来源：http://js.lnxyls.cn

Py:   resp.json()
来源：http://uz.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://dm.bookmarksfly.cn

JS:   await resp.json()
来源：http://uv.wgjwhj.cn

TS:   await resp.json()
来源：http://ud.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lq.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cw.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://zx.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vo.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://hl.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bc.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://db.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ho.colortex.cn

Java: resp.statusCode()
来源：http://dc.asd995.cn

Go:   resp.StatusCode
来源：http://vp.nszjky.cn

Ruby: resp.code.to_i
来源：http://xx.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://cq.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ih.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nq.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://ed.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ej.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qz.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xj.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ls.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://do.gzmigu.cn

================================================================================
来源：http://ga.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://kr.newstarts.cn

================================================================================
来源：http://qp.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://rl.gzmigu.cn

Py:   sys.argv[1:]
来源：http://fx.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://vd.newstarts.cn

JS:   process.argv.slice(2)
来源：http://oe.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://bt.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://dr.nicolike.cn

Go:   os.Args[1:]
来源：http://ms.panjiajie.cn

Ruby: ARGV
来源：http://ru.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://wz.521024.cn

[M02] 读取环境变量
来源：http://wc.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://ev.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gu.nicolike.cn

JS:   process.env.HOME
来源：http://ov.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://pn.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://ld.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xv.newstarts.cn

Ruby: ENV["HOME"]
来源：http://yo.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://is.chemitech.net.cn

[M03] 执行外部命令
来源：http://dg.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gq.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://se.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ns.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sa.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://em.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iv.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ht.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://or.huanxung.cn

[M04] 获取当前工作目录
来源：http://ba.nicolike.cn

Py:   os.getcwd()
来源：http://xd.haigaiapp.cn

PHP:  getcwd();
来源：http://wb.9csxet.cn

JS:   process.cwd()
来源：http://gv.521024.cn

TS:   process.cwd()
来源：http://tb.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://zf.yuexingan06.cn

Go:   os.Getwd()
来源：http://ql.gzmigu.cn

Ruby: Dir.pwd
来源：http://ag.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bj.newstarts.cn

[M05] 设置退出码
来源：http://vz.gzmigu.cn

Py:   sys.exit(1)
来源：http://ua.shxzukj.cn

PHP:  exit(1);
来源：http://tw.colortex.cn

JS:   process.exit(1)
来源：http://qa.nszjky.cn

TS:   process.exit(1)
来源：http://tq.521024.cn

Java: System.exit(1)
来源：http://tx.9csxet.cn

Go:   os.Exit(1)
来源：http://bg.chemitech.net.cn

Ruby: exit 1
来源：http://dk.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cm.huanxung.cn

[M06] 向标准错误输出
来源：http://wi.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://ee.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mj.newstarts.cn

JS:   console.error("err")
来源：http://jq.haigaiapp.cn

TS:   console.error("err")
来源：http://cd.nszjky.cn

Java: System.err.println("err")
来源：http://mm.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ce.haigaiapp.cn

Ruby: warn "err"
来源：http://rm.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://yh.shxzukj.cn

[M07] 判断是否为主入口
来源：http://pk.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://kj.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oj.wgjwhj.cn

JS:   require.main === module
来源：http://tp.521024.cn

TS:   require.main === module
来源：http://zc.lnxyls.cn

Java: public static void main(String[] args)
来源：http://rf.521024.cn

Go:   func main()
来源：http://oz.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eg.9csxet.cn

C#:   static void Main(string[] args)
来源：http://ch.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://tn.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://ck.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://to.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://li.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://xu.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bd.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fj.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wy.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://na.shxzskj.cn

================================================================================
来源：http://fo.huixinmuqiang.cn

N. 数据结构与算法
来源：http://fd.muxihuayi.cn

================================================================================
来源：http://uh.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://fm.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lm.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://od.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://em.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nr.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fi.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://bg.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rl.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yq.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://lh.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ha.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zx.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://se.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gj.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://xs.shxzskj.cn

Ruby: arr.sort
来源：http://az.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eb.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://pi.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vm.shtwfgs.cn


<!-- 参考信息 -->