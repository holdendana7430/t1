代发 wailian999

JS:   class MyError extends Error {}
来源：http://jr.newstarts.cn

TS:   class MyError extends Error {}
来源：http://lk.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://dg.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oe.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://zv.521024.cn

C#:   class MyException : Exception {}
来源：http://kb.shxzukj.cn

[H05] 捕获特定类型
来源：http://xn.yuexingan06.cn

Py:   except ValueError as e:
来源：http://gi.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zb.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://fj.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://rk.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://dz.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jp.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://dh.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ux.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://ui.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://st.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ui.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xm.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xl.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jg.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ls.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://sh.colortex.cn

[H07] 断言
来源：http://ev.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ek.panjiajie.cn

PHP:  assert($x > 0);
来源：http://vl.szsharing.cn

JS:   console.assert(x > 0);
来源：http://vi.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://vd.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://ff.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qa.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yg.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://qp.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://ef.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://fp.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://it.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://ci.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ok.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kd.hahajie.cn

Go:   err.Error()
来源：http://ng.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://yz.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://en.chemitech.net.cn

[H09] 带错误码的异常
来源：http://zt.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ok.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bq.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lu.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bi.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ce.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hx.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uy.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cg.shxzukj.cn

[H10] 资源自动释放
来源：http://qh.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uk.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xt.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nu.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://an.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fv.panjiajie.cn

Go:   defer f.Close()
来源：http://hc.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dp.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vp.shxzukj.cn

================================================================================
来源：http://wg.gzmigu.cn

I. 正则表达式
来源：http://ao.huixinmuqiang.cn

================================================================================
来源：http://yf.muxihuayi.cn

[I01] 判断是否匹配
来源：http://bq.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ut.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mi.colortex.cn

JS:   /\d+/.test(s)
来源：http://qg.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://hm.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vb.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jv.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://eg.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zy.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://pu.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://pi.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kq.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mu.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://bd.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sx.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fv.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://an.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ug.shxzukj.cn

[I03] 提取捕获分组
来源：http://bm.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gv.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lg.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ay.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bk.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sj.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kp.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wb.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tq.panjiajie.cn

[I04] 正则替换
来源：http://nw.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wy.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://za.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hl.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wl.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nk.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gr.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lc.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ye.wgjwhj.cn

[I05] 按正则拆分
来源：http://sq.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vs.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uk.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://ut.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ae.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://et.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tf.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tl.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ab.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fn.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vu.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ls.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bw.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wd.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sn.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bs.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yb.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rh.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://dc.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jp.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jh.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://to.521024.cn

TS:   /error/gim
来源：http://ra.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bc.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ra.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://eg.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fw.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rm.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fr.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fx.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hf.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bl.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iv.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wz.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pj.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qb.haigaiapp.cn

================================================================================
来源：http://ey.newstarts.cn

J. 日期与时间
来源：http://xn.shxzukj.cn

================================================================================
来源：http://jc.gzmigu.cn

[J01] 获取当前时间
来源：http://dq.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dx.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lg.newstarts.cn

JS:   new Date();  Date.now()
来源：http://ux.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://if.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://my.lnxyls.cn

Go:   time.Now()
来源：http://xu.gzmigu.cn

Ruby: Time.now
来源：http://zv.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bm.hahajie.cn

[J02] 格式化输出
来源：http://gc.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ex.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wm.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ci.jctech888.com.cn

TS:   d.toISOString()
来源：http://hl.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fu.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://se.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zx.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sz.asd995.cn

[J03] 字符串解析为日期
来源：http://rp.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fy.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tb.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://lb.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://hw.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ko.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://cf.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ha.newstarts.cn

[J04] 时间戳与日期互转
来源：http://fj.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ge.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cz.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sy.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qw.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hv.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xx.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cg.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zc.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://my.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://bo.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yk.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pw.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ds.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://uc.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pc.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://kt.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dz.shxzukj.cn

[J06] 计算两时间之差
来源：http://fr.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://jh.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://yk.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qj.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hr.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qo.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://bk.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://tr.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://cn.hahajie.cn

[J07] 比较两个日期
来源：http://gj.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://tf.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fh.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vp.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nz.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zc.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jy.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gs.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://rz.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ph.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dx.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dq.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cc.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uw.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ew.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fa.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yl.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ae.jctech888.com.cn

[J09] 时区处理
来源：http://zj.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ry.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dk.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pn.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jj.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sf.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nv.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cv.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ze.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ub.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://op.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dx.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bp.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tb.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bx.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kr.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ck.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yv.shxzukj.cn

================================================================================
来源：http://it.shtwfgs.cn

K. JSON 与序列化
来源：http://yl.huixiangedu.cn

================================================================================
来源：http://it.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://qg.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://te.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hr.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://yw.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://od.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://io.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://yi.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tx.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fq.colortex.cn

[K02] JSON 字符串转对象
来源：http://jl.shxzukj.cn

Py:   json.loads(s)
来源：http://ad.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sg.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://fi.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://nl.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hf.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://cw.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ro.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vo.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://qg.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://up.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ye.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pu.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dv.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wo.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://si.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://me.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zs.hahajie.cn

[K04] 读取 JSON 文件
来源：http://mz.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uc.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xq.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sz.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ea.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://de.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xc.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xf.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jd.hnjuh.cn

[K05] 深拷贝对象
来源：http://nh.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ei.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://wn.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://lo.newstarts.cn

TS:   structuredClone(obj)
来源：http://cq.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hr.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vu.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://if.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://is.asd995.cn

[K06] 解析 URL 查询串
来源：http://em.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vz.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qd.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uu.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tl.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aq.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xf.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rb.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eg.shxzukj.cn

[K07] 进制转换
来源：http://hu.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nu.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://om.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zi.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zp.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bt.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ge.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bw.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ck.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://fv.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ol.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wm.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://yf.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://bx.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dz.yuexingan06.cn


<!-- 参考信息 -->