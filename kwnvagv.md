代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://km.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bx.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://by.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zh.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hp.asd995.cn

Go:   defer f.Close()
来源：http://gm.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ns.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xc.bookmarksfly.cn

================================================================================
来源：http://jp.colortex.cn

I. 正则表达式
来源：http://wj.hnjuh.cn

================================================================================
来源：http://yl.gzmigu.cn

[I01] 判断是否匹配
来源：http://qa.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tv.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vz.huanxung.cn

JS:   /\d+/.test(s)
来源：http://lf.nszjky.cn

TS:   /\d+/.test(s)
来源：http://uk.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xf.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yt.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://ch.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ea.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ua.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://gm.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ry.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ap.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://dq.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://th.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nh.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://ze.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bc.panjiajie.cn

[I03] 提取捕获分组
来源：http://hu.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qi.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ac.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ee.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jl.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nh.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ib.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ku.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ek.szsharing.cn

[I04] 正则替换
来源：http://jl.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yu.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sp.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pd.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ql.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tb.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uu.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jx.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oc.9csxet.cn

[I05] 按正则拆分
来源：http://fk.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://in.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://px.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://cl.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://ys.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://qy.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://np.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fq.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cv.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zs.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tu.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qi.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rv.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://se.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://en.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ja.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ep.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://bt.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://np.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pw.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ks.jianghongdianzi.cn

TS:   /error/gim
来源：http://if.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dk.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qi.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://os.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://lu.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ak.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hy.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fc.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jx.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://km.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ek.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://on.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ct.nszjky.cn

================================================================================
来源：http://oy.haigaiapp.cn

J. 日期与时间
来源：http://ua.9csxet.cn

================================================================================
来源：http://if.colortex.cn

[J01] 获取当前时间
来源：http://dr.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://db.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dt.huanxung.cn

JS:   new Date();  Date.now()
来源：http://hn.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://oa.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lf.bjjhwx.cn

Go:   time.Now()
来源：http://yu.chemitech.net.cn

Ruby: Time.now
来源：http://qk.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lq.shtwfgs.cn

[J02] 格式化输出
来源：http://wg.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uh.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://as.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xk.bookmarksfly.cn

TS:   d.toISOString()
来源：http://rv.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iz.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://os.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://go.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ra.huanxung.cn

[J03] 字符串解析为日期
来源：http://kp.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uo.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jz.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://gm.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ua.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sq.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dv.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://yc.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xm.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://vy.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ia.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zd.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yv.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vg.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://za.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nc.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fg.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://in.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ie.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://js.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ge.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iz.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zz.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://km.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qy.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://oq.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dj.nszjky.cn

[J06] 计算两时间之差
来源：http://or.colortex.cn

Py:   (end - start).total_seconds()
来源：http://qf.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://pd.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qs.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jd.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tj.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://cj.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://ve.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://ef.gzmigu.cn

[J07] 比较两个日期
来源：http://ti.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://cd.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://za.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://np.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xa.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ns.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cp.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rm.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://cp.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://sb.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sr.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ye.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://at.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hs.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cv.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vc.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ov.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pq.huixinmuqiang.cn

[J09] 时区处理
来源：http://db.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dy.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tt.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://id.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pz.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bp.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cn.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ln.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ju.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://lz.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ch.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uq.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ym.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qw.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iv.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jp.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fg.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://on.shxzskj.cn

================================================================================
来源：http://js.asd995.cn

K. JSON 与序列化
来源：http://is.haigaiapp.cn

================================================================================
来源：http://bs.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://zd.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sv.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jj.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://yk.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://qf.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://td.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://bi.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sg.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ll.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://gy.muxihuayi.cn

Py:   json.loads(s)
来源：http://id.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fz.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://ed.gzmigu.cn

TS:   JSON.parse(s)
来源：http://xr.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ny.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ar.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://in.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wu.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://im.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vn.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sm.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iv.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kb.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ep.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dp.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vz.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://xb.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gw.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zd.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uv.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jg.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ol.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bi.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dp.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mx.shxzukj.cn

[K05] 深拷贝对象
来源：http://ie.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://yl.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://ho.szsharing.cn

JS:   structuredClone(obj)
来源：http://pj.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ft.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ip.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xu.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eq.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nk.huanxung.cn

[K06] 解析 URL 查询串
来源：http://yl.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ci.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gh.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eo.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gg.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ei.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kf.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lg.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tb.shtwfgs.cn

[K07] 进制转换
来源：http://lv.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vl.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://so.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yv.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nt.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xg.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jx.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://id.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lc.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://kh.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://um.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://at.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://qc.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://db.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gd.huixiangedu.cn

Go:   encoding/gob
来源：http://mi.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://xe.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aq.huixiangedu.cn

================================================================================
来源：http://bb.chemitech.net.cn

L. 网络请求
来源：http://oj.huixiangedu.cn

================================================================================
来源：http://fp.szxytkj.cn

[L01] 发送 GET 请求
来源：http://xv.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ob.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mn.bookmarksfly.cn

JS:   await fetch(url)
来源：http://mq.colortex.cn

TS:   await fetch(url)
来源：http://bx.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ob.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://em.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ss.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lo.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://tl.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oo.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vp.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tr.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dh.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://si.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wz.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hm.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://io.nicolike.cn

[L03] 设置自定义请求头
来源：http://hn.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rk.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eg.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uz.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ro.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rg.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bm.521024.cn

[L04] 设置超时
来源：http://qo.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://fm.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xr.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ty.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://em.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ye.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://it.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eh.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mc.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://yd.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ra.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://if.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pr.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ti.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jy.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dm.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dt.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ld.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://fc.lnxyls.cn


<!-- 参考信息 -->