代发 wailian999

[H07] 断言
来源：http://tl.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://wk.huanxung.cn

PHP:  assert($x > 0);
来源：http://rn.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://oh.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://uu.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://fa.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://np.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wo.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://hc.521024.cn

[H08] 获取错误信息与堆栈
来源：http://xd.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ea.nszjky.cn

JS:   e.message;  e.stack
来源：http://rs.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rz.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ie.jianghongdianzi.cn

Go:   err.Error()
来源：http://sy.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://qm.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ff.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://yg.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jb.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fq.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gs.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://il.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jv.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qa.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ow.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hp.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://jj.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kv.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xh.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dc.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tz.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://si.nszjky.cn

Go:   defer f.Close()
来源：http://ge.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sq.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mx.muxihuayi.cn

================================================================================
来源：http://yx.521024.cn

I. 正则表达式
来源：http://pg.newstarts.cn

================================================================================
来源：http://yu.muxihuayi.cn

[I01] 判断是否匹配
来源：http://bn.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jo.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xq.huanxung.cn

JS:   /\d+/.test(s)
来源：http://xq.521024.cn

TS:   /\d+/.test(s)
来源：http://gb.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://co.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zn.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://rl.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qt.huanxung.cn

[I02] 提取所有匹配
来源：http://rd.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://ev.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mj.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://td.521024.cn

TS:   s.match(/\d+/g)
来源：http://jy.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jd.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ym.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://iw.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ct.hahajie.cn

[I03] 提取捕获分组
来源：http://oi.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wx.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vi.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qi.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://np.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aw.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ro.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fm.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yy.yuntaijiaju.cn

[I04] 正则替换
来源：http://rx.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mp.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wp.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hq.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nl.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mh.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hv.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kw.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qc.colortex.cn

[I05] 按正则拆分
来源：http://ru.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tn.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lz.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://oj.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://hf.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://zn.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mo.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cp.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nk.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mk.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xw.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yg.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hd.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xd.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qb.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ds.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fd.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://vp.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ti.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jh.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pm.szxytkj.cn

TS:   /error/gim
来源：http://hn.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://by.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wb.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://em.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sn.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://gl.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://go.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://re.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lm.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eh.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nz.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fj.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://li.yuntaijiaju.cn

================================================================================
来源：http://yt.jianghongdianzi.cn

J. 日期与时间
来源：http://um.yuexingan06.cn

================================================================================
来源：http://jc.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://oy.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ii.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rc.colortex.cn

JS:   new Date();  Date.now()
来源：http://qc.colortex.cn

TS:   new Date();  Date.now()
来源：http://ht.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mm.wgjwhj.cn

Go:   time.Now()
来源：http://fe.shtwfgs.cn

Ruby: Time.now
来源：http://vu.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ue.yuntaijiaju.cn

[J02] 格式化输出
来源：http://hn.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fg.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vf.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://li.lnxyls.cn

TS:   d.toISOString()
来源：http://ne.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tu.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kb.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pb.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lp.521024.cn

[J03] 字符串解析为日期
来源：http://sm.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vg.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ec.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://er.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://rd.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gg.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dh.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://eo.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xn.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://rd.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fg.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jj.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kk.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bn.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qx.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://da.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mk.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gf.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ib.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://yn.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bg.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ze.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ql.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://iw.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qi.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://he.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uk.hahajie.cn

[J06] 计算两时间之差
来源：http://fx.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ip.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ct.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qy.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ok.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nt.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://xp.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://ib.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://sl.szsharing.cn

[J07] 比较两个日期
来源：http://dc.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://go.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lv.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://te.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xe.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kb.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kx.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ce.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://uk.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jt.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nn.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://no.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://in.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pe.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vd.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dx.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kx.bjjhwx.cn

[J09] 时区处理
来源：http://to.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bq.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gi.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://go.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tv.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://se.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gp.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hu.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lr.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://wq.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zo.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ev.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jc.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mi.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xo.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tt.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ja.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pe.hnjuh.cn

================================================================================
来源：http://gp.9csxet.cn

K. JSON 与序列化
来源：http://pd.asd995.cn

================================================================================
来源：http://fg.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://of.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qv.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nd.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://tw.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://hv.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vc.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://wa.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uo.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ek.nicolike.cn

[K02] JSON 字符串转对象
来源：http://xq.yuexingan06.cn

Py:   json.loads(s)
来源：http://zd.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ms.panjiajie.cn

JS:   JSON.parse(s)
来源：http://fe.szxytkj.cn

TS:   JSON.parse(s)
来源：http://xz.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jk.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://sq.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://pw.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kj.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://zv.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qo.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kf.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lb.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://if.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ig.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jy.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wc.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ca.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://yz.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ya.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hi.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xt.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ba.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sf.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fp.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qb.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mq.yuexingan06.cn

[K05] 深拷贝对象
来源：http://el.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://ad.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ev.nszjky.cn

JS:   structuredClone(obj)
来源：http://ex.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://qf.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vp.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xb.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zn.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ua.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://jf.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vc.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oo.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kh.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jg.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qm.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ea.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nq.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fn.huanxung.cn

[K07] 进制转换
来源：http://zh.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://go.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bp.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tw.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fz.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jx.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oz.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sg.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jl.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://nv.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://mb.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://og.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://er.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://jd.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ru.nicolike.cn

Go:   encoding/gob
来源：http://yq.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://uu.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oe.9csxet.cn

================================================================================
来源：http://nq.wgjwhj.cn

L. 网络请求
来源：http://cw.nszjky.cn

================================================================================
来源：http://iv.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://jc.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pe.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eh.panjiajie.cn

JS:   await fetch(url)
来源：http://kx.huanxung.cn

TS:   await fetch(url)
来源：http://ww.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dp.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://yg.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mw.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yt.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://eo.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aw.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xz.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zp.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gz.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bc.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ew.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qv.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kk.hnjuh.cn


<!-- 参考信息 -->