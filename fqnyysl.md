代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://zr.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oa.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://no.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://qu.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://yq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sl.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fu.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dv.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oq.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ce.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://br.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gw.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tk.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ec.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oi.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ak.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://he.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ts.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ff.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://se.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ia.chemitech.net.cn

TS:   /error/gim
来源：http://he.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gm.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pn.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://uw.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sk.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://is.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lu.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gr.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fw.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sw.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iu.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nk.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mn.wgjwhj.cn

================================================================================
来源：http://bz.hahajie.cn

J. 日期与时间
来源：http://nl.huixinmuqiang.cn

================================================================================
来源：http://fb.wgjwhj.cn

[J01] 获取当前时间
来源：http://xd.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://od.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wt.szsharing.cn

JS:   new Date();  Date.now()
来源：http://je.asd995.cn

TS:   new Date();  Date.now()
来源：http://ze.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://np.bookmarksfly.cn

Go:   time.Now()
来源：http://wv.521024.cn

Ruby: Time.now
来源：http://mf.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ju.muxihuayi.cn

[J02] 格式化输出
来源：http://pk.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://af.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dq.shxzukj.cn

TS:   d.toISOString()
来源：http://js.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oq.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jy.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://de.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cx.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://ua.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://st.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nu.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://rv.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://vw.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ml.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mi.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://po.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ht.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://uq.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oo.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ri.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cm.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kb.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ze.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uq.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iv.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gn.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://ox.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://wm.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rf.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zv.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mx.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://ol.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nx.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ec.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jw.nicolike.cn

[J06] 计算两时间之差
来源：http://qv.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://gh.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ly.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xm.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ja.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bb.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://br.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://zr.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://vl.muxihuayi.cn

[J07] 比较两个日期
来源：http://hs.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://fc.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yg.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tn.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lf.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xt.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://df.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mp.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://hg.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ba.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bm.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://su.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qf.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tb.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oc.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nm.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ni.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.huixiangedu.cn

[J09] 时区处理
来源：http://vw.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cy.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kr.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rp.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zl.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rj.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://az.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uy.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ub.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cx.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qr.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://of.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ox.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pq.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cd.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zz.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qw.9csxet.cn

================================================================================
来源：http://fq.bookmarksfly.cn

K. JSON 与序列化
来源：http://tl.huixiangedu.cn

================================================================================
来源：http://os.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://op.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sq.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pt.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ya.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://pr.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ho.9csxet.cn

Go:   json.Marshal(obj)
来源：http://td.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uq.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rv.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://lz.jctech888.com.cn

Py:   json.loads(s)
来源：http://zr.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mx.gzmigu.cn

JS:   JSON.parse(s)
来源：http://zo.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://bd.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xz.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://yn.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ly.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vp.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://jh.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fe.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cg.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bj.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nt.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nf.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ri.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://at.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hm.nicolike.cn

[K04] 读取 JSON 文件
来源：http://hd.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vv.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vr.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nw.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hg.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ei.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ir.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zh.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ep.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://st.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://mv.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://kn.szsharing.cn

JS:   structuredClone(obj)
来源：http://qv.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://sl.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ts.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://th.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://if.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sb.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://lk.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ag.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://df.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yb.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dd.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sa.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sd.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kx.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jp.yuntaijiaju.cn

[K07] 进制转换
来源：http://pe.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gp.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rv.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rb.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ac.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qa.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pl.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nl.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vb.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://zu.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://bw.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://io.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://uo.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://up.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ug.szsharing.cn

Go:   encoding/gob
来源：http://bm.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://bk.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://az.hnjuh.cn

================================================================================
来源：http://kw.shxzukj.cn

L. 网络请求
来源：http://il.shxzskj.cn

================================================================================
来源：http://gg.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://rl.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wt.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ro.nszjky.cn

JS:   await fetch(url)
来源：http://eq.szxytkj.cn

TS:   await fetch(url)
来源：http://fu.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bj.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://kl.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oy.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lg.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://yc.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wl.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kv.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zy.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ni.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nl.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://za.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kf.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qe.colortex.cn

[L03] 设置自定义请求头
来源：http://gp.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rp.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tr.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pe.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cw.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://th.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yo.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kt.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://os.hahajie.cn

[L04] 设置超时
来源：http://wg.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://jo.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://me.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fe.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qc.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qh.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cj.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ma.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://xv.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hm.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sw.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xc.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gl.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mk.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rj.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qc.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xx.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://yk.gzmigu.cn

Py:   resp.json()
来源：http://cu.colortex.cn

PHP:  json_decode($body, true);
来源：http://aj.jianghongdianzi.cn

JS:   await resp.json()
来源：http://pj.gzmigu.cn

TS:   await resp.json()
来源：http://mo.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tb.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ye.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://gw.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://kz.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bs.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nu.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ts.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://yk.hnjuh.cn

Java: resp.statusCode()
来源：http://ju.wgjwhj.cn

Go:   resp.StatusCode
来源：http://hh.521024.cn

Ruby: resp.code.to_i
来源：http://rq.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://es.shxzukj.cn

[L08] 并发请求多个地址
来源：http://qb.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xp.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://fr.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fw.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ke.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://am.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://il.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fh.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nv.huixiangedu.cn

================================================================================
来源：http://rw.521024.cn

M. 命令行 / 进程 / 环境
来源：http://df.9csxet.cn

================================================================================
来源：http://po.yuexingan06.cn

[M01] 读取命令行参数
来源：http://zy.9csxet.cn

Py:   sys.argv[1:]
来源：http://lh.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://xl.521024.cn

JS:   process.argv.slice(2)
来源：http://pp.hahajie.cn

TS:   process.argv.slice(2)
来源：http://oz.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://ci.nszjky.cn

Go:   os.Args[1:]
来源：http://vg.hnjuh.cn

Ruby: ARGV
来源：http://ji.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://fj.muxihuayi.cn

[M02] 读取环境变量
来源：http://oc.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ww.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://to.szsharing.cn

JS:   process.env.HOME
来源：http://ek.521024.cn

TS:   process.env.HOME
来源：http://iv.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://xe.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ko.colortex.cn

Ruby: ENV["HOME"]
来源：http://ua.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cj.hnjuh.cn

[M03] 执行外部命令
来源：http://zo.yuntaijiaju.cn


<!-- 参考信息 -->