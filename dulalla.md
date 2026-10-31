代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://qw.hnjuh.cn

[H04] 自定义异常类型
来源：http://aq.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://kz.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kb.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ws.nicolike.cn

TS:   class MyError extends Error {}
来源：http://qm.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://qs.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dt.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://is.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://rw.lnxyls.cn

[H05] 捕获特定类型
来源：http://dp.panjiajie.cn

Py:   except ValueError as e:
来源：http://sv.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bh.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://nu.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://rh.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ol.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eo.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://ct.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qs.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://no.colortex.cn

Py:   value = d.get("k") or default
来源：http://mj.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yx.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ml.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kl.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aj.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zp.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://mj.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://tr.wgjwhj.cn

[H07] 断言
来源：http://re.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://sx.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ry.newstarts.cn

JS:   console.assert(x > 0);
来源：http://gw.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://yv.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://vl.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ky.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://em.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://ll.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://xx.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://dq.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lf.huanxung.cn

JS:   e.message;  e.stack
来源：http://zt.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://de.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yv.yuntaijiaju.cn

Go:   err.Error()
来源：http://wb.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://go.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://kk.lnxyls.cn

[H09] 带错误码的异常
来源：http://in.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://of.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tb.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qk.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rx.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ya.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cz.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rr.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tr.huixiangedu.cn

[H10] 资源自动释放
来源：http://zu.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kv.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ht.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pw.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uk.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ec.huanxung.cn

Go:   defer f.Close()
来源：http://ij.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jl.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pv.jianghongdianzi.cn

================================================================================
来源：http://al.chemitech.net.cn

I. 正则表达式
来源：http://me.yuexingan06.cn

================================================================================
来源：http://ir.szsharing.cn

[I01] 判断是否匹配
来源：http://wy.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://py.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zl.szsharing.cn

JS:   /\d+/.test(s)
来源：http://px.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://et.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iz.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xf.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://mi.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rn.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://gi.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://dy.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vj.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vm.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://gx.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sw.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ox.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://nu.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lu.yuexingan06.cn

[I03] 提取捕获分组
来源：http://ry.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dy.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wh.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rp.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cd.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vc.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hw.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fo.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://er.newstarts.cn

[I04] 正则替换
来源：http://pg.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hj.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mk.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qq.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qi.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ye.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pi.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ir.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://li.shtwfgs.cn

[I05] 按正则拆分
来源：http://lx.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qq.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fz.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://kq.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://yf.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://hh.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wp.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lz.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wi.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vb.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xd.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gm.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yt.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ei.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qv.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ca.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://os.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yu.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://kq.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yb.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jj.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oj.lnxyls.cn

TS:   /error/gim
来源：http://cg.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ol.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yh.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://ac.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bd.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://kb.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pi.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vo.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nz.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vf.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iq.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://su.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sn.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bs.colortex.cn

================================================================================
来源：http://fx.shtwfgs.cn

J. 日期与时间
来源：http://zb.bjjhwx.cn

================================================================================
来源：http://gh.nicolike.cn

[J01] 获取当前时间
来源：http://qw.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yk.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tf.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://pw.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ux.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ff.521024.cn

Go:   time.Now()
来源：http://zn.newstarts.cn

Ruby: Time.now
来源：http://az.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tt.hnjuh.cn

[J02] 格式化输出
来源：http://mg.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xg.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rq.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pz.hnjuh.cn

TS:   d.toISOString()
来源：http://nt.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vi.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ky.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zq.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mm.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://nv.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://de.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hv.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://xh.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://px.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fd.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mc.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://io.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zi.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://br.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ne.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nz.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://li.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xv.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fc.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dy.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wf.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uw.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://jn.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://gi.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sy.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hw.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pa.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ri.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ue.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://us.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mh.hahajie.cn

[J06] 计算两时间之差
来源：http://wq.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://hz.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://pi.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ly.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tp.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tj.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://vn.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://xa.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://rg.9csxet.cn

[J07] 比较两个日期
来源：http://bc.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://un.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xv.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tr.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uh.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nh.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ps.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pp.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://rk.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ih.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nm.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fc.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xb.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ld.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vo.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hh.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wk.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qf.colortex.cn

[J09] 时区处理
来源：http://nj.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fe.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qi.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vd.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ya.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://md.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bu.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://og.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pe.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://et.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cc.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uw.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ki.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lc.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://py.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ok.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yd.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mn.muxihuayi.cn

================================================================================
来源：http://jl.chemitech.net.cn

K. JSON 与序列化
来源：http://gj.yuntaijiaju.cn

================================================================================
来源：http://pg.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://my.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qh.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rr.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://du.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ni.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kv.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://zy.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fh.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rc.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://wq.nszjky.cn

Py:   json.loads(s)
来源：http://zo.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ms.hnjuh.cn

JS:   JSON.parse(s)
来源：http://dd.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://nx.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jb.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ju.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://vj.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dx.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://tt.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cu.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ck.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ih.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ud.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vz.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ei.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qi.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kc.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ni.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wi.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pi.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://to.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://js.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yk.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zh.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wb.nicolike.cn

[K05] 深拷贝对象
来源：http://hr.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://ni.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://nd.shxzukj.cn

JS:   structuredClone(obj)
来源：http://di.colortex.cn

TS:   structuredClone(obj)
来源：http://df.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dd.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oe.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jh.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ni.521024.cn

[K06] 解析 URL 查询串
来源：http://ti.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://or.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bd.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pv.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kd.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fs.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ig.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nw.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zj.shxzukj.cn

[K07] 进制转换
来源：http://sw.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ai.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://er.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ie.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://go.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ab.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hi.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oy.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dv.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://gl.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://ws.szxytkj.cn


<!-- 参考信息 -->