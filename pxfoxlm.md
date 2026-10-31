代发 wailian999

Py:   value = d.get("k") or default
来源：http://om.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rj.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pu.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xz.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yd.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wb.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://lr.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://ly.chemitech.net.cn

[H07] 断言
来源：http://wv.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://rh.nszjky.cn

PHP:  assert($x > 0);
来源：http://jy.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://my.newstarts.cn

TS:   console.assert(x > 0);
来源：http://vp.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://ph.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mn.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fa.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://vb.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://on.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://yh.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rp.panjiajie.cn

JS:   e.message;  e.stack
来源：http://it.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xu.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dw.9csxet.cn

Go:   err.Error()
来源：http://iu.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://gs.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://ha.9csxet.cn

[H09] 带错误码的异常
来源：http://dn.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bl.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rr.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://in.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gf.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vg.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xl.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xu.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qw.szsharing.cn

[H10] 资源自动释放
来源：http://gr.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ev.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ia.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ly.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://my.nicolike.cn

Go:   defer f.Close()
来源：http://qc.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ei.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kr.asd995.cn

================================================================================
来源：http://ol.9csxet.cn

I. 正则表达式
来源：http://wl.jianghongdianzi.cn

================================================================================
来源：http://pc.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://mo.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hf.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ks.newstarts.cn

JS:   /\d+/.test(s)
来源：http://ti.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://sa.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wt.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vk.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://vt.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://no.yuexingan06.cn

[I02] 提取所有匹配
来源：http://yh.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://cf.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yw.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gz.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://jr.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zy.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://eh.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qk.asd995.cn

[I03] 提取捕获分组
来源：http://dm.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tv.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nn.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://of.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qc.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fu.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zn.bookmarksfly.cn

[I04] 正则替换
来源：http://uh.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tr.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ea.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cd.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://si.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mh.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dc.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wy.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gv.lnxyls.cn

[I05] 按正则拆分
来源：http://un.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ur.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wa.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://hz.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://dv.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://xs.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hb.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gs.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pn.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qo.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ze.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jb.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cc.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lt.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oq.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xz.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fw.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://as.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bc.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ty.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://en.newstarts.cn

TS:   /error/gim
来源：http://tb.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ro.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://im.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://yg.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hv.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://io.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mu.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dq.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yv.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://km.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yg.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ml.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ql.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sn.521024.cn

================================================================================
来源：http://ul.shtwfgs.cn

J. 日期与时间
来源：http://ej.jianghongdianzi.cn

================================================================================
来源：http://gm.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://bw.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wk.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ex.szsharing.cn

JS:   new Date();  Date.now()
来源：http://nt.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://fa.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ic.haigaiapp.cn

Go:   time.Now()
来源：http://us.huixiangedu.cn

Ruby: Time.now
来源：http://ou.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bu.bookmarksfly.cn

[J02] 格式化输出
来源：http://wk.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sb.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://js.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ij.hahajie.cn

TS:   d.toISOString()
来源：http://br.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://br.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://um.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eg.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bt.shxzskj.cn

[J03] 字符串解析为日期
来源：http://mf.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pv.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zz.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://oq.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://ed.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iy.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xc.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://kf.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pf.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://fr.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dd.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ri.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://by.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ke.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jm.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qs.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ez.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cx.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://th.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://ww.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fe.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://my.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qf.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://tp.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ek.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://rs.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nt.asd995.cn

[J06] 计算两时间之差
来源：http://gj.asd995.cn

Py:   (end - start).total_seconds()
来源：http://ou.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://zb.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dr.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vz.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nj.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ej.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://jy.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://at.szsharing.cn

[J07] 比较两个日期
来源：http://mh.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://mi.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dr.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://er.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ss.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lx.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mx.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ai.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://tw.panjiajie.cn

[J08] 提取年月日与星期
来源：http://dc.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zx.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jv.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ah.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uc.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vd.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fa.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ft.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bv.huixinmuqiang.cn

[J09] 时区处理
来源：http://bd.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qt.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rd.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uk.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hb.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xq.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nj.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ed.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vu.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://lu.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cp.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mt.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ug.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cb.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kj.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vq.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://js.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ly.jianghongdianzi.cn

================================================================================
来源：http://jf.nszjky.cn

K. JSON 与序列化
来源：http://fc.lnxyls.cn

================================================================================
来源：http://om.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://bi.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://go.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jh.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://aq.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://vt.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://le.nicolike.cn

Go:   json.Marshal(obj)
来源：http://pm.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mn.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uo.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://wz.yuexingan06.cn

Py:   json.loads(s)
来源：http://sk.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.szxytkj.cn

JS:   JSON.parse(s)
来源：http://fc.asd995.cn

TS:   JSON.parse(s)
来源：http://ew.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wm.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://ux.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://zi.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xx.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://kz.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ut.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kw.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fq.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aq.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ze.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ki.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mf.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bj.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://kt.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ep.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fr.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ut.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ek.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kd.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ua.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ad.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ak.hahajie.cn

[K05] 深拷贝对象
来源：http://pk.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://yn.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://py.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://mm.panjiajie.cn

TS:   structuredClone(obj)
来源：http://rr.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hi.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ww.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qb.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dj.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://qs.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rm.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yj.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pe.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mz.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://az.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sb.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vs.szxytkj.cn

[K07] 进制转换
来源：http://dk.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ei.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uu.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kx.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iv.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://om.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yb.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fz.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gd.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ee.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://sv.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yc.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://es.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://cb.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dw.bookmarksfly.cn

Go:   encoding/gob
来源：http://vl.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://ea.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gw.muxihuayi.cn

================================================================================
来源：http://fu.bookmarksfly.cn

L. 网络请求
来源：http://vz.jctech888.com.cn

================================================================================
来源：http://ku.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://gm.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ax.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ad.huanxung.cn

JS:   await fetch(url)
来源：http://uo.hnjuh.cn

TS:   await fetch(url)
来源：http://yy.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rf.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://kd.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ly.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yx.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://iq.shtwfgs.cn


<!-- 参考信息 -->