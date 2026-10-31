代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://we.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mi.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gq.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wy.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://di.gzmigu.cn

Go:   defer f.Close()
来源：http://ql.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hb.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hn.asd995.cn

================================================================================
来源：http://uz.shxzukj.cn

I. 正则表达式
来源：http://hv.asd995.cn

================================================================================
来源：http://hb.newstarts.cn

[I01] 判断是否匹配
来源：http://vn.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pz.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xp.nszjky.cn

JS:   /\d+/.test(s)
来源：http://eg.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://wc.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bd.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://py.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://fn.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gl.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://wa.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://bx.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://as.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zg.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://pe.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fe.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gk.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://kq.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aw.szxytkj.cn

[I03] 提取捕获分组
来源：http://wo.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://si.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zb.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lu.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rj.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://as.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mp.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ys.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jt.9csxet.cn

[I04] 正则替换
来源：http://qg.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zh.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mc.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wk.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zv.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fs.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jx.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cd.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uk.jctech888.com.cn

[I05] 按正则拆分
来源：http://cl.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vw.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nl.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://lf.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://sy.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://vo.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ws.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bz.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ga.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lk.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dn.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hq.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fk.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kv.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ex.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tz.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lc.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rt.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://si.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vt.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ga.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://br.yuntaijiaju.cn

TS:   /error/gim
来源：http://yy.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wt.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cw.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://ge.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bf.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://hp.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jj.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hd.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ai.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xf.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jv.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mo.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cs.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vj.hahajie.cn

================================================================================
来源：http://kn.yuntaijiaju.cn

J. 日期与时间
来源：http://sb.9csxet.cn

================================================================================
来源：http://cv.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://tq.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kc.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fg.asd995.cn

JS:   new Date();  Date.now()
来源：http://ju.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://fn.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sz.9csxet.cn

Go:   time.Now()
来源：http://kx.szsharing.cn

Ruby: Time.now
来源：http://ty.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ld.muxihuayi.cn

[J02] 格式化输出
来源：http://uz.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://py.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tr.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hu.huanxung.cn

TS:   d.toISOString()
来源：http://se.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wt.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cz.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aw.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qw.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://pm.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://md.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dd.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://tx.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://qi.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wg.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ch.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://xz.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cr.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://je.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fu.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cw.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uy.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kf.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ec.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gg.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hk.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cy.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://rx.521024.cn

Py:   now + timedelta(days=7)
来源：http://yt.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bi.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bg.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zm.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://so.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xb.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://kq.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sc.lnxyls.cn

[J06] 计算两时间之差
来源：http://ps.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://fq.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://bh.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yh.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ht.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pn.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://xp.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://xp.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://cr.nszjky.cn

[J07] 比较两个日期
来源：http://sl.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://rx.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lj.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hb.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cg.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://la.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uv.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ao.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://by.521024.cn

[J08] 提取年月日与星期
来源：http://co.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ow.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xd.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jc.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cp.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uw.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ka.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gk.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mg.szsharing.cn

[J09] 时区处理
来源：http://lf.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kb.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aj.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hk.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xv.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bc.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://pd.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xb.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qo.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ji.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rb.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://px.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ni.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yf.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xr.jctech888.com.cn

================================================================================
来源：http://qu.huixinmuqiang.cn

K. JSON 与序列化
来源：http://pu.yuntaijiaju.cn

================================================================================
来源：http://nv.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://qp.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jt.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cv.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://xo.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://up.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rc.huanxung.cn

Go:   json.Marshal(obj)
来源：http://vt.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zg.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bm.nszjky.cn

[K02] JSON 字符串转对象
来源：http://nw.chemitech.net.cn

Py:   json.loads(s)
来源：http://ki.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mx.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://yu.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://iy.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://em.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ab.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ip.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ey.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://uw.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rf.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cm.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ye.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zr.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fv.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mc.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ke.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nh.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://lt.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zz.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pk.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vv.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xe.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gk.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nw.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hu.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qy.gzmigu.cn

[K05] 深拷贝对象
来源：http://ut.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://wt.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://nf.newstarts.cn

JS:   structuredClone(obj)
来源：http://wp.shxzskj.cn

TS:   structuredClone(obj)
来源：http://yt.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tu.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ne.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xp.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pf.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://hl.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://is.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ga.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://js.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cp.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bm.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xk.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xw.shtwfgs.cn

[K07] 进制转换
来源：http://bl.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://il.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ix.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rd.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://td.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jy.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xk.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qf.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nw.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://je.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ra.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bd.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://rf.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://rx.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vr.yuntaijiaju.cn

Go:   encoding/gob
来源：http://qr.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://yp.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mj.hahajie.cn

================================================================================
来源：http://al.muxihuayi.cn

L. 网络请求
来源：http://eh.wgjwhj.cn

================================================================================
来源：http://mt.colortex.cn

[L01] 发送 GET 请求
来源：http://cx.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fk.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dw.521024.cn

JS:   await fetch(url)
来源：http://op.bookmarksfly.cn

TS:   await fetch(url)
来源：http://cw.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zt.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://cf.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://av.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xz.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://vl.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bo.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://do.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vd.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xn.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rx.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ew.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xc.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://oa.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jk.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ip.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aa.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nh.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://st.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kc.jctech888.com.cn

[L04] 设置超时
来源：http://lu.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ke.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://by.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zb.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bu.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nv.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fv.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vd.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://sg.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hr.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://al.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ds.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pi.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pn.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cy.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xh.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ay.huixiangedu.cn


<!-- 参考信息 -->