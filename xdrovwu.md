代发 wailian999

Py:   (end - start).total_seconds()
来源：http://di.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://qs.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jq.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ik.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xj.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://gp.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://cp.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://qv.lnxyls.cn

[J07] 比较两个日期
来源：http://ow.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://qy.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cu.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nv.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pt.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fx.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xb.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ik.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://az.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://vb.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aj.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zt.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bs.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xe.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ux.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cd.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vb.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://so.hnjuh.cn

[J09] 时区处理
来源：http://oh.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dy.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ng.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vr.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rs.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aj.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wy.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ql.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eb.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://vs.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sh.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zz.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lc.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qj.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://di.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fu.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wk.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xo.muxihuayi.cn

================================================================================
来源：http://wv.bookmarksfly.cn

K. JSON 与序列化
来源：http://gt.jctech888.com.cn

================================================================================
来源：http://nh.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://vg.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oz.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://im.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://iv.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://bu.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ir.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ii.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ux.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://me.9csxet.cn

[K02] JSON 字符串转对象
来源：http://pf.gzmigu.cn

Py:   json.loads(s)
来源：http://sk.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vl.szsharing.cn

JS:   JSON.parse(s)
来源：http://zk.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://wj.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ol.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://xj.hahajie.cn

Ruby: JSON.parse(s)
来源：http://jd.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ll.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://fe.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://as.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://st.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kd.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wn.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vt.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qn.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eg.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pt.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://bt.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fc.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ju.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ev.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dv.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tb.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pz.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vw.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://za.nszjky.cn

[K05] 深拷贝对象
来源：http://ih.521024.cn

Py:   copy.deepcopy(obj)
来源：http://wm.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://ep.hahajie.cn

JS:   structuredClone(obj)
来源：http://qh.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://fi.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qf.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mx.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pp.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cd.szsharing.cn

[K06] 解析 URL 查询串
来源：http://ad.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dd.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://st.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://by.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xb.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zb.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rf.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mr.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qw.newstarts.cn

[K07] 进制转换
来源：http://cs.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ao.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ei.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pm.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bn.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wm.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nm.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ev.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gj.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://mi.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://rh.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dz.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://pa.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://fm.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ox.szxytkj.cn

Go:   encoding/gob
来源：http://qn.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://oz.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hk.huixiangedu.cn

================================================================================
来源：http://ml.colortex.cn

L. 网络请求
来源：http://iq.bjjhwx.cn

================================================================================
来源：http://yh.colortex.cn

[L01] 发送 GET 请求
来源：http://yl.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lb.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hp.asd995.cn

JS:   await fetch(url)
来源：http://xf.bookmarksfly.cn

TS:   await fetch(url)
来源：http://ld.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jz.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://wl.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rs.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rh.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://hq.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sz.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bk.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kh.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ix.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://km.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://or.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xm.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wz.lnxyls.cn

[L03] 设置自定义请求头
来源：http://kl.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jo.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yp.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tg.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://di.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qs.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://se.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://px.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jt.panjiajie.cn

[L04] 设置超时
来源：http://nw.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://mv.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rk.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vy.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ug.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://az.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hx.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ub.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://fn.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ce.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ln.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ud.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://so.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lo.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://er.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rv.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wk.nszjky.cn

[L06] 解析响应为 JSON
来源：http://bo.hahajie.cn

Py:   resp.json()
来源：http://jz.colortex.cn

PHP:  json_decode($body, true);
来源：http://uv.szsharing.cn

JS:   await resp.json()
来源：http://up.muxihuayi.cn

TS:   await resp.json()
来源：http://wi.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ot.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wq.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://aw.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ve.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://yk.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bj.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uo.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://ti.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://ys.shxzskj.cn

Java: resp.statusCode()
来源：http://gw.bjjhwx.cn

Go:   resp.StatusCode
来源：http://wb.nszjky.cn

Ruby: resp.code.to_i
来源：http://hb.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://uj.szxytkj.cn

[L08] 并发请求多个地址
来源：http://pd.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uu.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://qp.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kt.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vv.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eo.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vr.shtwfgs.cn

================================================================================
来源：http://yf.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://wx.asd995.cn

================================================================================
来源：http://jw.colortex.cn

[M01] 读取命令行参数
来源：http://mw.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://of.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://pb.huanxung.cn

JS:   process.argv.slice(2)
来源：http://fi.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://mq.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://ee.asd995.cn

Go:   os.Args[1:]
来源：http://hk.haigaiapp.cn

Ruby: ARGV
来源：http://la.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://ru.haigaiapp.cn

[M02] 读取环境变量
来源：http://gl.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ca.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mz.haigaiapp.cn

JS:   process.env.HOME
来源：http://pb.nszjky.cn

TS:   process.env.HOME
来源：http://lr.newstarts.cn

Java: System.getenv("HOME")
来源：http://kq.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://et.asd995.cn

Ruby: ENV["HOME"]
来源：http://cf.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://if.521024.cn

[M03] 执行外部命令
来源：http://fw.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ne.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lq.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oi.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nh.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tb.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nf.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://fe.lnxyls.cn

[M04] 获取当前工作目录
来源：http://jw.shxzskj.cn

Py:   os.getcwd()
来源：http://qi.colortex.cn

PHP:  getcwd();
来源：http://vr.shxzskj.cn

JS:   process.cwd()
来源：http://st.hahajie.cn

TS:   process.cwd()
来源：http://im.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://il.521024.cn

Go:   os.Getwd()
来源：http://za.bjjhwx.cn

Ruby: Dir.pwd
来源：http://oh.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xt.yuntaijiaju.cn

[M05] 设置退出码
来源：http://fe.jctech888.com.cn

Py:   sys.exit(1)
来源：http://sn.panjiajie.cn

PHP:  exit(1);
来源：http://vw.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://ke.muxihuayi.cn

TS:   process.exit(1)
来源：http://wv.haigaiapp.cn

Java: System.exit(1)
来源：http://ru.szxytkj.cn

Go:   os.Exit(1)
来源：http://rn.nicolike.cn

Ruby: exit 1
来源：http://an.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gs.hahajie.cn

[M06] 向标准错误输出
来源：http://pn.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://qu.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://na.chemitech.net.cn

JS:   console.error("err")
来源：http://ay.newstarts.cn

TS:   console.error("err")
来源：http://sq.lnxyls.cn

Java: System.err.println("err")
来源：http://qu.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qg.huixinmuqiang.cn

Ruby: warn "err"
来源：http://gi.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://kg.szsharing.cn

[M07] 判断是否为主入口
来源：http://gp.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://mj.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jx.bjjhwx.cn

JS:   require.main === module
来源：http://uy.bookmarksfly.cn

TS:   require.main === module
来源：http://jc.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://gh.asd995.cn

Go:   func main()
来源：http://ch.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cg.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://ol.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://fi.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://rw.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://tz.szxytkj.cn

JS:   process.platform;  process.version
来源：http://pd.nszjky.cn

TS:   process.platform;  process.version
来源：http://nv.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ws.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zi.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zs.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xq.nicolike.cn

================================================================================
来源：http://az.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ho.shxzukj.cn

================================================================================
来源：http://qq.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://mb.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ip.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://it.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qg.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ko.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aq.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://kl.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qw.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ss.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://il.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ns.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sy.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://of.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xm.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wt.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://gv.huixinmuqiang.cn

Ruby: arr.sort
来源：http://fg.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xd.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://hd.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xd.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://dk.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ku.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ij.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wp.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ca.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yu.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tu.shtwfgs.cn

[N04] 斐波那契数列
来源：http://kt.bookmarksfly.cn


<!-- 参考信息 -->