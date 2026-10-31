代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iv.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://el.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tb.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vt.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eh.newstarts.cn

[I04] 正则替换
来源：http://rw.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mi.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sj.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zt.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cb.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zq.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hw.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://me.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kf.colortex.cn

[I05] 按正则拆分
来源：http://mb.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mb.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bw.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ah.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://ni.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://ro.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://im.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ou.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ax.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zu.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xk.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://na.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yy.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rp.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fo.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mz.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://md.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://th.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://sv.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nt.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vq.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://go.wgjwhj.cn

TS:   /error/gim
来源：http://nu.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vi.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eb.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://jl.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wu.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://ib.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bv.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eo.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cg.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ff.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gm.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://an.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ap.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vw.huixiangedu.cn

================================================================================
来源：http://ff.jctech888.com.cn

J. 日期与时间
来源：http://mx.hahajie.cn

================================================================================
来源：http://ur.szsharing.cn

[J01] 获取当前时间
来源：http://db.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://za.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lg.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://ym.hahajie.cn

TS:   new Date();  Date.now()
来源：http://rk.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cj.yuexingan06.cn

Go:   time.Now()
来源：http://el.nicolike.cn

Ruby: Time.now
来源：http://bp.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://va.shxzukj.cn

[J02] 格式化输出
来源：http://lf.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lm.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zk.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fj.newstarts.cn

TS:   d.toISOString()
来源：http://rx.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yt.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cx.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jj.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tv.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ap.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xh.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://st.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://ny.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://tv.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vl.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dm.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://th.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ut.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://ph.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jo.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pf.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wx.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ap.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xu.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ax.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://km.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ou.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://gc.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kk.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://st.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sc.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://fl.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xk.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://qq.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fr.huixiangedu.cn

[J06] 计算两时间之差
来源：http://vf.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://yx.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://me.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://di.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ex.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xu.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://ar.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ww.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://pu.nszjky.cn

[J07] 比较两个日期
来源：http://yx.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://lf.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sx.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zg.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ln.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xw.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ka.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cy.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://vd.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://kw.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://om.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oz.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ce.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://is.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rt.hnjuh.cn

[J09] 时区处理
来源：http://co.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kb.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fk.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mi.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oc.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tv.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ej.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ya.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://if.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://iw.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iv.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ts.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oo.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://te.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hv.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wv.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wn.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wc.shtwfgs.cn

================================================================================
来源：http://dc.lnxyls.cn

K. JSON 与序列化
来源：http://bb.huixinmuqiang.cn

================================================================================
来源：http://fr.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://tr.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bv.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jt.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://fe.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://jq.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ou.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://tm.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sa.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vb.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ij.haigaiapp.cn

Py:   json.loads(s)
来源：http://do.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yf.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://be.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://sp.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mk.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://gl.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://bs.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bn.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ag.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cd.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://op.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ya.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ak.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zd.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bc.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bv.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ob.szsharing.cn

[K04] 读取 JSON 文件
来源：http://ki.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://go.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fo.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ml.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://db.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ge.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pt.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vl.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ly.chemitech.net.cn

[K05] 深拷贝对象
来源：http://xn.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ym.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://wm.hahajie.cn

JS:   structuredClone(obj)
来源：http://fa.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://rj.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://co.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jl.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eg.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ph.szsharing.cn

[K06] 解析 URL 查询串
来源：http://gv.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jx.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wk.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sl.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gh.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://it.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ko.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rj.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tk.wgjwhj.cn

[K07] 进制转换
来源：http://wf.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rf.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://so.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zt.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mw.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eg.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://su.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xt.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ls.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://yp.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://rn.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://so.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bx.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://zb.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xd.yuntaijiaju.cn

Go:   encoding/gob
来源：http://sn.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://kt.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ae.szsharing.cn

================================================================================
来源：http://be.lnxyls.cn

L. 网络请求
来源：http://kb.shtwfgs.cn

================================================================================
来源：http://ql.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://lc.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xj.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pw.muxihuayi.cn

JS:   await fetch(url)
来源：http://js.haigaiapp.cn

TS:   await fetch(url)
来源：http://zw.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pn.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ml.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dh.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ir.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://hr.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://so.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qk.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ox.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vi.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bq.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pk.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fd.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tx.shxzukj.cn

[L03] 设置自定义请求头
来源：http://al.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gr.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fr.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uv.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zf.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kg.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oq.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vg.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fd.yuntaijiaju.cn

[L04] 设置超时
来源：http://dt.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://im.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iy.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zw.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oz.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lr.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dv.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vn.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dq.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://od.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pf.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eu.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ym.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ry.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cs.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gi.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hd.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ic.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://uf.huixinmuqiang.cn

Py:   resp.json()
来源：http://ya.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://bv.nicolike.cn

JS:   await resp.json()
来源：http://gw.newstarts.cn

TS:   await resp.json()
来源：http://gq.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fi.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ha.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://vf.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ww.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://fn.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ah.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cb.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ee.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://ix.huanxung.cn

Java: resp.statusCode()
来源：http://kw.haigaiapp.cn

Go:   resp.StatusCode
来源：http://pn.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://yw.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://dn.newstarts.cn

[L08] 并发请求多个地址
来源：http://bv.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ht.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://rx.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://py.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fl.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jy.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://do.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oc.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uk.huixinmuqiang.cn

================================================================================
来源：http://xb.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://mf.szsharing.cn

================================================================================
来源：http://dg.muxihuayi.cn

[M01] 读取命令行参数
来源：http://wn.szsharing.cn

Py:   sys.argv[1:]
来源：http://yf.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://pu.jctech888.com.cn


<!-- 参考信息 -->