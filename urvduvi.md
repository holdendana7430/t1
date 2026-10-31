代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gd.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lw.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xn.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xp.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nh.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gt.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://iy.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://cp.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cq.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fs.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gu.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://vf.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xp.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://gm.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xa.muxihuayi.cn

[J06] 计算两时间之差
来源：http://zz.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://mp.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://vq.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nf.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mj.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dk.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://dt.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://kf.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://ke.szsharing.cn

[J07] 比较两个日期
来源：http://qf.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://sn.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pp.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nd.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ij.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ql.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://og.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://gq.gzmigu.cn

[J08] 提取年月日与星期
来源：http://lb.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ty.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nf.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://so.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gk.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zd.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iz.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jb.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fy.hnjuh.cn

[J09] 时区处理
来源：http://nj.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tx.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eq.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jh.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sn.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zw.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kk.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wd.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wx.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://ay.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nd.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gl.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wn.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mn.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qu.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bp.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://al.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fi.haigaiapp.cn

================================================================================
来源：http://pd.huanxung.cn

K. JSON 与序列化
来源：http://jc.colortex.cn

================================================================================
来源：http://rr.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://ly.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ie.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mi.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://qv.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://zu.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://so.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://pm.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ei.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wg.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ae.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ym.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cs.nicolike.cn

JS:   JSON.parse(s)
来源：http://kc.nicolike.cn

TS:   JSON.parse(s)
来源：http://ff.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uo.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://qr.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://uh.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ho.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hq.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lu.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mc.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pp.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pq.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mv.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cg.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hy.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yh.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ka.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bn.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uq.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uv.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://st.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://am.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xa.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iw.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://or.colortex.cn

[K05] 深拷贝对象
来源：http://qd.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://jl.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://hc.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://ld.shxzukj.cn

TS:   structuredClone(obj)
来源：http://mq.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bc.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ac.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gm.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xy.huanxung.cn

[K06] 解析 URL 查询串
来源：http://hp.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oi.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fw.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jb.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mm.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oq.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ez.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xa.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lh.hahajie.cn

[K07] 进制转换
来源：http://ra.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://it.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mh.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rx.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nq.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qg.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gp.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jf.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ct.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://gi.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://qv.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nf.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://kh.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://vw.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vk.gzmigu.cn

Go:   encoding/gob
来源：http://bu.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://zu.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oc.haigaiapp.cn

================================================================================
来源：http://yr.bookmarksfly.cn

L. 网络请求
来源：http://ig.newstarts.cn

================================================================================
来源：http://tg.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://tn.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nn.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rf.hnjuh.cn

JS:   await fetch(url)
来源：http://bd.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://ja.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rh.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ho.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://up.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ra.asd995.cn

[L02] 发送 POST JSON
来源：http://ut.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mq.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zg.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gn.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gb.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cv.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sn.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://id.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://df.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://an.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ox.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://be.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://je.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ay.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nc.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dh.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pd.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tw.yuexingan06.cn

[L04] 设置超时
来源：http://ku.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://td.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://li.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tr.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ye.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nh.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fs.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ur.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ot.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://mf.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oi.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gz.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xm.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ya.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yx.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tn.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://io.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vz.521024.cn

[L06] 解析响应为 JSON
来源：http://cg.9csxet.cn

Py:   resp.json()
来源：http://bi.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://qs.newstarts.cn

JS:   await resp.json()
来源：http://bt.jianghongdianzi.cn

TS:   await resp.json()
来源：http://mi.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wb.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pw.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://et.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xt.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://wo.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gx.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://in.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ps.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://zl.huixiangedu.cn

Java: resp.statusCode()
来源：http://zq.muxihuayi.cn

Go:   resp.StatusCode
来源：http://gt.newstarts.cn

Ruby: resp.code.to_i
来源：http://qc.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://im.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://zl.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cm.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://zb.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pb.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cf.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fx.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kl.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uw.haigaiapp.cn

================================================================================
来源：http://fj.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://kh.panjiajie.cn

================================================================================
来源：http://fi.panjiajie.cn

[M01] 读取命令行参数
来源：http://wr.szsharing.cn

Py:   sys.argv[1:]
来源：http://nf.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://zn.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://oi.521024.cn

TS:   process.argv.slice(2)
来源：http://ai.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://vv.jctech888.com.cn

Go:   os.Args[1:]
来源：http://bk.jctech888.com.cn

Ruby: ARGV
来源：http://us.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://sw.521024.cn

[M02] 读取环境变量
来源：http://js.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://zh.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bi.shxzskj.cn

JS:   process.env.HOME
来源：http://tu.bjjhwx.cn

TS:   process.env.HOME
来源：http://vg.shxzskj.cn

Java: System.getenv("HOME")
来源：http://xf.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ts.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://pj.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yu.shtwfgs.cn

[M03] 执行外部命令
来源：http://fo.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bj.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dh.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vu.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wu.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mg.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fw.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yd.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://iz.colortex.cn

[M04] 获取当前工作目录
来源：http://dq.huanxung.cn

Py:   os.getcwd()
来源：http://xj.shtwfgs.cn

PHP:  getcwd();
来源：http://aw.szsharing.cn

JS:   process.cwd()
来源：http://md.huixiangedu.cn

TS:   process.cwd()
来源：http://tt.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ai.shxzskj.cn

Go:   os.Getwd()
来源：http://xu.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://hx.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://un.shxzskj.cn

[M05] 设置退出码
来源：http://xr.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://lt.nicolike.cn

PHP:  exit(1);
来源：http://xp.newstarts.cn

JS:   process.exit(1)
来源：http://tf.colortex.cn

TS:   process.exit(1)
来源：http://eb.szxytkj.cn

Java: System.exit(1)
来源：http://ha.panjiajie.cn

Go:   os.Exit(1)
来源：http://xr.jctech888.com.cn

Ruby: exit 1
来源：http://im.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qq.gzmigu.cn

[M06] 向标准错误输出
来源：http://ax.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://rz.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xb.bjjhwx.cn

JS:   console.error("err")
来源：http://zq.huixinmuqiang.cn

TS:   console.error("err")
来源：http://gt.9csxet.cn

Java: System.err.println("err")
来源：http://sh.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ol.bookmarksfly.cn

Ruby: warn "err"
来源：http://ji.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://dp.shxzukj.cn

[M07] 判断是否为主入口
来源：http://im.colortex.cn

Py:   if __name__ == "__main__":
来源：http://uu.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ba.bjjhwx.cn

JS:   require.main === module
来源：http://zd.wgjwhj.cn

TS:   require.main === module
来源：http://zh.hnjuh.cn

Java: public static void main(String[] args)
来源：http://ma.wgjwhj.cn

Go:   func main()
来源：http://go.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uy.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://mi.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://ch.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://fy.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ys.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ma.hnjuh.cn

TS:   process.platform;  process.version
来源：http://ro.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ok.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wa.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://og.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://me.bjjhwx.cn

================================================================================
来源：http://gv.huixinmuqiang.cn

N. 数据结构与算法
来源：http://fd.shxzskj.cn

================================================================================
来源：http://wz.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://uo.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qp.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yc.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dh.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ht.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bf.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://wa.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sb.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lh.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://gs.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tv.gzmigu.cn


<!-- 参考信息 -->