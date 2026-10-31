代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://qo.chemitech.net.cn

[H04] 自定义异常类型
来源：http://lx.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://uq.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ce.nicolike.cn

JS:   class MyError extends Error {}
来源：http://rl.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://as.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://lp.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dk.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://td.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://hr.shxzskj.cn

[H05] 捕获特定类型
来源：http://ie.huanxung.cn

Py:   except ValueError as e:
来源：http://ri.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sd.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://lb.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://km.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://gv.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aq.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://pa.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ov.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://ov.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://im.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yn.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yg.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ey.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ha.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ui.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://xz.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://sb.jctech888.com.cn

[H07] 断言
来源：http://oj.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://lg.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://ov.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://el.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://xn.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://uw.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wh.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://js.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://co.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://qn.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://av.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zw.szxytkj.cn

JS:   e.message;  e.stack
来源：http://ti.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rg.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aa.haigaiapp.cn

Go:   err.Error()
来源：http://cg.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://bg.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://vn.panjiajie.cn

[H09] 带错误码的异常
来源：http://tf.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dd.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ng.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://am.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vn.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ib.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xw.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ms.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iz.chemitech.net.cn

[H10] 资源自动释放
来源：http://ld.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nj.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xr.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pe.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://un.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://on.chemitech.net.cn

Go:   defer f.Close()
来源：http://ih.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ce.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ue.shxzskj.cn

================================================================================
来源：http://qu.lnxyls.cn

I. 正则表达式
来源：http://qe.shxzukj.cn

================================================================================
来源：http://th.szsharing.cn

[I01] 判断是否匹配
来源：http://bc.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kr.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jl.huanxung.cn

JS:   /\d+/.test(s)
来源：http://xx.9csxet.cn

TS:   /\d+/.test(s)
来源：http://fx.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vx.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gv.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://kw.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vl.9csxet.cn

[I02] 提取所有匹配
来源：http://lh.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://wz.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rg.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sh.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://rj.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iz.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mf.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://hk.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zs.9csxet.cn

[I03] 提取捕获分组
来源：http://tu.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://je.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fu.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://co.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ef.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ig.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://st.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dd.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://we.asd995.cn

[I04] 正则替换
来源：http://lt.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://in.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mj.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xy.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://do.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wz.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ih.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ch.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qa.bookmarksfly.cn

[I05] 按正则拆分
来源：http://el.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ps.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://av.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://tn.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://hj.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://jz.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fe.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tr.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ns.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xi.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wb.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://su.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yh.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ik.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zc.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cu.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sy.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://bf.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xu.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mu.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gx.huanxung.cn

TS:   /error/gim
来源：http://lh.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ge.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vh.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://hk.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zx.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://ex.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ga.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kh.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ig.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ct.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wh.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wy.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dm.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://el.hahajie.cn

================================================================================
来源：http://kv.nszjky.cn

J. 日期与时间
来源：http://jh.asd995.cn

================================================================================
来源：http://tp.shxzskj.cn

[J01] 获取当前时间
来源：http://kx.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ws.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jh.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://gs.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://je.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oi.newstarts.cn

Go:   time.Now()
来源：http://ar.szxytkj.cn

Ruby: Time.now
来源：http://qm.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ok.lnxyls.cn

[J02] 格式化输出
来源：http://su.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fg.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ft.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xa.szxytkj.cn

TS:   d.toISOString()
来源：http://om.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vt.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vo.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kq.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ll.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://ds.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eo.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://co.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://wm.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://yi.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://he.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ia.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ln.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yg.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://jg.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ev.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zv.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://di.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qv.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bz.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lx.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://up.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qt.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://yb.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://jw.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ls.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iy.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hu.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://zu.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xk.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://pt.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cu.newstarts.cn

[J06] 计算两时间之差
来源：http://fq.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://my.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://if.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cn.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cb.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ov.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://cl.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://gx.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://ad.hahajie.cn

[J07] 比较两个日期
来源：http://qx.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://qi.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vd.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xz.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://li.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ec.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cq.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zh.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ez.521024.cn

[J08] 提取年月日与星期
来源：http://fw.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wn.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mx.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yj.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gn.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lf.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yw.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ov.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lu.szsharing.cn

[J09] 时区处理
来源：http://nq.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://df.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ga.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dv.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fe.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xr.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ub.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tv.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://jz.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xj.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jf.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pf.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jf.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vc.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://et.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ye.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hf.bookmarksfly.cn

================================================================================
来源：http://mc.huanxung.cn

K. JSON 与序列化
来源：http://ll.gzmigu.cn

================================================================================
来源：http://ms.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://nl.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lx.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rj.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://oq.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://ir.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ra.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://gw.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pb.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fe.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://vf.newstarts.cn

Py:   json.loads(s)
来源：http://vi.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vr.szxytkj.cn

JS:   JSON.parse(s)
来源：http://hm.szsharing.cn

TS:   JSON.parse(s)
来源：http://cc.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ag.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://zi.newstarts.cn

Ruby: JSON.parse(s)
来源：http://fr.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://er.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://hy.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ew.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nt.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sq.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://br.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ry.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jv.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zv.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://og.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ae.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wv.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cw.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vt.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qm.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sw.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bo.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ub.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://af.lnxyls.cn

[K05] 深拷贝对象
来源：http://lc.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://rf.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://or.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://va.shxzukj.cn

TS:   structuredClone(obj)
来源：http://td.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eq.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oi.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gv.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qu.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://us.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cp.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tb.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qo.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tm.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ss.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zf.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qa.bookmarksfly.cn

[K07] 进制转换
来源：http://qm.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jl.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xi.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://be.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dt.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rf.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qj.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ty.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rw.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://zg.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://xb.bookmarksfly.cn


<!-- 参考信息 -->