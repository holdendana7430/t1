代发 wailian999

[I02] 提取所有匹配
来源：http://rz.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://me.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hv.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ym.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://eu.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mp.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fh.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://qv.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://de.jctech888.com.cn

[I03] 提取捕获分组
来源：http://bz.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rm.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ot.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pl.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yh.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gq.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pa.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://na.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qs.nicolike.cn

[I04] 正则替换
来源：http://ta.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hd.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wp.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gz.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ce.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xe.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mj.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nq.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sg.shtwfgs.cn

[I05] 按正则拆分
来源：http://cw.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ep.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bg.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://kp.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://vg.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://hy.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jv.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lm.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fg.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ds.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://po.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://of.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cm.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xe.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xw.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ds.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pp.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://af.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://hl.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eg.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sz.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nt.muxihuayi.cn

TS:   /error/gim
来源：http://rr.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ta.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ps.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://qt.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cr.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://sv.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jd.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xz.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://am.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hv.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cn.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://es.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mr.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fi.shxzukj.cn

================================================================================
来源：http://ek.shtwfgs.cn

J. 日期与时间
来源：http://mk.muxihuayi.cn

================================================================================
来源：http://ds.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ot.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xs.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gm.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://yx.hahajie.cn

TS:   new Date();  Date.now()
来源：http://xr.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nb.szsharing.cn

Go:   time.Now()
来源：http://wx.9csxet.cn

Ruby: Time.now
来源：http://gm.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oz.9csxet.cn

[J02] 格式化输出
来源：http://tr.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://df.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wb.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tx.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://uw.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hx.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nx.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://af.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gy.shxzukj.cn

[J03] 字符串解析为日期
来源：http://xb.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ey.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://in.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://km.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://cv.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nm.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://td.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://lw.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rj.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://oe.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ks.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yn.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xs.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kd.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wq.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vt.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bb.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cs.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://cl.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://jl.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ez.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sz.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bu.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://wc.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gh.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://la.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ss.szxytkj.cn

[J06] 计算两时间之差
来源：http://zi.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://jn.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://fy.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ue.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oa.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lq.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://mo.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://yp.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ea.jctech888.com.cn

[J07] 比较两个日期
来源：http://zn.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://ca.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yl.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sr.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gl.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nq.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tk.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vd.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ri.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://ws.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eh.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eg.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cb.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ev.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ef.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ue.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jq.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yb.shxzukj.cn

[J09] 时区处理
来源：http://so.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zy.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yh.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fi.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ko.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://au.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ux.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ak.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gf.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://nf.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://td.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cx.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ur.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://er.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xt.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kf.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://av.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sq.shtwfgs.cn

================================================================================
来源：http://wk.muxihuayi.cn

K. JSON 与序列化
来源：http://hw.szxytkj.cn

================================================================================
来源：http://pe.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://cz.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ta.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xz.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ts.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://wo.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nu.asd995.cn

Go:   json.Marshal(obj)
来源：http://hb.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uu.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://la.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://fr.gzmigu.cn

Py:   json.loads(s)
来源：http://ab.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pq.lnxyls.cn

JS:   JSON.parse(s)
来源：http://lb.shxzskj.cn

TS:   JSON.parse(s)
来源：http://qm.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ks.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://qq.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://bg.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cp.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://sn.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rg.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wb.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ef.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bp.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zb.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ew.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zd.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cs.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ae.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xs.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pa.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://at.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bn.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jv.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xk.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nw.haigaiapp.cn

[K05] 深拷贝对象
来源：http://pi.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://sg.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://vp.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://fm.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://vs.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yv.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aj.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ty.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hk.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://mb.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cp.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mj.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://la.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dt.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eg.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gp.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wc.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ec.huanxung.cn

[K07] 进制转换
来源：http://it.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jl.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ch.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tn.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jy.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://my.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qr.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://hn.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://pa.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sz.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://uy.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://bw.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ms.huixiangedu.cn

Go:   encoding/gob
来源：http://rv.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://et.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aq.hahajie.cn

================================================================================
来源：http://jo.chemitech.net.cn

L. 网络请求
来源：http://as.nszjky.cn

================================================================================
来源：http://ku.shxzukj.cn

[L01] 发送 GET 请求
来源：http://bq.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://if.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yc.colortex.cn

JS:   await fetch(url)
来源：http://xs.newstarts.cn

TS:   await fetch(url)
来源：http://ro.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pv.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://wb.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rg.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://me.szxytkj.cn

[L02] 发送 POST JSON
来源：http://tr.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sg.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://js.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ns.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ju.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hq.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ct.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://si.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ao.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://sh.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://th.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sj.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gs.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cj.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yu.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kp.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cj.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ee.521024.cn

[L04] 设置超时
来源：http://xw.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://ak.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zb.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mc.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://et.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vt.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wo.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qs.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qb.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://bk.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gq.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vg.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mx.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ou.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hr.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tw.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gw.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xd.nszjky.cn

[L06] 解析响应为 JSON
来源：http://zk.shxzskj.cn

Py:   resp.json()
来源：http://kk.colortex.cn

PHP:  json_decode($body, true);
来源：http://gm.bookmarksfly.cn

JS:   await resp.json()
来源：http://vj.gzmigu.cn

TS:   await resp.json()
来源：http://xt.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sp.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qb.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ta.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sa.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://io.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hw.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rz.asd995.cn

JS:   resp.ok;  resp.status
来源：http://wv.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ss.gzmigu.cn

Java: resp.statusCode()
来源：http://wl.huanxung.cn

Go:   resp.StatusCode
来源：http://lv.lnxyls.cn

Ruby: resp.code.to_i
来源：http://lc.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://kx.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ep.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nr.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://lk.muxihuayi.cn


<!-- 参考信息 -->