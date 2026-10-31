代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ru.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fd.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://po.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ul.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kw.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yr.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://da.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gk.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bs.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://so.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uj.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iv.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ge.muxihuayi.cn

TS:   /error/gim
来源：http://pf.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ym.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vw.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://vg.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mi.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://gs.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wv.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bt.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gi.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ua.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fz.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fz.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nx.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://op.newstarts.cn

================================================================================
来源：http://la.haigaiapp.cn

J. 日期与时间
来源：http://wn.nszjky.cn

================================================================================
来源：http://kb.lnxyls.cn

[J01] 获取当前时间
来源：http://zm.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pl.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cg.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://rq.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://bt.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xw.panjiajie.cn

Go:   time.Now()
来源：http://df.huixiangedu.cn

Ruby: Time.now
来源：http://uj.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ne.jctech888.com.cn

[J02] 格式化输出
来源：http://ts.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vr.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mb.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fv.bookmarksfly.cn

TS:   d.toISOString()
来源：http://no.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uz.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dd.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aj.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ln.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://cs.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://at.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kh.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://eo.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://ta.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qb.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gi.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ci.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qi.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://rt.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fs.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gw.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fn.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uh.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ia.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ho.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gk.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fc.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://vo.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://kn.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://en.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://al.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://sf.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ch.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ba.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://av.nicolike.cn

[J06] 计算两时间之差
来源：http://nm.asd995.cn

Py:   (end - start).total_seconds()
来源：http://xl.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://po.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bw.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ma.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ln.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://qq.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://zk.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ac.jctech888.com.cn

[J07] 比较两个日期
来源：http://ck.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://pi.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dc.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ly.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cq.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aq.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sb.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wt.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://xh.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://cn.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ly.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://md.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jm.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qk.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pd.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dl.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ug.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ii.nicolike.cn

[J09] 时区处理
来源：http://te.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ws.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oo.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://an.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cd.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jf.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://va.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nr.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://qf.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uk.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fh.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gl.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ij.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gm.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qf.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pz.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wl.nicolike.cn

================================================================================
来源：http://pd.huixinmuqiang.cn

K. JSON 与序列化
来源：http://qa.lnxyls.cn

================================================================================
来源：http://ew.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://hd.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cy.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ft.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://cg.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://fu.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rc.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://vf.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fm.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cj.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://np.yuexingan06.cn

Py:   json.loads(s)
来源：http://fo.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ps.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://dc.nszjky.cn

TS:   JSON.parse(s)
来源：http://rm.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ib.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://gr.521024.cn

Ruby: JSON.parse(s)
来源：http://tf.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uf.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://eg.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zt.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ne.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bn.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hs.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mh.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gq.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ok.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://it.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://kr.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pp.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zk.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gl.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://na.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ma.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wt.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tf.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gu.9csxet.cn

[K05] 深拷贝对象
来源：http://oj.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://qf.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://of.nicolike.cn

JS:   structuredClone(obj)
来源：http://se.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://wm.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ir.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oh.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uk.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ib.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://zl.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dt.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vs.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hj.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kb.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lh.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nb.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oz.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nb.asd995.cn

[K07] 进制转换
来源：http://qk.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nw.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pv.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lp.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ga.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rr.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mn.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qp.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ix.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://or.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://ut.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://li.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://nz.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://mp.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gf.chemitech.net.cn

Go:   encoding/gob
来源：http://pq.521024.cn

Ruby: Marshal.dump(obj)
来源：http://hb.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wx.gzmigu.cn

================================================================================
来源：http://za.nicolike.cn

L. 网络请求
来源：http://qp.bjjhwx.cn

================================================================================
来源：http://bi.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ob.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wa.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gu.newstarts.cn

JS:   await fetch(url)
来源：http://zm.huixiangedu.cn

TS:   await fetch(url)
来源：http://vu.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bh.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ww.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ke.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nx.9csxet.cn

[L02] 发送 POST JSON
来源：http://uw.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bl.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://up.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qv.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pj.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eh.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ds.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jm.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fk.colortex.cn

[L03] 设置自定义请求头
来源：http://us.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://al.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ny.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ha.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rf.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://be.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nn.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ot.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xt.yuexingan06.cn

[L04] 设置超时
来源：http://vj.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://zz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zf.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ug.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://px.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dg.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vb.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ve.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xi.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sm.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rf.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://on.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gz.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vw.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sa.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://xd.gzmigu.cn

Py:   resp.json()
来源：http://hj.9csxet.cn

PHP:  json_decode($body, true);
来源：http://gj.lnxyls.cn

JS:   await resp.json()
来源：http://nz.hnjuh.cn

TS:   await resp.json()
来源：http://qt.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mt.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ox.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://sk.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rn.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://us.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cs.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jh.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://jj.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://xq.hahajie.cn

Java: resp.statusCode()
来源：http://dd.jctech888.com.cn

Go:   resp.StatusCode
来源：http://ag.nszjky.cn

Ruby: resp.code.to_i
来源：http://sf.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://hq.szsharing.cn

[L08] 并发请求多个地址
来源：http://xr.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fk.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://pc.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ve.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://do.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ab.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wa.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gy.huanxung.cn

================================================================================
来源：http://ju.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://bd.chemitech.net.cn

================================================================================
来源：http://sr.panjiajie.cn

[M01] 读取命令行参数
来源：http://rt.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://cy.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://hz.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://mo.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://vr.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://uf.bjjhwx.cn

Go:   os.Args[1:]
来源：http://lo.panjiajie.cn

Ruby: ARGV
来源：http://ce.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://fm.nszjky.cn

[M02] 读取环境变量
来源：http://yg.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://kx.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bg.hnjuh.cn

JS:   process.env.HOME
来源：http://pl.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://qh.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://wk.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zt.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://lo.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mw.chemitech.net.cn

[M03] 执行外部命令
来源：http://ot.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bo.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hs.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cb.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://al.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://it.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://du.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pi.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://jy.bookmarksfly.cn


<!-- 参考信息 -->