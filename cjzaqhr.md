代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://yb.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gr.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mw.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dy.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rz.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fv.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kh.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mk.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wk.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ue.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bo.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bn.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wc.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://nc.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ab.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ty.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hq.huanxung.cn

TS:   /error/gim
来源：http://ao.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hk.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bd.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://cz.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ag.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ng.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wf.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wk.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gc.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sl.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rx.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ed.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yw.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://me.asd995.cn

================================================================================
来源：http://xt.hnjuh.cn

J. 日期与时间
来源：http://nx.huixinmuqiang.cn

================================================================================
来源：http://rk.nicolike.cn

[J01] 获取当前时间
来源：http://oj.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cw.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qw.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://bu.nicolike.cn

TS:   new Date();  Date.now()
来源：http://ab.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xz.szsharing.cn

Go:   time.Now()
来源：http://kr.hahajie.cn

Ruby: Time.now
来源：http://ry.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mm.bjjhwx.cn

[J02] 格式化输出
来源：http://lc.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bm.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wr.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ef.521024.cn

TS:   d.toISOString()
来源：http://ic.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fu.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tg.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ia.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bb.shxzskj.cn

[J03] 字符串解析为日期
来源：http://fs.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mb.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fw.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://za.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://tm.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qa.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vc.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://cq.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jo.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://nl.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jb.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://np.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kp.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ud.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uo.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yc.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zo.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://st.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://rw.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ej.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xn.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oj.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ol.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ni.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://bq.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://js.szxytkj.cn

[J06] 计算两时间之差
来源：http://zq.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://yf.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://uv.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ac.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lu.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qz.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://fh.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://lm.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://rg.shxzukj.cn

[J07] 比较两个日期
来源：http://sq.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://jw.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bm.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qm.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pm.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uv.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cx.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ek.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://vo.nszjky.cn

[J08] 提取年月日与星期
来源：http://pq.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hk.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sh.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://te.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dn.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bd.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gj.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pc.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aq.gzmigu.cn

[J09] 时区处理
来源：http://pi.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uq.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://it.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fh.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wi.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lg.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vt.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qw.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yb.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://bl.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pr.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wu.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hc.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tr.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ac.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ag.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gt.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cq.shxzukj.cn

================================================================================
来源：http://bg.lnxyls.cn

K. JSON 与序列化
来源：http://fa.jctech888.com.cn

================================================================================
来源：http://sw.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://rp.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zs.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rb.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://nb.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://fe.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cs.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://vf.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://km.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pg.nszjky.cn

[K02] JSON 字符串转对象
来源：http://bb.colortex.cn

Py:   json.loads(s)
来源：http://qo.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zo.lnxyls.cn

JS:   JSON.parse(s)
来源：http://nq.nszjky.cn

TS:   JSON.parse(s)
来源：http://ji.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nb.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ch.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://rb.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ng.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://og.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cs.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://da.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wv.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lk.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ub.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wa.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ze.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fr.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://pm.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qr.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zr.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gc.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://al.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ua.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pu.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bw.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jf.huixiangedu.cn

[K05] 深拷贝对象
来源：http://fd.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://cn.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://cz.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://vx.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://hg.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ol.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hq.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fz.newstarts.cn

[K06] 解析 URL 查询串
来源：http://nm.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jc.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fs.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ir.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ru.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wt.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jk.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hf.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cw.nszjky.cn

[K07] 进制转换
来源：http://tg.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sm.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wf.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cz.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kw.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ed.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://py.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pq.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nn.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ks.colortex.cn

Py:   pickle.dumps(obj)
来源：http://bv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dh.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://ri.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://rs.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gp.9csxet.cn

Go:   encoding/gob
来源：http://kn.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://wh.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wm.nicolike.cn

================================================================================
来源：http://yz.521024.cn

L. 网络请求
来源：http://at.szsharing.cn

================================================================================
来源：http://cd.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ed.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ls.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ua.shxzukj.cn

JS:   await fetch(url)
来源：http://wk.chemitech.net.cn

TS:   await fetch(url)
来源：http://wp.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ug.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://zd.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ga.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hu.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ak.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cc.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bo.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wb.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://am.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zm.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qe.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fd.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xj.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://pu.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xe.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yy.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eh.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ux.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jm.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bl.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rm.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ge.szsharing.cn

[L04] 设置超时
来源：http://mb.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://bj.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fm.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ri.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ys.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zf.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uw.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ry.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rq.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ub.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wa.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hl.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nw.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bu.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jq.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vh.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aj.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://et.huixinmuqiang.cn

Py:   resp.json()
来源：http://sj.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ar.nicolike.cn

JS:   await resp.json()
来源：http://hw.hahajie.cn

TS:   await resp.json()
来源：http://zk.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bc.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kv.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://wn.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ed.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://mz.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://go.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gi.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://xn.521024.cn

TS:   resp.ok;  resp.status
来源：http://qa.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://nl.szsharing.cn

Go:   resp.StatusCode
来源：http://pb.521024.cn

Ruby: resp.code.to_i
来源：http://oc.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://zf.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://od.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://id.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://rg.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pk.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ui.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hs.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ut.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lg.szxytkj.cn

================================================================================
来源：http://am.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://rq.hnjuh.cn

================================================================================
来源：http://dn.lnxyls.cn

[M01] 读取命令行参数
来源：http://eg.asd995.cn

Py:   sys.argv[1:]
来源：http://jg.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://uv.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://xw.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ed.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://np.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://bk.yuexingan06.cn

Ruby: ARGV
来源：http://xh.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://si.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://wn.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://kd.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rb.jctech888.com.cn

JS:   process.env.HOME
来源：http://pa.bookmarksfly.cn

TS:   process.env.HOME
来源：http://jg.szxytkj.cn

Java: System.getenv("HOME")
来源：http://vr.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pt.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://cw.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wq.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://bp.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ue.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://io.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ve.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vm.hahajie.cn


<!-- 参考信息 -->