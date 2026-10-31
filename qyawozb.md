代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kv.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wc.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://mo.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://ga.bjjhwx.cn

[H07] 断言
来源：http://ou.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://zh.521024.cn

PHP:  assert($x > 0);
来源：http://qf.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://ap.szsharing.cn

TS:   console.assert(x > 0);
来源：http://rp.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://wb.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nd.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rz.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://pf.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://tv.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://qi.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fk.hahajie.cn

JS:   e.message;  e.stack
来源：http://pn.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jd.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mm.shxzukj.cn

Go:   err.Error()
来源：http://gg.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://vj.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ge.gzmigu.cn

[H09] 带错误码的异常
来源：http://dx.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dv.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yu.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aw.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sv.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ye.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zg.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ow.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://id.gzmigu.cn

[H10] 资源自动释放
来源：http://bu.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yc.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://km.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://st.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yu.nszjky.cn

Go:   defer f.Close()
来源：http://wa.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ae.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gu.shtwfgs.cn

================================================================================
来源：http://ky.9csxet.cn

I. 正则表达式
来源：http://ld.shtwfgs.cn

================================================================================
来源：http://km.shtwfgs.cn

[I01] 判断是否匹配
来源：http://pz.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qe.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uw.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://vc.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://it.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yk.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nu.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://br.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yc.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ep.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://sd.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mu.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pm.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://ms.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hb.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sn.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://iy.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://er.yuexingan06.cn

[I03] 提取捕获分组
来源：http://qf.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ba.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ep.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pa.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ei.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vh.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ns.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rr.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://js.nszjky.cn

[I04] 正则替换
来源：http://us.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nu.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qj.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xb.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pj.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://or.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ei.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iu.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rk.newstarts.cn

[I05] 按正则拆分
来源：http://lw.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ci.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ex.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wv.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://ki.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://es.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fs.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ww.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zy.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ie.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mg.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rt.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mg.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vs.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wy.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yq.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mo.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pk.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ve.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oq.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gl.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wn.bookmarksfly.cn

TS:   /error/gim
来源：http://wp.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://og.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ge.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://ik.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dc.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://mx.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fl.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kw.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://at.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lb.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://am.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qn.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://br.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hs.shtwfgs.cn

================================================================================
来源：http://jy.bookmarksfly.cn

J. 日期与时间
来源：http://az.panjiajie.cn

================================================================================
来源：http://fh.lnxyls.cn

[J01] 获取当前时间
来源：http://kf.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lj.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cn.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://fe.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://uo.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wu.yuntaijiaju.cn

Go:   time.Now()
来源：http://py.bookmarksfly.cn

Ruby: Time.now
来源：http://no.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ef.bookmarksfly.cn

[J02] 格式化输出
来源：http://fp.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ze.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ez.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cw.huixiangedu.cn

TS:   d.toISOString()
来源：http://vr.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jr.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://up.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://di.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ax.nicolike.cn

[J03] 字符串解析为日期
来源：http://cw.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nb.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ll.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://yp.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://ea.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sj.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nd.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://bh.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eu.nszjky.cn

[J04] 时间戳与日期互转
来源：http://aj.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sl.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qm.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vh.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wn.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zw.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gr.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jf.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ds.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://gv.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://xz.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lp.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sg.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://tx.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sd.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://yq.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ol.jctech888.com.cn

[J06] 计算两时间之差
来源：http://xh.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://uh.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://mk.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wu.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wc.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ng.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://ek.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ha.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://gk.bjjhwx.cn

[J07] 比较两个日期
来源：http://wh.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://vg.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://if.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aq.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wl.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yr.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cd.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oe.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://up.szsharing.cn

[J08] 提取年月日与星期
来源：http://zo.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ky.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gm.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yq.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zl.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bv.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ft.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uv.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ag.lnxyls.cn

[J09] 时区处理
来源：http://vp.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zf.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xu.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kr.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ct.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eb.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ij.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pu.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zs.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://dg.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ap.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wk.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ea.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wh.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vs.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xc.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aw.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ev.muxihuayi.cn

================================================================================
来源：http://ul.jianghongdianzi.cn

K. JSON 与序列化
来源：http://mp.newstarts.cn

================================================================================
来源：http://wm.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://gh.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://be.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pq.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://mt.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://cg.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bc.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ol.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kp.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mh.colortex.cn

[K02] JSON 字符串转对象
来源：http://zq.jctech888.com.cn

Py:   json.loads(s)
来源：http://tt.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ss.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://ue.gzmigu.cn

TS:   JSON.parse(s)
来源：http://vt.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://we.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ic.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://tm.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rh.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://pv.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yx.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jw.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qz.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qw.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pt.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vt.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rd.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fc.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://yi.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hd.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sg.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lz.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qu.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hy.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qg.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hg.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yp.colortex.cn

[K05] 深拷贝对象
来源：http://xg.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://rx.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://sn.nicolike.cn

JS:   structuredClone(obj)
来源：http://ze.gzmigu.cn

TS:   structuredClone(obj)
来源：http://uf.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zu.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xo.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zi.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uq.nszjky.cn

[K06] 解析 URL 查询串
来源：http://as.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rs.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zo.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cw.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dx.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ci.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oa.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bt.bjjhwx.cn

[K07] 进制转换
来源：http://te.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mb.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yt.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wg.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ro.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eg.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iu.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nt.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nd.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://zo.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://zb.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tj.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://bp.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://hw.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yo.521024.cn

Go:   encoding/gob
来源：http://dl.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://xi.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://rq.chemitech.net.cn

L. 网络请求
来源：http://xf.shtwfgs.cn

================================================================================
来源：http://hh.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://kf.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rn.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://et.bjjhwx.cn

JS:   await fetch(url)
来源：http://tx.wgjwhj.cn

TS:   await fetch(url)
来源：http://xp.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ke.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://ll.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cs.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uc.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://yx.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ym.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://py.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dj.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ph.szxytkj.cn


<!-- 参考信息 -->