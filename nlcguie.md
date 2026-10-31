代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cs.jctech888.com.cn

[I03] 提取捕获分组
来源：http://hm.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aq.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kx.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ea.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eg.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vt.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kb.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dl.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ot.asd995.cn

[I04] 正则替换
来源：http://gs.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qb.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ni.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ap.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hv.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vv.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dy.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wr.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://af.gzmigu.cn

[I05] 按正则拆分
来源：http://ry.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aw.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zn.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://gh.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://fk.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://yt.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ns.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pz.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yp.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tu.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yn.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gy.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://je.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vd.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aq.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dl.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://av.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ql.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://zo.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wj.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gc.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cb.bjjhwx.cn

TS:   /error/gim
来源：http://od.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pp.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uq.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://fx.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vs.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://jp.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mm.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ih.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mu.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zj.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nl.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ux.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xk.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zs.9csxet.cn

================================================================================
来源：http://pz.9csxet.cn

J. 日期与时间
来源：http://yx.521024.cn

================================================================================
来源：http://dd.9csxet.cn

[J01] 获取当前时间
来源：http://fd.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tb.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wb.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://sr.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ak.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jd.9csxet.cn

Go:   time.Now()
来源：http://kg.shxzskj.cn

Ruby: Time.now
来源：http://cr.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xx.huanxung.cn

[J02] 格式化输出
来源：http://xr.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aa.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wa.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wd.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://ix.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eh.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://au.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nw.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jv.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ag.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dv.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bp.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://vm.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://gg.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qj.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lw.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://zj.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kb.huanxung.cn

[J04] 时间戳与日期互转
来源：http://gh.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yt.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fh.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://up.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xh.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vz.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hm.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kr.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xa.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://kj.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ua.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lv.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ch.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vm.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fb.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://cx.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tx.asd995.cn

[J06] 计算两时间之差
来源：http://yu.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://lv.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://go.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bq.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zj.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wj.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://il.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://vf.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://vo.gzmigu.cn

[J07] 比较两个日期
来源：http://hh.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://sb.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oz.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://an.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ot.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dw.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fk.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jy.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://ka.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ax.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mk.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xv.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qc.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aq.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yb.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ct.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kb.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bc.hnjuh.cn

[J09] 时区处理
来源：http://aj.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ts.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vr.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ao.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nx.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zo.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pd.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://wl.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rs.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zy.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dg.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ze.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vb.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yl.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sx.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jr.gzmigu.cn

================================================================================
来源：http://tl.hahajie.cn

K. JSON 与序列化
来源：http://ol.bookmarksfly.cn

================================================================================
来源：http://ro.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://rk.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ng.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cf.colortex.cn

JS:   JSON.stringify(obj)
来源：http://co.asd995.cn

TS:   JSON.stringify(obj)
来源：http://db.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sk.nicolike.cn

Go:   json.Marshal(obj)
来源：http://tu.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ak.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hk.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://hz.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://zn.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ku.shxzskj.cn

JS:   JSON.parse(s)
来源：http://jc.nszjky.cn

TS:   JSON.parse(s)
来源：http://cc.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tf.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ux.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://fg.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ib.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://pv.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nk.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uh.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://st.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mv.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dw.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pk.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dc.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://us.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://cz.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jd.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zx.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ms.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://et.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mr.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ig.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hm.lnxyls.cn

[K05] 深拷贝对象
来源：http://lh.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://vb.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.panjiajie.cn

JS:   structuredClone(obj)
来源：http://kq.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://zy.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vq.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ha.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ty.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hr.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://fp.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hk.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nq.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://on.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pn.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cb.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ro.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bl.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lf.lnxyls.cn

[K07] 进制转换
来源：http://tt.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://co.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eo.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xb.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://da.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bq.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mg.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hx.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ee.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://fw.521024.cn

Py:   pickle.dumps(obj)
来源：http://pg.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bp.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://yh.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://ou.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bd.newstarts.cn

Go:   encoding/gob
来源：http://hl.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://ae.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fw.muxihuayi.cn

================================================================================
来源：http://po.yuntaijiaju.cn

L. 网络请求
来源：http://ak.huixinmuqiang.cn

================================================================================
来源：http://bx.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://nx.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://te.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jt.521024.cn

JS:   await fetch(url)
来源：http://se.shxzskj.cn

TS:   await fetch(url)
来源：http://bn.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jw.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://wm.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wv.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cj.521024.cn

[L02] 发送 POST JSON
来源：http://iy.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kd.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qr.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qj.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cv.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tc.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ua.shxzskj.cn

[L03] 设置自定义请求头
来源：http://sx.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ti.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ju.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tj.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pa.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lh.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yg.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://py.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wj.lnxyls.cn

[L04] 设置超时
来源：http://rn.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://ua.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wp.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kb.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hv.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iw.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zy.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sp.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://lp.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hm.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://az.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://it.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hu.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://az.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ow.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cc.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vg.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://fm.shxzukj.cn

Py:   resp.json()
来源：http://wx.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://ut.521024.cn

JS:   await resp.json()
来源：http://ex.hahajie.cn

TS:   await resp.json()
来源：http://gp.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mv.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pt.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://qs.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://an.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://xg.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ek.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tn.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://rf.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://xr.hahajie.cn

Java: resp.statusCode()
来源：http://ns.newstarts.cn

Go:   resp.StatusCode
来源：http://cr.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://qh.521024.cn

C#:   (int)resp.StatusCode
来源：http://th.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ce.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ct.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://ip.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ay.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rl.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rf.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cf.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pq.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ht.huixinmuqiang.cn

================================================================================
来源：http://xe.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://pk.lnxyls.cn


<!-- 参考信息 -->