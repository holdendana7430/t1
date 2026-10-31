代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zt.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gt.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gj.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zy.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rr.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://zd.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ly.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yo.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gk.yuntaijiaju.cn

TS:   /error/gim
来源：http://io.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://st.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ez.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://rx.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ok.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://ri.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://er.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zm.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eq.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gg.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kb.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://db.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ca.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mt.hahajie.cn

================================================================================
来源：http://le.szsharing.cn

J. 日期与时间
来源：http://nu.yuntaijiaju.cn

================================================================================
来源：http://fy.jctech888.com.cn

[J01] 获取当前时间
来源：http://pe.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vb.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fb.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://aq.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://ax.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qb.huanxung.cn

Go:   time.Now()
来源：http://ki.shtwfgs.cn

Ruby: Time.now
来源：http://dj.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ta.panjiajie.cn

[J02] 格式化输出
来源：http://ti.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://za.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iy.lnxyls.cn

TS:   d.toISOString()
来源：http://aw.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wb.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zu.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yt.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rw.shxzskj.cn

[J03] 字符串解析为日期
来源：http://hv.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xa.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://om.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://be.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://jk.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nl.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tw.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://nc.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hq.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://pb.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sk.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iq.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zp.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://az.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lu.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ow.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://od.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kt.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://vm.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://eu.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://or.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ne.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://af.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ll.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eg.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://vi.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bo.521024.cn

[J06] 计算两时间之差
来源：http://fe.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://jr.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://vy.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ch.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tp.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dj.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://kv.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://px.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ad.wgjwhj.cn

[J07] 比较两个日期
来源：http://xg.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://gd.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zl.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ss.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zb.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oh.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lc.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://gx.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://an.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gq.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kt.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tk.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vj.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ql.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jl.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ci.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://da.hnjuh.cn

[J09] 时区处理
来源：http://wz.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xc.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sp.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eg.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iz.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lr.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zz.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nc.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://re.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://rc.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dh.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lv.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aj.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://br.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pu.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hi.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xq.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ys.shxzskj.cn

================================================================================
来源：http://zc.yuexingan06.cn

K. JSON 与序列化
来源：http://zm.asd995.cn

================================================================================
来源：http://ez.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://kh.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qp.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dh.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://hg.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://mt.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zr.9csxet.cn

Go:   json.Marshal(obj)
来源：http://jv.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vm.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ym.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://kq.haigaiapp.cn

Py:   json.loads(s)
来源：http://tw.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ny.nszjky.cn

JS:   JSON.parse(s)
来源：http://zq.shxzukj.cn

TS:   JSON.parse(s)
来源：http://wk.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bz.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://rs.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://hl.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mr.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://lv.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bi.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tz.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://my.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gv.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tr.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://my.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ok.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://op.szsharing.cn

[K04] 读取 JSON 文件
来源：http://zb.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ot.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ep.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://le.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oy.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yj.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://um.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uf.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mf.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://lk.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://sb.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://sc.shxzukj.cn

JS:   structuredClone(obj)
来源：http://ju.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://ct.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ei.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ty.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vc.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://la.9csxet.cn

[K06] 解析 URL 查询串
来源：http://at.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://od.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://em.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uc.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lz.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vm.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://to.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zi.huanxung.cn

[K07] 进制转换
来源：http://tr.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://er.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fp.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jh.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ue.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ex.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qy.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://se.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mx.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://ib.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://kn.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://po.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://yq.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://db.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ni.huanxung.cn

Go:   encoding/gob
来源：http://es.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://db.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bk.szxytkj.cn

================================================================================
来源：http://dz.wgjwhj.cn

L. 网络请求
来源：http://yj.colortex.cn

================================================================================
来源：http://ci.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://bk.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vw.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://br.huixiangedu.cn

JS:   await fetch(url)
来源：http://cx.gzmigu.cn

TS:   await fetch(url)
来源：http://eb.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ch.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://fm.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jw.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kh.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://vh.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gc.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eg.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vh.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wf.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nk.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pf.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cs.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://so.hnjuh.cn

[L03] 设置自定义请求头
来源：http://wt.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zn.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ay.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dr.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gc.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gz.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pf.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://da.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ym.bookmarksfly.cn

[L04] 设置超时
来源：http://pw.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://xr.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://st.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bs.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tw.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zn.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gd.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kz.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ed.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://rx.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fg.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sj.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ix.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sp.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bl.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vw.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hi.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ur.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://ax.shxzukj.cn

Py:   resp.json()
来源：http://np.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://tz.asd995.cn

JS:   await resp.json()
来源：http://mk.gzmigu.cn

TS:   await resp.json()
来源：http://pz.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://de.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jo.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ib.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xq.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://xr.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jo.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jh.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://dr.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://ng.yuexingan06.cn

Java: resp.statusCode()
来源：http://yv.shxzukj.cn

Go:   resp.StatusCode
来源：http://la.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://lg.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://cg.colortex.cn

[L08] 并发请求多个地址
来源：http://gd.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wt.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://bo.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gc.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://da.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ow.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kt.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jb.huixinmuqiang.cn

================================================================================
来源：http://lx.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://ii.hnjuh.cn

================================================================================
来源：http://ur.gzmigu.cn

[M01] 读取命令行参数
来源：http://qu.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://qt.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://yc.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ol.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://ju.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://id.panjiajie.cn

Go:   os.Args[1:]
来源：http://xz.bjjhwx.cn

Ruby: ARGV
来源：http://sr.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://nl.bookmarksfly.cn

[M02] 读取环境变量
来源：http://yh.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://mb.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hr.haigaiapp.cn

JS:   process.env.HOME
来源：http://bj.bookmarksfly.cn

TS:   process.env.HOME
来源：http://mu.colortex.cn

Java: System.getenv("HOME")
来源：http://vc.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://at.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vi.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ln.haigaiapp.cn

[M03] 执行外部命令
来源：http://dd.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pe.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hc.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fm.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gd.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vv.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wx.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://au.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://um.colortex.cn

[M04] 获取当前工作目录
来源：http://ga.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://mf.huixiangedu.cn

PHP:  getcwd();
来源：http://xr.szxytkj.cn

JS:   process.cwd()
来源：http://aj.lnxyls.cn


<!-- 参考信息 -->