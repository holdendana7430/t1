代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eu.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zl.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rz.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qq.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jo.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nm.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cb.hahajie.cn

[I05] 按正则拆分
来源：http://bn.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sq.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yy.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://lf.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://pc.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://mg.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ru.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bp.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://co.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zq.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cl.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cg.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hx.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ci.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jr.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lv.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ar.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sn.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://so.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gu.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ge.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zb.muxihuayi.cn

TS:   /error/gim
来源：http://dk.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://si.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ha.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://ek.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cs.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ai.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ym.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mq.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ia.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://im.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yq.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dm.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cx.szxytkj.cn

================================================================================
来源：http://xp.colortex.cn

J. 日期与时间
来源：http://or.nszjky.cn

================================================================================
来源：http://lh.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://my.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vc.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tx.newstarts.cn

JS:   new Date();  Date.now()
来源：http://ls.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://ix.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dh.nicolike.cn

Go:   time.Now()
来源：http://ck.newstarts.cn

Ruby: Time.now
来源：http://en.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vr.szsharing.cn

[J02] 格式化输出
来源：http://tc.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mx.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xg.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ob.panjiajie.cn

TS:   d.toISOString()
来源：http://iv.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://br.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ce.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zc.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qr.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://fu.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://br.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wc.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://pk.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://sq.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pf.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cc.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://qg.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ub.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://ib.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nx.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dc.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iw.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ek.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ae.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gh.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ew.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lf.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://md.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://wj.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lv.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lg.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ee.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://qh.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hv.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://ae.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://np.newstarts.cn

[J06] 计算两时间之差
来源：http://yr.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://lq.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://et.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lj.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tx.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vb.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://qd.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://gy.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://fg.shxzukj.cn

[J07] 比较两个日期
来源：http://vq.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zi.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://in.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mr.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kg.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ft.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fb.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xd.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ew.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://do.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vz.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://im.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ar.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wc.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ki.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ju.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zz.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ep.chemitech.net.cn

[J09] 时区处理
来源：http://zz.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bs.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://op.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pn.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zf.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bm.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ba.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oh.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zq.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://rw.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wg.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xk.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wh.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qz.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hd.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yn.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qk.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uu.huanxung.cn

================================================================================
来源：http://iu.szxytkj.cn

K. JSON 与序列化
来源：http://mf.jianghongdianzi.cn

================================================================================
来源：http://re.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://vx.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ff.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rv.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://ao.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://se.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pu.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://un.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://se.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pe.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://bj.bjjhwx.cn

Py:   json.loads(s)
来源：http://yv.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://il.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://qs.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ud.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fh.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://sr.huanxung.cn

Ruby: JSON.parse(s)
来源：http://dp.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fm.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://mq.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xc.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uv.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jj.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://km.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vz.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jt.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mx.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lx.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://xb.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gp.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kn.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hb.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jf.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://of.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pl.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ul.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nf.shtwfgs.cn

[K05] 深拷贝对象
来源：http://aw.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://go.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://yp.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://ka.colortex.cn

TS:   structuredClone(obj)
来源：http://zf.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://td.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ot.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vp.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tg.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://xm.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fv.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mf.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rb.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zp.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ho.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nc.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://od.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://br.panjiajie.cn

[K07] 进制转换
来源：http://dr.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lc.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xb.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jx.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://un.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mi.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://np.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yb.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mr.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://vs.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://sd.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gg.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ko.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://gu.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ya.colortex.cn

Go:   encoding/gob
来源：http://uc.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://qd.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bi.huanxung.cn

================================================================================
来源：http://jn.jctech888.com.cn

L. 网络请求
来源：http://oi.bjjhwx.cn

================================================================================
来源：http://qc.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://kx.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://is.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hg.szxytkj.cn

JS:   await fetch(url)
来源：http://bq.haigaiapp.cn

TS:   await fetch(url)
来源：http://fl.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kn.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ee.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iz.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://st.hnjuh.cn

[L02] 发送 POST JSON
来源：http://lv.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ke.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hk.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mc.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://po.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gb.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xu.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iw.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wf.hahajie.cn

[L03] 设置自定义请求头
来源：http://pl.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ur.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yk.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ed.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fk.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jy.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://se.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fv.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ld.haigaiapp.cn

[L04] 设置超时
来源：http://vs.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://di.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ne.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vs.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uy.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ds.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cv.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qd.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uv.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ih.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jy.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hu.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ou.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xh.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lp.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://px.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bv.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://by.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://re.jianghongdianzi.cn

Py:   resp.json()
来源：http://gn.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://qn.jianghongdianzi.cn

JS:   await resp.json()
来源：http://ph.wgjwhj.cn

TS:   await resp.json()
来源：http://wo.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lb.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qq.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://dw.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dl.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://vm.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://my.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cw.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://bc.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://kx.panjiajie.cn

Java: resp.statusCode()
来源：http://oz.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ji.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://ol.521024.cn

C#:   (int)resp.StatusCode
来源：http://vv.9csxet.cn

[L08] 并发请求多个地址
来源：http://dk.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aw.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://il.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bo.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ew.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ws.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pf.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://lf.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://tq.gzmigu.cn

================================================================================
来源：http://zr.colortex.cn

[M01] 读取命令行参数
来源：http://hu.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ad.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://dm.newstarts.cn

JS:   process.argv.slice(2)
来源：http://kr.hahajie.cn

TS:   process.argv.slice(2)
来源：http://nz.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://mw.9csxet.cn

Go:   os.Args[1:]
来源：http://qi.shxzskj.cn

Ruby: ARGV
来源：http://qj.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://gb.hnjuh.cn

[M02] 读取环境变量
来源：http://ec.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://rh.muxihuayi.cn


<!-- 参考信息 -->