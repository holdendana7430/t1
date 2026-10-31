代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yj.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uc.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://ci.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://vh.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bs.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kh.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://hh.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jb.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://lb.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://cc.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://as.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bi.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://qi.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tu.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://de.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ry.szxytkj.cn

[I03] 提取捕获分组
来源：http://qg.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lv.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nw.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ea.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rp.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qq.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gi.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eq.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pr.asd995.cn

[I04] 正则替换
来源：http://sm.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cb.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nc.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ps.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sx.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bg.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mb.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mo.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pf.huixiangedu.cn

[I05] 按正则拆分
来源：http://ot.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://in.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ry.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://rt.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wn.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://ys.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wy.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xc.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eo.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://su.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://au.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xw.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ao.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jc.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ok.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jn.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hr.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qd.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://kw.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mc.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hw.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jr.shxzukj.cn

TS:   /error/gim
来源：http://om.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xe.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wy.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://zu.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://up.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://oj.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://da.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qg.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vy.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ph.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eo.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hl.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://it.haigaiapp.cn

================================================================================
来源：http://wb.jctech888.com.cn

J. 日期与时间
来源：http://dp.huixinmuqiang.cn

================================================================================
来源：http://tb.nicolike.cn

[J01] 获取当前时间
来源：http://id.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://da.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fy.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://wj.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://bl.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ks.gzmigu.cn

Go:   time.Now()
来源：http://it.hnjuh.cn

Ruby: Time.now
来源：http://eb.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gj.huanxung.cn

[J02] 格式化输出
来源：http://fb.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gz.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://td.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pr.hahajie.cn

TS:   d.toISOString()
来源：http://rf.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gd.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kw.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://im.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dk.9csxet.cn

[J03] 字符串解析为日期
来源：http://mi.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tt.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bc.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://hd.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://zx.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mm.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wa.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://qe.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hb.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://be.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nx.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qt.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ed.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ae.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fh.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pk.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://in.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sv.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://qt.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://hu.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ib.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nr.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mm.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://cu.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kz.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://rw.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bt.jctech888.com.cn

[J06] 计算两时间之差
来源：http://fm.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://lk.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://cv.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fe.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ql.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://az.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://ag.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://vu.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://dk.chemitech.net.cn

[J07] 比较两个日期
来源：http://qz.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ew.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wx.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dk.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nl.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cn.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uv.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zi.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://fz.shxzukj.cn

[J08] 提取年月日与星期
来源：http://sy.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ru.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lv.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sp.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ak.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aw.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pt.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://df.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cr.yuntaijiaju.cn

[J09] 时区处理
来源：http://yw.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ex.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ku.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hx.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://go.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jy.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uf.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oh.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ig.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fs.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dn.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fz.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mp.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uh.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nf.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ot.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yg.yuexingan06.cn

================================================================================
来源：http://yd.hnjuh.cn

K. JSON 与序列化
来源：http://wy.szxytkj.cn

================================================================================
来源：http://ns.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://zg.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fs.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ka.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://xt.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://jf.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ia.colortex.cn

Go:   json.Marshal(obj)
来源：http://uk.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://st.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://js.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://qn.colortex.cn

Py:   json.loads(s)
来源：http://on.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ba.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://dq.asd995.cn

TS:   JSON.parse(s)
来源：http://sl.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://he.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ks.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://pz.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jg.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://nn.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mv.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cc.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gv.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lu.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://be.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gm.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://es.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zk.newstarts.cn

[K04] 读取 JSON 文件
来源：http://eo.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tt.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ul.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://za.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yw.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cc.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://no.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://of.szsharing.cn

[K05] 深拷贝对象
来源：http://zr.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://gq.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://dm.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://ib.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://in.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bu.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ws.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mc.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iw.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://en.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rz.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ae.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ho.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ao.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zo.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vr.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://np.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gp.shxzukj.cn

[K07] 进制转换
来源：http://ds.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yd.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ra.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xx.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gg.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fx.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mz.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jo.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dt.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://yy.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://di.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bt.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://tz.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://go.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yc.shxzukj.cn

Go:   encoding/gob
来源：http://wj.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ox.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uk.hnjuh.cn

================================================================================
来源：http://pi.jianghongdianzi.cn

L. 网络请求
来源：http://uu.bookmarksfly.cn

================================================================================
来源：http://da.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://th.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gg.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uc.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://aj.szsharing.cn

TS:   await fetch(url)
来源：http://au.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uf.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://bc.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mv.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://im.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://ov.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fl.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nu.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zo.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yy.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qn.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rx.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lx.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jl.panjiajie.cn

[L03] 设置自定义请求头
来源：http://pd.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ij.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://af.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mi.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vq.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ve.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tu.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uy.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xc.huanxung.cn

[L04] 设置超时
来源：http://fx.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://rj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gq.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://im.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sf.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zh.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lh.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ol.nszjky.cn

[L05] 上传文件（multipart）
来源：http://pf.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ya.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dd.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vf.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mc.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tz.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zl.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ed.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rx.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://ww.nicolike.cn

Py:   resp.json()
来源：http://wb.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ui.521024.cn

JS:   await resp.json()
来源：http://pt.jctech888.com.cn

TS:   await resp.json()
来源：http://mm.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nd.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hr.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://mg.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://no.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://tg.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bs.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ub.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://fb.asd995.cn


<!-- 参考信息 -->