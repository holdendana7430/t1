代发 wailian999

JS:   class MyError extends Error {}
来源：http://ue.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://qp.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://wk.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://td.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://xa.521024.cn

C#:   class MyException : Exception {}
来源：http://ee.szxytkj.cn

[H05] 捕获特定类型
来源：http://lf.nszjky.cn

Py:   except ValueError as e:
来源：http://ra.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://as.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://bb.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://bk.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://xd.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qk.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://sr.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zf.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://mb.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://tv.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zo.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://om.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rq.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://db.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://de.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://gn.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://sl.9csxet.cn

[H07] 断言
来源：http://jx.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://nx.panjiajie.cn

PHP:  assert($x > 0);
来源：http://yi.huanxung.cn

JS:   console.assert(x > 0);
来源：http://jo.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://wj.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://mo.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ks.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zm.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://wp.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://nz.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://sx.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uy.hahajie.cn

JS:   e.message;  e.stack
来源：http://aj.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://im.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cq.bookmarksfly.cn

Go:   err.Error()
来源：http://mx.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://pq.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://ii.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://pj.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vc.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mh.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kg.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eo.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bo.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mq.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jy.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ho.bjjhwx.cn

[H10] 资源自动释放
来源：http://mf.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://so.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xh.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gx.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nv.newstarts.cn

Go:   defer f.Close()
来源：http://xh.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qv.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://up.nszjky.cn

================================================================================
来源：http://ar.huixiangedu.cn

I. 正则表达式
来源：http://wq.newstarts.cn

================================================================================
来源：http://qv.huixiangedu.cn

[I01] 判断是否匹配
来源：http://ef.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ec.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sr.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://xx.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://rv.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gv.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://au.521024.cn

Ruby: s.match?(/\d+/)
来源：http://ip.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zn.shxzskj.cn

[I02] 提取所有匹配
来源：http://xl.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://pu.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dh.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hf.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://jk.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ju.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mt.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ob.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ja.colortex.cn

[I03] 提取捕获分组
来源：http://gz.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://po.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nk.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dt.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mm.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://du.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://le.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bq.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lo.muxihuayi.cn

[I04] 正则替换
来源：http://pq.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yn.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dj.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ak.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wy.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qo.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ie.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ut.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://at.shxzukj.cn

[I05] 按正则拆分
来源：http://ex.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vt.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ri.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://pl.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://ce.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://cg.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nb.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zj.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qv.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iu.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mv.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zy.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hg.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hp.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dj.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yf.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://on.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uc.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://oy.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dg.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bh.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mz.bookmarksfly.cn

TS:   /error/gim
来源：http://ul.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://li.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lo.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://rs.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xs.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://ig.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vf.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rs.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://po.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tz.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dr.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vl.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pc.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cu.yuexingan06.cn

================================================================================
来源：http://ey.9csxet.cn

J. 日期与时间
来源：http://aw.szxytkj.cn

================================================================================
来源：http://ug.shxzskj.cn

[J01] 获取当前时间
来源：http://hp.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gm.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qu.nicolike.cn

JS:   new Date();  Date.now()
来源：http://jf.asd995.cn

TS:   new Date();  Date.now()
来源：http://mf.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gu.jianghongdianzi.cn

Go:   time.Now()
来源：http://vz.huanxung.cn

Ruby: Time.now
来源：http://ql.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ru.yuntaijiaju.cn

[J02] 格式化输出
来源：http://ge.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ol.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://on.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tg.huanxung.cn

TS:   d.toISOString()
来源：http://ay.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xb.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pk.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://is.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eo.colortex.cn

[J03] 字符串解析为日期
来源：http://sy.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gw.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tb.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://bg.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://ue.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tc.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bc.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://tg.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bb.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://fj.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vo.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oe.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sc.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wl.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://up.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://df.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wm.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ws.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ay.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://nw.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gp.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pq.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://su.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://va.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://th.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://wz.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ro.colortex.cn

[J06] 计算两时间之差
来源：http://xi.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://wb.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://lc.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rl.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xq.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://vi.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://hy.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://le.asd995.cn

[J07] 比较两个日期
来源：http://fo.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ez.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qa.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wa.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fy.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nc.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gj.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kd.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://hx.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://hj.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ix.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ww.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tj.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vt.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hg.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pv.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qe.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://is.szxytkj.cn

[J09] 时区处理
来源：http://dm.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yw.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ld.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eq.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dn.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://al.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://an.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dt.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lm.521024.cn

[J10] 取今天 / 本月第一天
来源：http://sc.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kk.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://al.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pk.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fn.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ai.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zn.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ri.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ny.yuntaijiaju.cn

================================================================================
来源：http://ok.jianghongdianzi.cn

K. JSON 与序列化
来源：http://hq.haigaiapp.cn

================================================================================
来源：http://hv.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ek.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ni.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zm.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://vx.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://or.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kw.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://xv.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lc.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yw.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://zm.szsharing.cn

Py:   json.loads(s)
来源：http://hj.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ni.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://zo.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://nx.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sk.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://di.szsharing.cn

Ruby: JSON.parse(s)
来源：http://og.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://od.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://kl.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tw.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ki.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ws.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yi.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rn.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zi.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xr.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://te.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://op.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kg.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://df.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ur.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hh.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pn.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cx.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wi.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kf.hahajie.cn

[K05] 深拷贝对象
来源：http://dl.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://km.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://xt.colortex.cn

JS:   structuredClone(obj)
来源：http://vv.szsharing.cn

TS:   structuredClone(obj)
来源：http://xg.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rm.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lq.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eb.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wb.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://tr.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lh.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fd.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qd.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qa.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hc.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vz.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qw.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nc.521024.cn

[K07] 进制转换
来源：http://qx.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bg.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zx.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fp.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fv.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qh.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mb.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ny.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rt.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ob.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://fc.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xu.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://du.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://kr.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gu.asd995.cn


<!-- 参考信息 -->