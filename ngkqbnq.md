代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yi.jctech888.com.cn

Go:   defer f.Close()
来源：http://li.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ps.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bn.bjjhwx.cn

================================================================================
来源：http://mx.haigaiapp.cn

I. 正则表达式
来源：http://tw.nicolike.cn

================================================================================
来源：http://kq.colortex.cn

[I01] 判断是否匹配
来源：http://yt.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dl.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yl.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://wo.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://ko.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ta.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ls.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://sk.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hd.chemitech.net.cn

[I02] 提取所有匹配
来源：http://do.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://pb.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xo.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tz.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://gk.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jh.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lb.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://pq.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ip.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://pf.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://df.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yx.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ap.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bv.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hl.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eo.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ad.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xr.jianghongdianzi.cn

[I04] 正则替换
来源：http://qc.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://li.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wo.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ix.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bf.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://az.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qx.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yt.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bo.szsharing.cn

[I05] 按正则拆分
来源：http://uy.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ob.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lc.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ol.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://rb.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://sj.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pl.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wm.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pb.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vb.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wl.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://io.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ve.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mj.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iz.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vm.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://js.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jk.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://zs.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yc.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ti.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cn.yuexingan06.cn

TS:   /error/gim
来源：http://jr.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jh.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fh.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://jf.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iz.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://lx.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mc.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://od.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wb.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dx.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uu.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qs.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xf.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jr.muxihuayi.cn

================================================================================
来源：http://zm.jctech888.com.cn

J. 日期与时间
来源：http://rv.huixiangedu.cn

================================================================================
来源：http://xj.shtwfgs.cn

[J01] 获取当前时间
来源：http://ly.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cd.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dq.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://kd.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://or.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ms.panjiajie.cn

Go:   time.Now()
来源：http://ps.bjjhwx.cn

Ruby: Time.now
来源：http://ep.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ju.bjjhwx.cn

[J02] 格式化输出
来源：http://ol.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dj.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ar.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rc.chemitech.net.cn

TS:   d.toISOString()
来源：http://rh.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wo.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oy.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dj.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://me.nicolike.cn

[J03] 字符串解析为日期
来源：http://vc.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xh.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sv.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://tz.colortex.cn

TS:   new Date("2024-01-02")
来源：http://sx.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hj.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nf.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://cy.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://if.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://kg.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ab.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iy.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oq.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hc.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dw.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vj.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zl.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cv.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://yp.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://qk.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://px.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ta.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://be.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://uh.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bu.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://cz.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mc.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://tz.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://wa.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://ek.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qy.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ne.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pn.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://bn.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://go.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://xr.hnjuh.cn

[J07] 比较两个日期
来源：http://pn.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://fh.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vc.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ok.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oy.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zj.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pg.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cl.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ev.gzmigu.cn

[J08] 提取年月日与星期
来源：http://rx.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jl.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sr.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gd.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tm.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xa.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jx.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bv.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wn.hahajie.cn

[J09] 时区处理
来源：http://yj.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ud.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://va.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pu.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xr.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zp.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wi.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uc.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xg.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://lx.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gj.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kq.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tv.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://em.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xd.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ym.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://la.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rk.newstarts.cn

================================================================================
来源：http://zv.huixiangedu.cn

K. JSON 与序列化
来源：http://ie.yuntaijiaju.cn

================================================================================
来源：http://hf.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://ei.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sp.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mv.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://hr.asd995.cn

TS:   JSON.stringify(obj)
来源：http://tu.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oi.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://rs.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wl.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ke.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://yw.huixiangedu.cn

Py:   json.loads(s)
来源：http://dm.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uu.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://ue.lnxyls.cn

TS:   JSON.parse(s)
来源：http://yx.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lj.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://pe.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://yy.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bi.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://po.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gg.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wn.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rz.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://po.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yn.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rv.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gm.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rw.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://sv.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gw.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bd.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tz.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rl.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ac.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cy.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ty.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ve.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://cv.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://wg.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://fa.newstarts.cn

TS:   structuredClone(obj)
来源：http://gw.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zn.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ph.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xr.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uw.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://sc.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qt.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ax.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yj.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ee.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tz.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jf.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vn.hahajie.cn

[K07] 进制转换
来源：http://aa.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kx.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kp.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gb.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zm.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ou.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dn.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lt.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nc.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qd.asd995.cn

Py:   pickle.dumps(obj)
来源：http://vj.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wm.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://zd.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://bs.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ys.huixinmuqiang.cn

Go:   encoding/gob
来源：http://nq.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://sg.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ij.chemitech.net.cn

================================================================================
来源：http://fo.asd995.cn

L. 网络请求
来源：http://zu.9csxet.cn

================================================================================
来源：http://ya.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://rr.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qz.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://di.bjjhwx.cn

JS:   await fetch(url)
来源：http://kq.jctech888.com.cn

TS:   await fetch(url)
来源：http://if.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nj.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://at.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wo.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ey.shxzukj.cn

[L02] 发送 POST JSON
来源：http://tm.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sm.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pv.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kf.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ei.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://no.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wg.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://np.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ud.gzmigu.cn

[L03] 设置自定义请求头
来源：http://or.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ep.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zw.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hj.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gl.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://it.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fy.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zf.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yk.jianghongdianzi.cn

[L04] 设置超时
来源：http://lk.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://iw.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wl.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vc.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xp.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cw.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zl.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tm.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sr.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://tc.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vg.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ot.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oj.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vo.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yv.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qa.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fn.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://my.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://ff.hahajie.cn

Py:   resp.json()
来源：http://mj.nicolike.cn

PHP:  json_decode($body, true);
来源：http://lr.szsharing.cn

JS:   await resp.json()
来源：http://kx.muxihuayi.cn

TS:   await resp.json()
来源：http://hr.jianghongdianzi.cn


<!-- 参考信息 -->