代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://px.hnjuh.cn

Go:   defer f.Close()
来源：http://ay.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ad.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rc.yuntaijiaju.cn

================================================================================
来源：http://zi.muxihuayi.cn

I. 正则表达式
来源：http://hd.hahajie.cn

================================================================================
来源：http://at.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://vt.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://la.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tr.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://xd.newstarts.cn

TS:   /\d+/.test(s)
来源：http://zt.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fi.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pc.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://no.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sp.shxzskj.cn

[I02] 提取所有匹配
来源：http://gb.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://xw.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qn.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vd.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://qn.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hs.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bg.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://bc.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ru.9csxet.cn

[I03] 提取捕获分组
来源：http://tf.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pw.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nx.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jp.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gb.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://se.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iw.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kx.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vv.huixiangedu.cn

[I04] 正则替换
来源：http://ox.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zv.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sc.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sm.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jj.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ts.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gw.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://az.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ew.chemitech.net.cn

[I05] 按正则拆分
来源：http://lg.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nv.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jr.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://fs.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mp.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://fx.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ja.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fh.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://go.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tq.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ew.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hb.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aa.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ie.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eo.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fi.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vy.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rw.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://hw.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kn.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ed.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gm.chemitech.net.cn

TS:   /error/gim
来源：http://la.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ka.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://so.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://yl.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ja.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://wr.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ii.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vo.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://el.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gn.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gb.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xn.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ck.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dl.huixiangedu.cn

================================================================================
来源：http://oc.hahajie.cn

J. 日期与时间
来源：http://cz.colortex.cn

================================================================================
来源：http://lm.bookmarksfly.cn

[J01] 获取当前时间
来源：http://yy.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cj.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mf.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://yf.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://hg.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ff.521024.cn

Go:   time.Now()
来源：http://mx.nszjky.cn

Ruby: Time.now
来源：http://we.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zm.lnxyls.cn

[J02] 格式化输出
来源：http://ky.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mf.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://te.chemitech.net.cn

TS:   d.toISOString()
来源：http://xe.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vo.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ur.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hy.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://mp.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mh.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sv.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://tp.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://hw.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ho.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pj.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://fi.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tt.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://wi.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://me.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pp.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ww.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ps.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dk.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://es.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tg.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://du.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://nj.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://sp.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sg.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gy.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wl.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://oy.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vh.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://kd.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vs.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://ht.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://np.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://da.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://so.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rc.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jo.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://if.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://rb.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://jy.chemitech.net.cn

[J07] 比较两个日期
来源：http://jq.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://tn.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://en.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mz.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://en.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mr.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xl.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xc.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://cl.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://qj.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jd.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fs.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://en.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ca.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iq.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xp.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bm.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://un.shtwfgs.cn

[J09] 时区处理
来源：http://qd.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fp.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cc.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yf.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eb.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wm.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tv.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oh.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://pw.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eu.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ah.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nv.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://of.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qx.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://da.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mf.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yt.haigaiapp.cn

================================================================================
来源：http://ys.shxzukj.cn

K. JSON 与序列化
来源：http://uf.nszjky.cn

================================================================================
来源：http://tg.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://yt.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://km.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kj.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://vv.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://bv.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ba.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://hb.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ls.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ah.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://eu.nszjky.cn

Py:   json.loads(s)
来源：http://ia.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ze.newstarts.cn

JS:   JSON.parse(s)
来源：http://pk.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://wj.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://we.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ry.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://lm.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bh.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vk.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ii.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vg.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tt.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pd.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dd.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ui.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gc.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://jx.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kv.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://om.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sz.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zl.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ov.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wr.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nz.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ua.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://my.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://rk.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://dg.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://de.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://bv.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ck.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xv.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oy.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bu.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://op.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ez.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fx.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xj.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ot.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uc.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jg.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nt.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fk.shxzukj.cn

[K07] 进制转换
来源：http://ss.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mu.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ni.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ji.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qp.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://da.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zm.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aw.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tv.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qg.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://rn.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://my.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ko.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://tt.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://of.colortex.cn

Go:   encoding/gob
来源：http://ww.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://mf.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hs.newstarts.cn

================================================================================
来源：http://et.gzmigu.cn

L. 网络请求
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://wo.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://mj.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vp.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zo.gzmigu.cn

JS:   await fetch(url)
来源：http://yq.9csxet.cn

TS:   await fetch(url)
来源：http://da.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qb.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://he.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://am.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://of.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://rh.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ak.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mh.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kp.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hx.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yr.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wm.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rc.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uw.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://ff.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mq.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cd.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mn.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nm.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kr.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qg.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ju.chemitech.net.cn

[L04] 设置超时
来源：http://hb.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://uu.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xm.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cy.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ww.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eq.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pe.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qr.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ab.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://rk.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://io.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://np.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dk.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wt.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hq.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bh.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rd.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qt.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://zo.jianghongdianzi.cn

Py:   resp.json()
来源：http://no.asd995.cn

PHP:  json_decode($body, true);
来源：http://cz.nicolike.cn

JS:   await resp.json()
来源：http://va.chemitech.net.cn

TS:   await resp.json()
来源：http://qr.9csxet.cn


<!-- 参考信息 -->