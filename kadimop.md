代发 wailian999

[H07] 断言
来源：http://dv.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://wt.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://lh.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://bq.nszjky.cn

TS:   console.assert(x > 0);
来源：http://ls.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://sg.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nl.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ou.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://qd.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://tl.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pm.colortex.cn

JS:   e.message;  e.stack
来源：http://zv.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ur.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mm.9csxet.cn

Go:   err.Error()
来源：http://eo.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://jn.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://fw.szsharing.cn

[H09] 带错误码的异常
来源：http://qs.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xe.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bt.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cm.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ef.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nu.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ac.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ej.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gg.9csxet.cn

[H10] 资源自动释放
来源：http://xt.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gf.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xk.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nf.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jg.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sk.szxytkj.cn

Go:   defer f.Close()
来源：http://ee.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lb.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rm.521024.cn

================================================================================
来源：http://so.hnjuh.cn

I. 正则表达式
来源：http://be.lnxyls.cn

================================================================================
来源：http://fu.jctech888.com.cn

[I01] 判断是否匹配
来源：http://bd.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ih.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aa.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://fz.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://tv.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://my.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hg.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://eg.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://px.shxzskj.cn

[I02] 提取所有匹配
来源：http://mi.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://ia.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hb.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://et.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://pc.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://it.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uw.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://sj.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yr.521024.cn

[I03] 提取捕获分组
来源：http://uo.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ol.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ko.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xy.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pr.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mh.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ub.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sx.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qu.jianghongdianzi.cn

[I04] 正则替换
来源：http://sx.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://db.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ye.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://th.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ej.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fh.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xm.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lg.gzmigu.cn

[I05] 按正则拆分
来源：http://xg.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ic.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ih.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ew.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ox.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://gw.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wc.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uf.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://of.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ly.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nm.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://px.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pq.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vj.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oj.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kw.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lh.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jr.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://nq.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://co.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qc.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sl.muxihuayi.cn

TS:   /error/gim
来源：http://dk.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gx.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bs.asd995.cn

Ruby: s.scan(/error/i)
来源：http://sq.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iu.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://zp.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cd.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bu.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ra.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fo.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sd.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nt.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ba.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://up.yuntaijiaju.cn

================================================================================
来源：http://qr.bjjhwx.cn

J. 日期与时间
来源：http://mo.521024.cn

================================================================================
来源：http://hy.jctech888.com.cn

[J01] 获取当前时间
来源：http://bw.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vw.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rz.asd995.cn

JS:   new Date();  Date.now()
来源：http://wy.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://gq.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wx.nszjky.cn

Go:   time.Now()
来源：http://mp.hahajie.cn

Ruby: Time.now
来源：http://qa.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gk.asd995.cn

[J02] 格式化输出
来源：http://td.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bb.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://or.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dq.9csxet.cn

TS:   d.toISOString()
来源：http://sj.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://et.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cu.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yx.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jf.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://xn.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uw.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gn.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://bh.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://ym.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zg.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zb.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://ot.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tu.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://xn.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://su.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sh.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ez.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ug.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yl.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xj.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tg.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://dz.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://cd.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ci.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://po.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dx.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://dh.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dj.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://of.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://by.szsharing.cn

[J06] 计算两时间之差
来源：http://sy.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://sq.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://wj.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hy.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sx.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ol.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://zt.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://kj.jctech888.com.cn

[J07] 比较两个日期
来源：http://mo.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://sm.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eb.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wi.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rz.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wb.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://il.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://sx.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://na.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hw.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wf.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yj.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tl.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ua.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yp.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jv.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ns.huixiangedu.cn

[J09] 时区处理
来源：http://fk.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cs.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ls.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vh.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xd.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://es.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bx.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nh.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gm.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://op.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hj.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vb.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cp.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lp.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mm.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ut.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ve.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ap.muxihuayi.cn

================================================================================
来源：http://zi.szxytkj.cn

K. JSON 与序列化
来源：http://ii.chemitech.net.cn

================================================================================
来源：http://iz.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://pu.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vk.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kf.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://eh.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://sp.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pb.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://sd.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://im.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sc.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://zp.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ns.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jm.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ga.panjiajie.cn

TS:   JSON.parse(s)
来源：http://pk.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fx.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ap.nszjky.cn

Ruby: JSON.parse(s)
来源：http://hp.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mk.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ms.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ni.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bj.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ef.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dl.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qe.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tp.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dl.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oa.nszjky.cn

[K04] 读取 JSON 文件
来源：http://wb.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vx.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lz.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tv.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xi.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zr.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ht.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://od.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lv.colortex.cn

[K05] 深拷贝对象
来源：http://vg.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://dx.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://hi.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ag.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://sk.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iv.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pv.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ta.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bj.hahajie.cn

[K06] 解析 URL 查询串
来源：http://ub.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rt.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wp.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vd.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bb.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bj.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ca.jianghongdianzi.cn

[K07] 进制转换
来源：http://an.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uy.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qp.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yf.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://df.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gj.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xn.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ru.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://jt.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://rl.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sy.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://ev.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://ps.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qa.huanxung.cn

Go:   encoding/gob
来源：http://lf.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://sk.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aa.jctech888.com.cn

================================================================================
来源：http://hr.shxzukj.cn

L. 网络请求
来源：http://du.yuntaijiaju.cn

================================================================================
来源：http://st.hahajie.cn

[L01] 发送 GET 请求
来源：http://ic.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cq.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gj.shxzskj.cn

JS:   await fetch(url)
来源：http://ta.newstarts.cn

TS:   await fetch(url)
来源：http://dc.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wq.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://bo.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dp.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kk.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://vr.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ga.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vt.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bu.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ni.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vg.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zm.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://we.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ht.jianghongdianzi.cn


<!-- 参考信息 -->