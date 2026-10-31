代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://ss.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://id.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cc.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cc.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tg.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vd.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lt.haigaiapp.cn

[H10] 资源自动释放
来源：http://dz.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ba.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wz.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ey.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dw.szxytkj.cn

Go:   defer f.Close()
来源：http://ur.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sg.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://di.hnjuh.cn

================================================================================
来源：http://ny.hahajie.cn

I. 正则表达式
来源：http://pm.huixiangedu.cn

================================================================================
来源：http://fr.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ae.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://en.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bz.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://in.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://hb.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qs.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gx.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://hr.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mu.bjjhwx.cn

[I02] 提取所有匹配
来源：http://op.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://me.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wp.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kl.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://dp.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kr.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gq.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://lv.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hp.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://tz.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cb.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://an.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tm.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gn.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://px.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ut.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tj.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bo.colortex.cn

[I04] 正则替换
来源：http://pl.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hg.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cr.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eb.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eu.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sg.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tf.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yl.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jp.huanxung.cn

[I05] 按正则拆分
来源：http://yy.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rf.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xr.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://xu.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://ty.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://jx.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cc.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qi.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wx.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lg.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jx.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qz.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uz.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pw.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pt.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bd.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gj.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://wc.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mm.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rd.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mh.yuntaijiaju.cn

TS:   /error/gim
来源：http://fg.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bi.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xk.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://pz.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yj.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://va.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yr.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pg.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fy.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fu.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zr.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://we.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ox.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mo.bjjhwx.cn

================================================================================
来源：http://jb.lnxyls.cn

J. 日期与时间
来源：http://on.huixiangedu.cn

================================================================================
来源：http://bc.hahajie.cn

[J01] 获取当前时间
来源：http://od.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ep.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nu.newstarts.cn

JS:   new Date();  Date.now()
来源：http://hb.521024.cn

TS:   new Date();  Date.now()
来源：http://ap.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rm.colortex.cn

Go:   time.Now()
来源：http://es.wgjwhj.cn

Ruby: Time.now
来源：http://jx.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rb.szxytkj.cn

[J02] 格式化输出
来源：http://lc.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gq.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hx.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fx.shxzukj.cn

TS:   d.toISOString()
来源：http://de.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pa.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://go.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nx.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ca.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://jq.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jk.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://us.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://jl.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://hu.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tm.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wl.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://vy.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bx.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://lc.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hl.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rt.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xy.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qg.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hg.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rk.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bf.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cg.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://us.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://ih.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ob.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tc.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dy.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://wi.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xt.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ld.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ka.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ye.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://oy.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://fr.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aa.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kh.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zf.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://aw.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://sn.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://zn.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://wg.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ur.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://li.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fq.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xt.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pq.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ng.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rq.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.nszjky.cn

[J08] 提取年月日与星期
来源：http://ru.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://he.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yr.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kx.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xg.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ym.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zg.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wc.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://se.jctech888.com.cn

[J09] 时区处理
来源：http://mt.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ep.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ht.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zo.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gt.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yk.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sq.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dk.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tv.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://yb.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sm.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ek.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bt.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nl.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gb.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://za.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://py.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ij.muxihuayi.cn

================================================================================
来源：http://cn.nicolike.cn

K. JSON 与序列化
来源：http://fi.wgjwhj.cn

================================================================================
来源：http://wx.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://fk.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dp.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dn.colortex.cn

JS:   JSON.stringify(obj)
来源：http://kq.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://op.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xk.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://tz.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ny.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ft.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ul.nszjky.cn

Py:   json.loads(s)
来源：http://dn.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jr.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://di.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://hs.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qc.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://hy.newstarts.cn

Ruby: JSON.parse(s)
来源：http://gr.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iu.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zm.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bv.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mo.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gm.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hg.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ai.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gs.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qa.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hl.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://aj.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mc.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pa.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qb.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yu.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kd.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xd.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fe.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://zv.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://zy.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://gq.colortex.cn

JS:   structuredClone(obj)
来源：http://fl.gzmigu.cn

TS:   structuredClone(obj)
来源：http://nj.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pd.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vl.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ka.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rl.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ka.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wa.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vt.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mv.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ug.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fl.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pz.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ur.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cm.gzmigu.cn

[K07] 进制转换
来源：http://pa.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tp.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pt.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://to.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rn.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ov.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ux.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qd.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bg.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://sw.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://lg.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://le.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://qg.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ft.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://or.gzmigu.cn

Go:   encoding/gob
来源：http://pw.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://df.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yp.hnjuh.cn

================================================================================
来源：http://up.shxzukj.cn

L. 网络请求
来源：http://vn.hahajie.cn

================================================================================
来源：http://nq.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://cs.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yp.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tv.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://lz.muxihuayi.cn

TS:   await fetch(url)
来源：http://pp.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vn.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://qh.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ku.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mh.nszjky.cn

[L02] 发送 POST JSON
来源：http://zr.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://en.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pm.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zk.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yg.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hn.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://el.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nk.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wt.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://cl.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oo.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ib.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cu.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iz.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ij.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mg.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://et.hnjuh.cn

[L04] 设置超时
来源：http://mu.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ud.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fc.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cn.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kv.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tx.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yh.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fr.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tj.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://yj.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wb.yuntaijiaju.cn


<!-- 参考信息 -->