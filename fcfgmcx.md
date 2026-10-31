代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://wu.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zz.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zy.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zy.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ci.521024.cn

Go:   defer f.Close()
来源：http://ti.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jn.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yz.521024.cn

================================================================================
来源：http://qh.haigaiapp.cn

I. 正则表达式
来源：http://db.jianghongdianzi.cn

================================================================================
来源：http://yh.huanxung.cn

[I01] 判断是否匹配
来源：http://gb.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ie.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pv.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://qg.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://yh.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ji.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vh.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://rs.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ua.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://cr.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://kc.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tz.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wf.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://kq.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rn.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://td.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://kh.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nc.huixiangedu.cn

[I03] 提取捕获分组
来源：http://gs.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kv.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iu.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mt.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cl.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pw.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cc.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tg.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cn.bjjhwx.cn

[I04] 正则替换
来源：http://vf.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zk.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dk.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pd.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qv.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xg.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ew.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nj.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xx.panjiajie.cn

[I05] 按正则拆分
来源：http://ci.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gc.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jh.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tn.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://jt.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://hh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cz.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sf.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jq.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zj.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hb.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rd.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ju.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dh.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ok.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zv.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pt.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jy.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://bs.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ui.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zd.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qx.newstarts.cn

TS:   /error/gim
来源：http://nh.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vp.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ba.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://hm.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cq.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gd.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gz.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aj.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yc.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dn.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tv.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xk.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rm.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wb.haigaiapp.cn

================================================================================
来源：http://wb.521024.cn

J. 日期与时间
来源：http://cd.jianghongdianzi.cn

================================================================================
来源：http://xh.muxihuayi.cn

[J01] 获取当前时间
来源：http://ir.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kj.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mh.hahajie.cn

JS:   new Date();  Date.now()
来源：http://iv.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://ew.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cp.huanxung.cn

Go:   time.Now()
来源：http://bl.yuexingan06.cn

Ruby: Time.now
来源：http://cq.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tx.asd995.cn

[J02] 格式化输出
来源：http://kr.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uf.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://my.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tv.haigaiapp.cn

TS:   d.toISOString()
来源：http://pm.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://to.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qb.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pe.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jt.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://td.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tu.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lz.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://qp.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://yq.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ya.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yt.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://jy.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yv.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ez.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ft.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mm.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wb.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://es.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ra.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jm.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ld.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gk.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://zr.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://np.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kr.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zc.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://bf.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jt.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://iy.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ih.hnjuh.cn

[J06] 计算两时间之差
来源：http://pi.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://gn.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://wz.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xy.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oe.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jw.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://up.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://oi.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://ig.panjiajie.cn

[J07] 比较两个日期
来源：http://xk.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://gq.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sy.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hq.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ye.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tj.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://te.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gm.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ga.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ad.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dg.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xn.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://we.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nj.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wm.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lo.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ux.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rx.huanxung.cn

[J09] 时区处理
来源：http://us.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cm.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xe.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xm.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qx.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rz.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gw.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://we.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://cr.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ad.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ng.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qg.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mk.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rj.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ok.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ok.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gw.bjjhwx.cn

================================================================================
来源：http://ul.muxihuayi.cn

K. JSON 与序列化
来源：http://wx.521024.cn

================================================================================
来源：http://rc.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://xy.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qt.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oo.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://dr.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://vt.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tv.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://gp.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ft.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kw.nszjky.cn

[K02] JSON 字符串转对象
来源：http://zd.521024.cn

Py:   json.loads(s)
来源：http://jf.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ux.newstarts.cn

JS:   JSON.parse(s)
来源：http://dh.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://hy.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://td.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://fy.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://jy.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ae.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://ji.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yj.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rp.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yf.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zd.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xd.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yx.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cm.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zc.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://ph.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jc.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pj.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fv.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jh.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ca.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pv.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cv.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ao.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://tl.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://xf.panjiajie.cn

JS:   structuredClone(obj)
来源：http://id.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://vy.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wn.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tv.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eb.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fz.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://rw.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xd.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://py.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fn.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jo.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uh.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ga.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tb.shxzskj.cn

[K07] 进制转换
来源：http://bv.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mf.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sh.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pc.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sg.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hq.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oz.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uq.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ui.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://hh.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://wm.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jy.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://nk.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://qj.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ru.szsharing.cn

Go:   encoding/gob
来源：http://xd.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://kc.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ft.panjiajie.cn

================================================================================
来源：http://dm.yuntaijiaju.cn

L. 网络请求
来源：http://dh.bookmarksfly.cn

================================================================================
来源：http://ki.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://tc.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mt.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mq.szxytkj.cn

JS:   await fetch(url)
来源：http://kp.yuexingan06.cn

TS:   await fetch(url)
来源：http://sk.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ae.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://pz.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gq.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dp.panjiajie.cn

[L02] 发送 POST JSON
来源：http://so.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://il.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cr.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lg.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zr.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://op.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pw.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sn.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jf.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ia.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ig.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yc.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wa.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lu.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hw.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sd.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yl.jctech888.com.cn

[L04] 设置超时
来源：http://ad.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://nr.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://di.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jy.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cw.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://la.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wv.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mb.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wy.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://oa.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ua.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yn.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zi.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qz.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dh.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zo.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ot.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wp.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://en.shxzskj.cn


<!-- 参考信息 -->