代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://vp.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jd.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.haigaiapp.cn

[I05] 按正则拆分
来源：http://go.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ce.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ca.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://id.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://th.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://pg.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://go.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sq.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lu.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ma.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kg.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://si.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uy.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yt.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wk.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cj.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jj.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eb.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://gh.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://az.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hs.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ki.shtwfgs.cn

TS:   /error/gim
来源：http://vz.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rw.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://id.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://xo.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bw.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://ac.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eh.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fe.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bc.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://df.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pu.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uh.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bb.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dg.colortex.cn

================================================================================
来源：http://wk.huixinmuqiang.cn

J. 日期与时间
来源：http://yk.jianghongdianzi.cn

================================================================================
来源：http://ve.wgjwhj.cn

[J01] 获取当前时间
来源：http://zy.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://if.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xg.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://si.nicolike.cn

TS:   new Date();  Date.now()
来源：http://dr.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dw.gzmigu.cn

Go:   time.Now()
来源：http://dv.huanxung.cn

Ruby: Time.now
来源：http://fi.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dd.wgjwhj.cn

[J02] 格式化输出
来源：http://ni.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rh.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zk.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xi.wgjwhj.cn

TS:   d.toISOString()
来源：http://vb.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tc.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iu.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uv.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bz.panjiajie.cn

[J03] 字符串解析为日期
来源：http://hp.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gm.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ft.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://zt.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uu.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zp.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://vl.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xv.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://eu.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mb.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ml.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ru.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nk.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qr.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gg.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ey.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wr.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://cj.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://tx.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wj.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ua.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vf.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zy.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://zk.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://on.lnxyls.cn

[J06] 计算两时间之差
来源：http://km.521024.cn

Py:   (end - start).total_seconds()
来源：http://ln.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://sg.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ps.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lz.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aj.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://mo.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://mf.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://mg.szxytkj.cn

[J07] 比较两个日期
来源：http://vt.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://pc.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jp.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cr.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://if.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xx.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://se.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sk.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://tx.newstarts.cn

[J08] 提取年月日与星期
来源：http://we.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hy.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gc.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fk.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lu.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hr.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qb.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wa.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.haigaiapp.cn

[J09] 时区处理
来源：http://vj.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fc.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ai.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wx.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ga.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ib.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pj.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ef.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ze.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://xs.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xy.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fl.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tu.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eh.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fb.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ey.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ha.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mk.shxzukj.cn

================================================================================
来源：http://sj.yuntaijiaju.cn

K. JSON 与序列化
来源：http://lz.chemitech.net.cn

================================================================================
来源：http://vg.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://hr.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ke.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rp.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://ev.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://lb.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ca.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://rk.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bn.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pn.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://gr.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ha.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dr.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://jm.nszjky.cn

TS:   JSON.parse(s)
来源：http://nk.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xz.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://bs.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://qo.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rg.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ol.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xk.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yj.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uf.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sm.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tj.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mm.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sp.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sn.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://zw.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yz.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lk.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iu.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nw.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tr.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://in.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://je.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fj.newstarts.cn

[K05] 深拷贝对象
来源：http://am.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://gv.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://cy.newstarts.cn

JS:   structuredClone(obj)
来源：http://rg.szsharing.cn

TS:   structuredClone(obj)
来源：http://ms.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kw.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qh.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qx.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ag.colortex.cn

[K06] 解析 URL 查询串
来源：http://jj.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://te.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://it.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://as.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ax.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iy.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://om.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jf.haigaiapp.cn

[K07] 进制转换
来源：http://pt.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ai.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yt.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cx.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gn.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sk.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fv.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kc.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nq.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sg.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ip.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wj.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://pe.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://wr.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.haigaiapp.cn

Go:   encoding/gob
来源：http://vv.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://wp.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pn.panjiajie.cn

================================================================================
来源：http://je.haigaiapp.cn

L. 网络请求
来源：http://zy.wgjwhj.cn

================================================================================
来源：http://kg.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://dr.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qa.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ll.bookmarksfly.cn

JS:   await fetch(url)
来源：http://hv.huixiangedu.cn

TS:   await fetch(url)
来源：http://pp.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rv.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://la.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yv.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gf.newstarts.cn

[L02] 发送 POST JSON
来源：http://gl.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ju.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ov.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lp.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ah.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uy.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gu.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tq.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ah.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://wl.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xh.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zr.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ti.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yl.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fs.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jw.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wc.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sr.shxzukj.cn

[L04] 设置超时
来源：http://nx.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://uy.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nt.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ws.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nx.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ei.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uq.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qy.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xi.hahajie.cn

[L05] 上传文件（multipart）
来源：http://my.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oi.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zd.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://df.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nd.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://go.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hp.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ag.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kp.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://em.huixinmuqiang.cn

Py:   resp.json()
来源：http://oj.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://jo.jctech888.com.cn

JS:   await resp.json()
来源：http://ou.nicolike.cn

TS:   await resp.json()
来源：http://eh.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mh.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mm.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://me.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ol.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ab.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://to.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://kx.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://yj.shxzukj.cn

Java: resp.statusCode()
来源：http://ai.bjjhwx.cn

Go:   resp.StatusCode
来源：http://zh.colortex.cn

Ruby: resp.code.to_i
来源：http://tc.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://pr.shxzskj.cn

[L08] 并发请求多个地址
来源：http://zn.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hh.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://ux.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wo.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xs.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vc.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kv.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fq.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wy.nicolike.cn

================================================================================
来源：http://bn.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://ty.yuexingan06.cn

================================================================================
来源：http://to.bjjhwx.cn

[M01] 读取命令行参数
来源：http://is.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://qz.newstarts.cn

PHP:  $argv;  $argc;
来源：http://cm.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://wr.521024.cn

TS:   process.argv.slice(2)
来源：http://dy.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://cg.521024.cn

Go:   os.Args[1:]
来源：http://kn.jctech888.com.cn

Ruby: ARGV
来源：http://ke.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://vn.huixiangedu.cn

[M02] 读取环境变量
来源：http://lp.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://pd.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nd.chemitech.net.cn

JS:   process.env.HOME
来源：http://ub.haigaiapp.cn

TS:   process.env.HOME
来源：http://rb.panjiajie.cn

Java: System.getenv("HOME")
来源：http://hk.lnxyls.cn


<!-- 参考信息 -->