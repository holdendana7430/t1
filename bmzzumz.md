代发 wailian999

Py:   value = d.get("k") or default
来源：http://vc.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vz.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://db.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://om.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ou.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sn.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ld.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://hw.szxytkj.cn

[H07] 断言
来源：http://ub.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://sx.nszjky.cn

PHP:  assert($x > 0);
来源：http://jg.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://wp.9csxet.cn

TS:   console.assert(x > 0);
来源：http://lq.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://iv.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://se.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ah.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://lb.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://fn.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://xi.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://io.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://ny.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ai.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ld.jctech888.com.cn

Go:   err.Error()
来源：http://ao.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://dr.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://kl.chemitech.net.cn

[H09] 带错误码的异常
来源：http://zi.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wh.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://by.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ot.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wx.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ze.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oo.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kh.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://je.hahajie.cn

[H10] 资源自动释放
来源：http://sg.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ki.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lr.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://py.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dk.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wt.9csxet.cn

Go:   defer f.Close()
来源：http://th.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dg.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aq.asd995.cn

================================================================================
来源：http://xs.yuexingan06.cn

I. 正则表达式
来源：http://no.nicolike.cn

================================================================================
来源：http://wr.bjjhwx.cn

[I01] 判断是否匹配
来源：http://xu.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hc.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lv.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://lc.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://oz.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ws.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ua.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://kq.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yv.gzmigu.cn

[I02] 提取所有匹配
来源：http://rq.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://jy.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zq.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zs.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://gv.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gy.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://gh.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tx.gzmigu.cn

[I03] 提取捕获分组
来源：http://jq.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tq.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://af.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ay.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cc.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tz.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pz.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dt.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vv.nszjky.cn

[I04] 正则替换
来源：http://yf.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zl.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ad.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bd.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mh.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ot.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nl.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://di.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pi.gzmigu.cn

[I05] 按正则拆分
来源：http://vv.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oq.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hr.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://di.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ey.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://uf.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://db.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dv.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yn.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wi.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bo.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ve.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aa.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nc.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hb.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mo.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ik.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://xa.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nt.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://to.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iz.521024.cn

TS:   /error/gim
来源：http://we.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pz.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vr.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://fj.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ws.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ee.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fp.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ft.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wb.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fz.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://av.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ky.shxzukj.cn

================================================================================
来源：http://wp.jianghongdianzi.cn

J. 日期与时间
来源：http://mx.gzmigu.cn

================================================================================
来源：http://oy.huixiangedu.cn

[J01] 获取当前时间
来源：http://ka.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fo.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cf.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://dv.nicolike.cn

TS:   new Date();  Date.now()
来源：http://yo.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wn.nicolike.cn

Go:   time.Now()
来源：http://or.nicolike.cn

Ruby: Time.now
来源：http://hb.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://an.huixinmuqiang.cn

[J02] 格式化输出
来源：http://xp.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hx.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lq.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hy.hahajie.cn

TS:   d.toISOString()
来源：http://er.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gi.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vl.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mv.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://by.521024.cn

[J03] 字符串解析为日期
来源：http://ws.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iq.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zb.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://oh.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://el.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zq.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rc.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://hi.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://db.hahajie.cn

[J04] 时间戳与日期互转
来源：http://cw.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xy.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://by.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ul.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ez.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mm.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ir.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xl.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://df.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://vs.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://we.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pt.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ga.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yn.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://qx.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ww.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://bz.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ix.hahajie.cn

[J06] 计算两时间之差
来源：http://dh.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://zo.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://nt.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ms.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tw.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pj.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://cn.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://lq.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://oq.jctech888.com.cn

[J07] 比较两个日期
来源：http://pt.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://dy.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hq.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jl.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bv.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yj.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mh.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://cr.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ej.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zz.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mj.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kj.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://az.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://br.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://be.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pe.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bp.lnxyls.cn

[J09] 时区处理
来源：http://bf.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zl.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uw.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://el.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ah.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fb.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gj.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mw.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ee.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://vj.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dn.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lm.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gn.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ol.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ov.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yo.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gj.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yu.szxytkj.cn

================================================================================
来源：http://kh.wgjwhj.cn

K. JSON 与序列化
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://pw.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://eh.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ow.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lo.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://ms.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://ok.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rz.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://ou.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bk.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vq.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://qf.521024.cn

Py:   json.loads(s)
来源：http://hq.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rw.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://gh.521024.cn

TS:   JSON.parse(s)
来源：http://hn.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://st.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://kg.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://xy.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ee.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://om.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kf.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://do.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mm.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tv.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vt.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dm.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rj.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fq.521024.cn

[K04] 读取 JSON 文件
来源：http://lv.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://al.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ei.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gq.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fp.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nt.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ij.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tw.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cf.newstarts.cn

[K05] 深拷贝对象
来源：http://bn.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ag.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://bk.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://lm.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://iw.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fu.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zb.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xm.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qw.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://jt.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aj.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oj.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fz.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kc.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hx.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://db.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pq.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uv.yuntaijiaju.cn

[K07] 进制转换
来源：http://fa.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://et.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qf.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eb.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pv.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yk.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rj.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qq.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nv.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://mc.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://zm.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ao.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ui.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://az.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kc.colortex.cn

Go:   encoding/gob
来源：http://mu.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://my.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uy.huixiangedu.cn

================================================================================
来源：http://cg.huixinmuqiang.cn

L. 网络请求
来源：http://eb.shxzukj.cn

================================================================================
来源：http://ju.szsharing.cn

[L01] 发送 GET 请求
来源：http://po.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fi.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cx.bjjhwx.cn

JS:   await fetch(url)
来源：http://qx.jctech888.com.cn

TS:   await fetch(url)
来源：http://at.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dj.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ys.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tf.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gq.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ep.9csxet.cn


<!-- 参考信息 -->