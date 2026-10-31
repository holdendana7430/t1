代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://qh.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gw.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lm.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xv.wgjwhj.cn

Go:   defer f.Close()
来源：http://fs.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bl.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bt.hahajie.cn

================================================================================
来源：http://kj.shxzskj.cn

I. 正则表达式
来源：http://lb.colortex.cn

================================================================================
来源：http://uh.chemitech.net.cn

[I01] 判断是否匹配
来源：http://zf.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tm.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ft.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://jk.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://bd.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qr.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ti.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://zc.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uc.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://kf.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://ro.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ad.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hn.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://fw.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://az.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jx.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://zy.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qf.wgjwhj.cn

[I03] 提取捕获分组
来源：http://pe.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rt.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zc.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jc.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zy.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hd.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sx.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xj.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mz.szsharing.cn

[I04] 正则替换
来源：http://hu.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ol.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ie.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jk.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mp.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rh.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qh.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oc.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gc.shxzskj.cn

[I05] 按正则拆分
来源：http://iq.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hg.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dy.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://wk.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://bl.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://rt.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ta.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wt.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wp.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://of.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lu.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://up.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mk.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://og.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fs.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://br.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mc.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kd.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://lc.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gy.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://am.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ve.newstarts.cn

TS:   /error/gim
来源：http://le.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hj.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yb.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ni.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jk.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://yc.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://de.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mq.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pl.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cu.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ld.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uu.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jh.gzmigu.cn

================================================================================
来源：http://wt.yuexingan06.cn

J. 日期与时间
来源：http://vq.jianghongdianzi.cn

================================================================================
来源：http://ny.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://mv.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://md.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bz.newstarts.cn

JS:   new Date();  Date.now()
来源：http://hf.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://ue.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xk.newstarts.cn

Go:   time.Now()
来源：http://ti.nicolike.cn

Ruby: Time.now
来源：http://xn.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nh.9csxet.cn

[J02] 格式化输出
来源：http://az.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vx.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ce.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://um.521024.cn

TS:   d.toISOString()
来源：http://xp.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qd.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yk.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mx.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yb.gzmigu.cn

[J03] 字符串解析为日期
来源：http://js.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://es.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gw.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://kg.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://vv.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://td.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pi.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://wj.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sd.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ex.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ud.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hh.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gm.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ak.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sv.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sd.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wr.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nl.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ye.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://iv.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gu.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oi.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://un.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://vq.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hp.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ek.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hb.shxzukj.cn

[J06] 计算两时间之差
来源：http://ga.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://bw.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://wx.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zw.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ij.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qz.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ru.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://su.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://yh.huixiangedu.cn

[J07] 比较两个日期
来源：http://jn.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://oj.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ll.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oj.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jv.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vd.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oq.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sz.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://sl.lnxyls.cn

[J08] 提取年月日与星期
来源：http://uq.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hl.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aj.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://of.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://no.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://on.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jv.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fy.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vq.yuntaijiaju.cn

[J09] 时区处理
来源：http://kz.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jv.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mr.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sm.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vi.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xa.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xr.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yc.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fp.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://um.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jn.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sm.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cf.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rr.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mk.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zr.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hs.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xz.jianghongdianzi.cn

================================================================================
来源：http://ds.jctech888.com.cn

K. JSON 与序列化
来源：http://ek.haigaiapp.cn

================================================================================
来源：http://ko.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ej.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://of.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xe.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://zg.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://qp.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ry.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://zd.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kf.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kk.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ea.gzmigu.cn

Py:   json.loads(s)
来源：http://xc.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://of.colortex.cn

JS:   JSON.parse(s)
来源：http://to.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://wo.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sk.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://vh.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://xh.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bn.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ny.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ry.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aq.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://og.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sh.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zp.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xf.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://to.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ot.nszjky.cn

[K04] 读取 JSON 文件
来源：http://sn.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zl.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gl.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://au.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://di.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lk.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://at.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zy.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dz.haigaiapp.cn

[K05] 深拷贝对象
来源：http://tk.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://xw.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://cn.521024.cn

JS:   structuredClone(obj)
来源：http://dm.shxzukj.cn

TS:   structuredClone(obj)
来源：http://zk.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tv.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yt.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rq.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aw.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://dm.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://am.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ad.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ld.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qz.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mp.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fi.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fm.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fk.bjjhwx.cn

[K07] 进制转换
来源：http://go.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ds.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ow.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ck.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rc.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zk.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cg.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jw.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://wy.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ef.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bu.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://lc.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ru.chemitech.net.cn

Go:   encoding/gob
来源：http://at.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://cj.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vx.hnjuh.cn

================================================================================
来源：http://bv.haigaiapp.cn

L. 网络请求
来源：http://rd.hnjuh.cn

================================================================================
来源：http://op.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://cj.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://of.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nw.muxihuayi.cn

JS:   await fetch(url)
来源：http://ol.bjjhwx.cn

TS:   await fetch(url)
来源：http://fc.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vr.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://yo.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zn.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oj.lnxyls.cn

[L02] 发送 POST JSON
来源：http://dk.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nc.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vj.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eq.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gs.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ty.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ey.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dy.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qv.shxzukj.cn

[L03] 设置自定义请求头
来源：http://tp.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dg.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://te.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fc.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rk.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://un.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yj.panjiajie.cn

[L04] 设置超时
来源：http://ri.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://cj.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ae.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jh.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://by.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ao.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dn.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xl.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lo.newstarts.cn

[L05] 上传文件（multipart）
来源：http://at.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oc.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tw.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oe.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ld.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cq.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yc.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wt.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yt.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://oe.gzmigu.cn


<!-- 参考信息 -->