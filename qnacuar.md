代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://wc.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://km.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bx.muxihuayi.cn

[I05] 按正则拆分
来源：http://vx.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fg.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://su.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://yj.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://jo.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ug.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ud.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uj.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xp.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yi.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vt.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cj.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gm.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ik.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jz.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vq.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vn.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sy.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://xz.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tx.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pz.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bw.gzmigu.cn

TS:   /error/gim
来源：http://uv.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://px.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cv.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://tg.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ii.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://dv.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nn.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iz.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gb.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ec.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ii.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fx.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hw.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bl.panjiajie.cn

================================================================================
来源：http://xu.hahajie.cn

J. 日期与时间
来源：http://iy.szxytkj.cn

================================================================================
来源：http://ch.haigaiapp.cn

[J01] 获取当前时间
来源：http://mz.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ob.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fu.colortex.cn

JS:   new Date();  Date.now()
来源：http://na.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://nd.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ns.bookmarksfly.cn

Go:   time.Now()
来源：http://gf.bjjhwx.cn

Ruby: Time.now
来源：http://sw.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://co.hahajie.cn

[J02] 格式化输出
来源：http://ls.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ic.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://up.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://od.chemitech.net.cn

TS:   d.toISOString()
来源：http://so.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://we.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sl.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iv.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sg.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://pd.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ix.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://km.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://vw.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ad.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iu.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hc.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://jf.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yi.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://qh.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ui.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jg.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ya.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nj.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kq.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vc.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tn.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fb.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://hq.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://sc.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qz.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pe.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://ke.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tm.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://hq.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kx.nicolike.cn

[J06] 计算两时间之差
来源：http://rq.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://wo.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://br.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rj.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lh.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://ja.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://zz.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ka.jctech888.com.cn

[J07] 比较两个日期
来源：http://ji.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://gi.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ky.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iq.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vt.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nw.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kz.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ly.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://dq.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://fy.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fj.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gf.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pa.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yb.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nm.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wj.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ay.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sf.hnjuh.cn

[J09] 时区处理
来源：http://fl.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wo.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pt.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://my.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ln.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xc.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pu.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tj.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://es.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://nc.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nv.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pn.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ju.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lj.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ea.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bm.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://il.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ya.yuntaijiaju.cn

================================================================================
来源：http://kd.huanxung.cn

K. JSON 与序列化
来源：http://zx.bookmarksfly.cn

================================================================================
来源：http://bk.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://cb.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ck.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oc.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://fd.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://zr.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://of.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://kd.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mo.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fa.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ys.lnxyls.cn

Py:   json.loads(s)
来源：http://md.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zu.huanxung.cn

JS:   JSON.parse(s)
来源：http://ma.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://ic.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zx.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ox.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://nx.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gw.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://bk.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://am.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://au.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bb.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bw.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yc.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xm.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ox.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ix.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ax.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sq.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ty.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uj.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zm.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zb.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uu.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ac.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ti.521024.cn

[K05] 深拷贝对象
来源：http://gn.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://ow.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://eu.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://pw.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ya.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ot.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jh.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tl.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://df.asd995.cn

[K06] 解析 URL 查询串
来源：http://dj.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dn.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pp.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://db.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ps.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qa.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ht.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xv.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sp.lnxyls.cn

[K07] 进制转换
来源：http://zv.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lg.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jt.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fw.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hm.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dy.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uv.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qa.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rx.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://sz.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://gk.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://by.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://xg.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://xp.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://al.lnxyls.cn

Go:   encoding/gob
来源：http://tz.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://nf.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jl.huixiangedu.cn

================================================================================
来源：http://vg.bookmarksfly.cn

L. 网络请求
来源：http://jf.huixiangedu.cn

================================================================================
来源：http://ws.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ca.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jr.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bz.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://pf.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://hg.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mz.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://jm.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://te.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pr.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ug.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ll.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://af.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mp.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pb.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dt.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ch.panjiajie.cn

[L03] 设置自定义请求头
来源：http://tb.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://op.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ag.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://br.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jq.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://co.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vq.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xo.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mu.jctech888.com.cn

[L04] 设置超时
来源：http://ab.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ve.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oa.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sw.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ku.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hj.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mh.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sf.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://if.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://uy.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zj.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ja.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://is.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hy.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jj.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gu.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pu.asd995.cn

[L06] 解析响应为 JSON
来源：http://uo.newstarts.cn

Py:   resp.json()
来源：http://hh.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://fh.wgjwhj.cn

JS:   await resp.json()
来源：http://xe.panjiajie.cn

TS:   await resp.json()
来源：http://yv.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fq.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://vq.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wj.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://me.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wg.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zn.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://wm.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://hf.nicolike.cn

Java: resp.statusCode()
来源：http://nd.bjjhwx.cn

Go:   resp.StatusCode
来源：http://tn.521024.cn

Ruby: resp.code.to_i
来源：http://wk.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://fd.szsharing.cn

[L08] 并发请求多个地址
来源：http://ko.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://at.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://vp.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nw.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pq.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uw.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://td.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ek.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ui.nszjky.cn

================================================================================
来源：http://gz.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://yp.shxzskj.cn

================================================================================
来源：http://rp.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://im.nszjky.cn

Py:   sys.argv[1:]
来源：http://ud.szsharing.cn

PHP:  $argv;  $argc;
来源：http://bs.newstarts.cn

JS:   process.argv.slice(2)
来源：http://pp.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://dz.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://ia.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://sp.hnjuh.cn

Ruby: ARGV
来源：http://bj.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://zw.shtwfgs.cn

[M02] 读取环境变量
来源：http://uq.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://jh.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yu.gzmigu.cn

JS:   process.env.HOME
来源：http://yf.asd995.cn

TS:   process.env.HOME
来源：http://tr.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://ag.muxihuayi.cn


<!-- 参考信息 -->