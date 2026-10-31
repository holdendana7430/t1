代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xb.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://nv.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gn.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ne.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bd.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sf.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cy.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dt.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xk.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fd.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://sp.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://zi.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://my.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pg.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ji.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://on.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cd.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://ew.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://la.wgjwhj.cn

[J06] 计算两时间之差
来源：http://ty.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://vj.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://gv.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://st.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kc.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bv.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ym.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://hl.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://cj.hahajie.cn

[J07] 比较两个日期
来源：http://tv.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://jz.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yk.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nf.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oc.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pu.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xg.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sh.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://yc.newstarts.cn

[J08] 提取年月日与星期
来源：http://sf.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hc.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ls.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ut.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yq.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://am.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gc.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nk.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ir.wgjwhj.cn

[J09] 时区处理
来源：http://du.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ik.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jf.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pg.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qv.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ue.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ll.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cp.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gn.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://gq.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://up.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tx.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zo.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dp.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kt.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fy.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ry.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nn.chemitech.net.cn

================================================================================
来源：http://jp.hnjuh.cn

K. JSON 与序列化
来源：http://bh.wgjwhj.cn

================================================================================
来源：http://go.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://iu.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xb.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://io.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://lf.asd995.cn

TS:   JSON.stringify(obj)
来源：http://hg.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dy.nicolike.cn

Go:   json.Marshal(obj)
来源：http://oy.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jw.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dg.newstarts.cn

[K02] JSON 字符串转对象
来源：http://em.szxytkj.cn

Py:   json.loads(s)
来源：http://hn.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ta.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://km.nszjky.cn

TS:   JSON.parse(s)
来源：http://rk.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rr.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ra.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://ow.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://on.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://vz.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qh.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ay.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jp.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bw.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qx.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sq.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gx.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sz.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://tb.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gh.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://er.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nm.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fn.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qc.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://so.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fg.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vt.colortex.cn

[K05] 深拷贝对象
来源：http://tj.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://kp.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://fr.9csxet.cn

JS:   structuredClone(obj)
来源：http://be.521024.cn

TS:   structuredClone(obj)
来源：http://sa.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sg.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rb.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ru.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qe.9csxet.cn

[K06] 解析 URL 查询串
来源：http://zn.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ls.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eb.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yp.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ps.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ht.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fz.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yo.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xw.asd995.cn

[K07] 进制转换
来源：http://kn.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bt.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ho.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zs.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://te.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cb.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wg.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://df.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sp.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://jj.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://rf.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jo.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://kz.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://wr.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hi.yuexingan06.cn

Go:   encoding/gob
来源：http://lq.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://sb.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ws.yuexingan06.cn

================================================================================
来源：http://hm.521024.cn

L. 网络请求
来源：http://mn.lnxyls.cn

================================================================================
来源：http://uw.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://wa.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hh.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ik.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://cq.wgjwhj.cn

TS:   await fetch(url)
来源：http://kt.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ka.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ku.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yg.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gf.hahajie.cn

[L02] 发送 POST JSON
来源：http://wc.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lu.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tm.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wj.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://av.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pu.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ch.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xs.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qp.nicolike.cn

[L03] 设置自定义请求头
来源：http://iy.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iq.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lh.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ib.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pk.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cq.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ah.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iq.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ng.shxzukj.cn

[L04] 设置超时
来源：http://zj.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://ul.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hp.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ro.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gr.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gx.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cn.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yu.nszjky.cn

[L05] 上传文件（multipart）
来源：http://xi.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nw.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fr.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kf.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ki.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ly.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yp.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vh.521024.cn

[L06] 解析响应为 JSON
来源：http://ao.hahajie.cn

Py:   resp.json()
来源：http://nq.szsharing.cn

PHP:  json_decode($body, true);
来源：http://ho.panjiajie.cn

JS:   await resp.json()
来源：http://nl.huixiangedu.cn

TS:   await resp.json()
来源：http://rh.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ea.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xa.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://nv.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xs.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://tv.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ju.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mw.521024.cn

JS:   resp.ok;  resp.status
来源：http://gg.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://mg.hnjuh.cn

Java: resp.statusCode()
来源：http://im.yuexingan06.cn

Go:   resp.StatusCode
来源：http://to.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://xx.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://fe.hahajie.cn

[L08] 并发请求多个地址
来源：http://ge.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://un.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://hc.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gs.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xq.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kx.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tn.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hg.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rq.panjiajie.cn

================================================================================
来源：http://fj.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://fl.newstarts.cn

================================================================================
来源：http://eo.newstarts.cn

[M01] 读取命令行参数
来源：http://jk.newstarts.cn

Py:   sys.argv[1:]
来源：http://pp.szsharing.cn

PHP:  $argv;  $argc;
来源：http://gj.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://ls.colortex.cn

TS:   process.argv.slice(2)
来源：http://aj.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://jp.shtwfgs.cn

Go:   os.Args[1:]
来源：http://rb.huixiangedu.cn

Ruby: ARGV
来源：http://sw.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://rr.szxytkj.cn

[M02] 读取环境变量
来源：http://zv.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://wo.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tw.shxzskj.cn

JS:   process.env.HOME
来源：http://mp.nszjky.cn

TS:   process.env.HOME
来源：http://lo.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://gx.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gu.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://qn.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vk.hahajie.cn

[M03] 执行外部命令
来源：http://wi.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://np.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cu.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://os.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xo.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rh.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vk.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://tw.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://eg.bjjhwx.cn

Py:   os.getcwd()
来源：http://kn.muxihuayi.cn

PHP:  getcwd();
来源：http://li.huixinmuqiang.cn

JS:   process.cwd()
来源：http://sd.shxzskj.cn

TS:   process.cwd()
来源：http://nh.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://zx.chemitech.net.cn

Go:   os.Getwd()
来源：http://bp.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://kf.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://py.yuntaijiaju.cn

[M05] 设置退出码
来源：http://cv.gzmigu.cn

Py:   sys.exit(1)
来源：http://cg.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ab.wgjwhj.cn

JS:   process.exit(1)
来源：http://lp.haigaiapp.cn

TS:   process.exit(1)
来源：http://fe.nicolike.cn

Java: System.exit(1)
来源：http://iy.521024.cn

Go:   os.Exit(1)
来源：http://uq.nicolike.cn

Ruby: exit 1
来源：http://av.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jb.asd995.cn

[M06] 向标准错误输出
来源：http://cm.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://db.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ml.shxzskj.cn

JS:   console.error("err")
来源：http://gq.wgjwhj.cn

TS:   console.error("err")
来源：http://oe.chemitech.net.cn

Java: System.err.println("err")
来源：http://al.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ja.hnjuh.cn

Ruby: warn "err"
来源：http://cq.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://lu.newstarts.cn

[M07] 判断是否为主入口
来源：http://jt.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://dh.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://us.wgjwhj.cn

JS:   require.main === module
来源：http://dj.wgjwhj.cn

TS:   require.main === module
来源：http://ko.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://bc.yuntaijiaju.cn

Go:   func main()
来源：http://al.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mp.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://wv.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://qp.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://xq.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://zm.panjiajie.cn

JS:   process.platform;  process.version
来源：http://uz.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://ma.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rs.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fh.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wm.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mr.yuntaijiaju.cn

================================================================================
来源：http://nh.521024.cn

N. 数据结构与算法
来源：http://hm.shxzskj.cn

================================================================================
来源：http://dw.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://bs.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ng.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ca.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xe.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://io.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cu.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://pe.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cs.yuexingan06.cn


<!-- 参考信息 -->