代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mo.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fl.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oz.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ld.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://le.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jm.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xf.gzmigu.cn

[I05] 按正则拆分
来源：http://xy.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oe.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wk.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://xo.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mn.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://sz.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uj.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ph.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eq.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yp.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jc.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wq.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zz.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wy.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gy.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://li.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ik.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://zf.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kt.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gz.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bn.jctech888.com.cn

TS:   /error/gim
来源：http://nx.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hm.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ol.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://pj.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zf.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://dv.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hr.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bb.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ad.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hs.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://an.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://me.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jl.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pr.muxihuayi.cn

================================================================================
来源：http://lo.bjjhwx.cn

J. 日期与时间
来源：http://ex.panjiajie.cn

================================================================================
来源：http://rw.gzmigu.cn

[J01] 获取当前时间
来源：http://kp.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ep.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tm.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://id.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://qc.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tq.hnjuh.cn

Go:   time.Now()
来源：http://kl.shxzskj.cn

Ruby: Time.now
来源：http://sf.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ph.newstarts.cn

[J02] 格式化输出
来源：http://on.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ik.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yv.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fn.521024.cn

TS:   d.toISOString()
来源：http://ab.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nl.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://do.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ee.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ye.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://cw.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bz.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zg.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://hx.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://bu.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fu.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yr.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://us.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kw.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ws.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ky.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cl.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ti.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tr.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://di.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kp.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nt.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ys.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://lm.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://wy.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sk.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://js.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pv.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://io.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ew.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://cg.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yz.jctech888.com.cn

[J06] 计算两时间之差
来源：http://dw.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://yf.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://hs.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ac.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qu.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ak.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://nm.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://km.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://me.colortex.cn

[J07] 比较两个日期
来源：http://ab.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://dg.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ia.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://og.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ff.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iu.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mm.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pr.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://so.shxzukj.cn

[J08] 提取年月日与星期
来源：http://hu.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ou.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kf.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vc.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eh.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ep.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tq.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vh.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://su.colortex.cn

[J09] 时区处理
来源：http://fj.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ab.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kc.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gu.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gi.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://at.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pk.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yt.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wx.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://jl.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pj.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cu.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kr.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tc.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://li.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qm.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lo.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gh.huanxung.cn

================================================================================
来源：http://dn.colortex.cn

K. JSON 与序列化
来源：http://mc.shxzukj.cn

================================================================================
来源：http://qe.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ej.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fr.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ug.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://vy.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://id.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://we.nicolike.cn

Go:   json.Marshal(obj)
来源：http://cb.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zn.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mq.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://nt.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ra.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xp.nszjky.cn

JS:   JSON.parse(s)
来源：http://ed.nicolike.cn

TS:   JSON.parse(s)
来源：http://md.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lh.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://fq.colortex.cn

Ruby: JSON.parse(s)
来源：http://lv.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fd.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://ti.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wf.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dh.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pv.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://to.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oh.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tt.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yr.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ls.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://py.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tv.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jf.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yi.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yf.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kl.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oe.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cu.szsharing.cn

[K05] 深拷贝对象
来源：http://bs.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://xg.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://vq.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://wb.panjiajie.cn

TS:   structuredClone(obj)
来源：http://rv.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hy.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kg.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ux.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pm.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://jr.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bj.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ly.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wb.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hy.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jo.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vd.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hy.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ep.huixiangedu.cn

[K07] 进制转换
来源：http://vx.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ml.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ti.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nt.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gj.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uv.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nf.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ec.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sx.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gg.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://jj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bh.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://lc.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://pb.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jv.colortex.cn

Go:   encoding/gob
来源：http://io.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ng.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vd.szsharing.cn

================================================================================
来源：http://vi.chemitech.net.cn

L. 网络请求
来源：http://da.szsharing.cn

================================================================================
来源：http://hi.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://tz.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nb.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bw.gzmigu.cn

JS:   await fetch(url)
来源：http://qj.szsharing.cn

TS:   await fetch(url)
来源：http://wq.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ek.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://qj.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sa.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://to.newstarts.cn

[L02] 发送 POST JSON
来源：http://kv.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qf.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hh.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gc.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ne.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pa.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dd.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fl.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mf.szxytkj.cn

[L03] 设置自定义请求头
来源：http://fy.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ta.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pi.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wt.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dk.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qk.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wo.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ud.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wf.gzmigu.cn

[L04] 设置超时
来源：http://bl.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://dp.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ef.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gm.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ha.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cr.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ia.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gj.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://ou.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oa.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mh.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ui.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kt.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fr.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nn.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rj.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xv.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://au.yuntaijiaju.cn

Py:   resp.json()
来源：http://ql.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://it.shxzskj.cn

JS:   await resp.json()
来源：http://ao.lnxyls.cn

TS:   await resp.json()
来源：http://la.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ez.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qt.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://zj.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dd.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://fg.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yc.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gv.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ic.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ts.huanxung.cn

Java: resp.statusCode()
来源：http://eo.shxzskj.cn

Go:   resp.StatusCode
来源：http://ao.panjiajie.cn

Ruby: resp.code.to_i
来源：http://wi.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://cp.szsharing.cn

[L08] 并发请求多个地址
来源：http://my.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mx.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://ku.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qi.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ef.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qu.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qk.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sm.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ah.wgjwhj.cn

================================================================================
来源：http://pj.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ak.gzmigu.cn

================================================================================
来源：http://sx.colortex.cn

[M01] 读取命令行参数
来源：http://hx.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ty.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://td.nszjky.cn

JS:   process.argv.slice(2)
来源：http://dd.huanxung.cn

TS:   process.argv.slice(2)
来源：http://cv.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ex.gzmigu.cn

Go:   os.Args[1:]
来源：http://ct.huixiangedu.cn

Ruby: ARGV
来源：http://nl.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://iz.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://au.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://mn.szxytkj.cn


<!-- 参考信息 -->