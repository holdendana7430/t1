代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gf.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vl.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qw.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sh.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vz.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lv.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://da.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://iz.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dm.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wk.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://tz.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vd.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://sh.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jg.shxzskj.cn

[J06] 计算两时间之差
来源：http://pa.521024.cn

Py:   (end - start).total_seconds()
来源：http://xd.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://jw.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://el.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://za.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bl.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://vj.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://qx.521024.cn

C#:   (end - start).TotalSeconds
来源：http://bt.yuexingan06.cn

[J07] 比较两个日期
来源：http://iq.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://fj.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rr.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yl.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ik.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zk.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xx.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ny.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://bb.colortex.cn

[J08] 提取年月日与星期
来源：http://gm.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rf.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fj.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bh.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gy.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rj.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xm.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nk.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qe.huanxung.cn

[J09] 时区处理
来源：http://xf.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ct.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bf.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bk.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mb.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sl.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mo.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ri.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ki.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://vs.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uz.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iq.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yu.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xq.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pc.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lp.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ez.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ae.jianghongdianzi.cn

================================================================================
来源：http://yx.chemitech.net.cn

K. JSON 与序列化
来源：http://me.yuntaijiaju.cn

================================================================================
来源：http://nu.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://tt.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jl.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qq.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://xe.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ev.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nt.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://pi.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://da.szsharing.cn

[K02] JSON 字符串转对象
来源：http://qx.shxzukj.cn

Py:   json.loads(s)
来源：http://mp.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gl.colortex.cn

JS:   JSON.parse(s)
来源：http://ry.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://ao.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wb.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://df.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://fh.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://av.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ja.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zw.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gc.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://if.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tz.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qd.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rd.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jn.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ew.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://yi.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lx.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ow.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nb.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ma.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ff.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ff.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ul.shtwfgs.cn

[K05] 深拷贝对象
来源：http://rp.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://nh.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://le.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://bj.lnxyls.cn

TS:   structuredClone(obj)
来源：http://aa.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qt.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ry.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vu.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hp.asd995.cn

[K06] 解析 URL 查询串
来源：http://lh.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ro.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xx.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bo.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wx.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ve.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://df.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yg.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kn.asd995.cn

[K07] 进制转换
来源：http://yc.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mg.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nq.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xd.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fh.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eh.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kc.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nu.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://um.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://oc.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://pe.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pa.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://kw.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://qv.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ej.lnxyls.cn

Go:   encoding/gob
来源：http://hz.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://zr.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wg.chemitech.net.cn

================================================================================
来源：http://kf.hnjuh.cn

L. 网络请求
来源：http://ep.muxihuayi.cn

================================================================================
来源：http://nm.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://eb.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fy.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vz.nszjky.cn

JS:   await fetch(url)
来源：http://ij.hahajie.cn

TS:   await fetch(url)
来源：http://lf.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yr.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://zk.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://in.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cn.gzmigu.cn

[L02] 发送 POST JSON
来源：http://tz.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ao.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tq.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uc.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hx.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://je.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ne.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vh.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vb.shxzskj.cn

[L03] 设置自定义请求头
来源：http://xc.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gq.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qc.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wt.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bq.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wj.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fu.panjiajie.cn

[L04] 设置超时
来源：http://xf.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://wi.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ki.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://be.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ip.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jg.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wr.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zb.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ic.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://hn.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ta.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://le.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gb.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fp.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ev.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fz.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rq.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jy.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://my.asd995.cn

Py:   resp.json()
来源：http://vd.szsharing.cn

PHP:  json_decode($body, true);
来源：http://kg.wgjwhj.cn

JS:   await resp.json()
来源：http://el.yuntaijiaju.cn

TS:   await resp.json()
来源：http://qu.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wv.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://jn.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gp.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://do.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xa.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fj.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://gk.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://dr.jctech888.com.cn

Java: resp.statusCode()
来源：http://zv.colortex.cn

Go:   resp.StatusCode
来源：http://ia.hahajie.cn

Ruby: resp.code.to_i
来源：http://gr.521024.cn

C#:   (int)resp.StatusCode
来源：http://yq.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://oa.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wn.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://kq.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sv.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zz.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yt.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sp.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lf.shxzskj.cn

================================================================================
来源：http://kq.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://ab.szxytkj.cn

================================================================================
来源：http://ks.shxzskj.cn

[M01] 读取命令行参数
来源：http://ci.nicolike.cn

Py:   sys.argv[1:]
来源：http://gv.nicolike.cn

PHP:  $argv;  $argc;
来源：http://vp.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://nb.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://pc.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://rg.wgjwhj.cn

Go:   os.Args[1:]
来源：http://ub.yuexingan06.cn

Ruby: ARGV
来源：http://on.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://jm.yuexingan06.cn

[M02] 读取环境变量
来源：http://yx.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://op.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://av.muxihuayi.cn

JS:   process.env.HOME
来源：http://zs.gzmigu.cn

TS:   process.env.HOME
来源：http://ag.lnxyls.cn

Java: System.getenv("HOME")
来源：http://vi.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ri.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://yc.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ik.shxzskj.cn

[M03] 执行外部命令
来源：http://kl.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gy.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ly.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xw.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ws.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lp.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rv.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ne.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://oi.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://uy.muxihuayi.cn

Py:   os.getcwd()
来源：http://uc.panjiajie.cn

PHP:  getcwd();
来源：http://hy.gzmigu.cn

JS:   process.cwd()
来源：http://zn.lnxyls.cn

TS:   process.cwd()
来源：http://lw.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://np.bjjhwx.cn

Go:   os.Getwd()
来源：http://ll.huixiangedu.cn

Ruby: Dir.pwd
来源：http://tf.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://js.nszjky.cn

[M05] 设置退出码
来源：http://mn.huanxung.cn

Py:   sys.exit(1)
来源：http://sz.hahajie.cn

PHP:  exit(1);
来源：http://ax.hahajie.cn

JS:   process.exit(1)
来源：http://jk.9csxet.cn

TS:   process.exit(1)
来源：http://gj.521024.cn

Java: System.exit(1)
来源：http://cl.hnjuh.cn

Go:   os.Exit(1)
来源：http://go.hnjuh.cn

Ruby: exit 1
来源：http://ph.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nn.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ya.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://tk.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qr.szsharing.cn

JS:   console.error("err")
来源：http://il.521024.cn

TS:   console.error("err")
来源：http://jg.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://vw.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dt.huixinmuqiang.cn

Ruby: warn "err"
来源：http://vg.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://hg.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://ff.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://dp.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dk.chemitech.net.cn

JS:   require.main === module
来源：http://bo.shxzukj.cn

TS:   require.main === module
来源：http://gz.newstarts.cn

Java: public static void main(String[] args)
来源：http://mv.nszjky.cn

Go:   func main()
来源：http://xl.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oh.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://ae.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://bm.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://nz.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://gy.szsharing.cn

JS:   process.platform;  process.version
来源：http://pz.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://pj.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ym.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hi.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zr.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yy.huanxung.cn

================================================================================
来源：http://fj.newstarts.cn

N. 数据结构与算法
来源：http://ej.shxzukj.cn

================================================================================
来源：http://br.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://pm.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rz.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zr.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jq.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gt.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fe.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://xd.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cm.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ly.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://bj.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://we.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ye.521024.cn


<!-- 参考信息 -->