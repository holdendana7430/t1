代发 wailian999

Py:   value = d.get("k") or default
来源：http://kl.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mt.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ku.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://it.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dx.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bf.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://op.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ie.yuexingan06.cn

[H07] 断言
来源：http://li.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://im.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://tc.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://zf.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://ct.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://dr.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fh.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ij.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://xo.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://px.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://ar.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nv.asd995.cn

JS:   e.message;  e.stack
来源：http://zb.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://de.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xs.asd995.cn

Go:   err.Error()
来源：http://ps.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://ux.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://ed.huanxung.cn

[H09] 带错误码的异常
来源：http://vv.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oe.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ek.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ae.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cw.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ug.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bu.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wb.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ox.lnxyls.cn

[H10] 资源自动释放
来源：http://mm.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rr.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gu.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mg.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sn.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jd.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://vv.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fr.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bs.gzmigu.cn

================================================================================
来源：http://iz.shtwfgs.cn

I. 正则表达式
来源：http://jv.bjjhwx.cn

================================================================================
来源：http://lf.gzmigu.cn

[I01] 判断是否匹配
来源：http://lb.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jh.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hh.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://sc.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://uv.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ji.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eo.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ox.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ij.haigaiapp.cn

[I02] 提取所有匹配
来源：http://bi.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://ty.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oo.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kx.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://fl.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://za.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vr.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://up.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wh.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ge.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pq.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dg.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xq.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wg.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kc.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wo.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mr.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kf.hahajie.cn

[I04] 正则替换
来源：http://jm.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://br.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wy.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hm.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rn.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lq.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nk.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ou.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sw.nszjky.cn

[I05] 按正则拆分
来源：http://hm.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://go.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ag.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://tg.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://bi.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://mx.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gk.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fc.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ix.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xq.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sq.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zy.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fp.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ra.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hg.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://py.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kz.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fr.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://tk.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pm.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://my.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tg.huixiangedu.cn

TS:   /error/gim
来源：http://rt.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://su.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rj.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://po.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ft.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xw.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wj.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zt.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kn.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vp.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zg.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fa.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gf.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xt.bookmarksfly.cn

================================================================================
来源：http://it.nicolike.cn

J. 日期与时间
来源：http://jc.huanxung.cn

================================================================================
来源：http://lg.huixiangedu.cn

[J01] 获取当前时间
来源：http://aq.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ho.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yz.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://ov.colortex.cn

TS:   new Date();  Date.now()
来源：http://sx.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vn.jianghongdianzi.cn

Go:   time.Now()
来源：http://lf.9csxet.cn

Ruby: Time.now
来源：http://fq.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wb.huanxung.cn

[J02] 格式化输出
来源：http://bh.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cw.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ef.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kv.muxihuayi.cn

TS:   d.toISOString()
来源：http://wc.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ir.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://of.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sq.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mr.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://ez.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jl.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ec.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://iq.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://tk.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qr.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yu.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://bo.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cy.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://uw.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mx.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cq.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bu.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lf.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bs.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jm.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ng.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ol.521024.cn

[J05] 时间加减（加 7 天）
来源：http://bw.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://qa.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pz.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kj.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cx.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://rd.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kn.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://jd.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bd.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://bz.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://ua.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://rt.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wt.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://it.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zd.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://lw.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ke.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ic.szsharing.cn

[J07] 比较两个日期
来源：http://qj.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hc.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fq.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://is.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://en.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qk.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ey.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kv.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://ma.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ul.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kk.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vc.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oq.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oa.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ve.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wt.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bj.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fg.gzmigu.cn

[J09] 时区处理
来源：http://fn.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://te.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ui.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nu.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bt.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ya.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://si.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cz.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ki.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://mc.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://br.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://st.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dc.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kx.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xx.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jk.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qk.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ac.huixinmuqiang.cn

================================================================================
来源：http://yd.jctech888.com.cn

K. JSON 与序列化
来源：http://xi.gzmigu.cn

================================================================================
来源：http://yd.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://qa.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bj.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wv.521024.cn

JS:   JSON.stringify(obj)
来源：http://zh.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://rl.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jo.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://qd.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fn.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yf.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://pu.nszjky.cn

Py:   json.loads(s)
来源：http://ed.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gd.newstarts.cn

JS:   JSON.parse(s)
来源：http://ch.hahajie.cn

TS:   JSON.parse(s)
来源：http://na.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://du.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://mz.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://xs.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oq.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://hq.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dx.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zx.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ju.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://la.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gu.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ju.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ui.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zt.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://sn.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gx.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tz.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kn.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iz.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mj.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sh.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zl.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://al.huanxung.cn

[K05] 深拷贝对象
来源：http://cj.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://oa.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://gw.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://wg.hnjuh.cn

TS:   structuredClone(obj)
来源：http://fb.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://by.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vv.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vl.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lc.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://wm.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://af.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ey.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tr.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zd.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ir.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ix.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ph.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qs.jianghongdianzi.cn

[K07] 进制转换
来源：http://hl.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://na.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pj.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://te.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dw.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ir.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cy.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hs.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sw.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ki.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://hv.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ci.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ak.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://wh.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ni.panjiajie.cn

Go:   encoding/gob
来源：http://sb.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://qi.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mt.jctech888.com.cn

================================================================================
来源：http://ru.asd995.cn

L. 网络请求
来源：http://zb.shxzukj.cn

================================================================================
来源：http://po.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://an.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yo.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jg.yuexingan06.cn

JS:   await fetch(url)
来源：http://br.lnxyls.cn

TS:   await fetch(url)
来源：http://ve.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ss.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://zf.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pt.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dp.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://fc.bookmarksfly.cn


<!-- 参考信息 -->