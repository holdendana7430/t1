代发 wailian999

TS:   throw new Error("错误信息");
来源：http://sx.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bu.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kw.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hl.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iq.nszjky.cn

[H04] 自定义异常类型
来源：http://mu.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://uj.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kh.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://bp.szsharing.cn

TS:   class MyError extends Error {}
来源：http://qr.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://yz.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wp.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://px.nszjky.cn

C#:   class MyException : Exception {}
来源：http://sg.szxytkj.cn

[H05] 捕获特定类型
来源：http://xc.wgjwhj.cn

Py:   except ValueError as e:
来源：http://vs.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ji.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://yv.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://yu.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://zv.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://em.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://ll.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vd.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://ps.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://vn.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ae.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dx.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://if.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lw.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dh.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://ut.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://mp.jctech888.com.cn

[H07] 断言
来源：http://yg.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://hk.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://qf.colortex.cn

JS:   console.assert(x > 0);
来源：http://lu.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://yv.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://qm.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jl.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ul.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://za.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://uo.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://pk.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://he.hnjuh.cn

JS:   e.message;  e.stack
来源：http://eu.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lz.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nv.lnxyls.cn

Go:   err.Error()
来源：http://ba.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://ud.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://xi.huanxung.cn

[H09] 带错误码的异常
来源：http://ut.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yy.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ll.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://na.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iq.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ts.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rr.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vy.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vq.521024.cn

[H10] 资源自动释放
来源：http://uk.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pj.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://am.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rd.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hq.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://om.bjjhwx.cn

Go:   defer f.Close()
来源：http://bg.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lv.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qc.huixinmuqiang.cn

================================================================================
来源：http://gr.yuexingan06.cn

I. 正则表达式
来源：http://uq.panjiajie.cn

================================================================================
来源：http://yw.newstarts.cn

[I01] 判断是否匹配
来源：http://gz.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wg.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gl.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://ui.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://qx.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vo.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hp.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://bi.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gw.szxytkj.cn

[I02] 提取所有匹配
来源：http://ga.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://qu.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sk.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tp.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://zw.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://au.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tq.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://fu.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://of.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://bb.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uf.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xx.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://py.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xg.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tk.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fo.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vm.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jw.521024.cn

[I04] 正则替换
来源：http://uf.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pq.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dc.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ro.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rc.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rw.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gt.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nu.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zc.nszjky.cn

[I05] 按正则拆分
来源：http://ig.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lw.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wx.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://tt.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://in.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://zq.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ba.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ip.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://he.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ck.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qu.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://on.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fh.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ou.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kz.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oc.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://fo.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tk.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cw.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mb.gzmigu.cn

TS:   /error/gim
来源：http://wz.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iq.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uh.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://yj.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ba.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://zx.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://no.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://co.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ad.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ry.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ad.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ly.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cf.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bz.jctech888.com.cn

================================================================================
来源：http://yk.szxytkj.cn

J. 日期与时间
来源：http://ur.lnxyls.cn

================================================================================
来源：http://it.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://mc.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nc.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vk.nszjky.cn

JS:   new Date();  Date.now()
来源：http://bs.newstarts.cn

TS:   new Date();  Date.now()
来源：http://mb.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nw.lnxyls.cn

Go:   time.Now()
来源：http://om.jianghongdianzi.cn

Ruby: Time.now
来源：http://if.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gu.muxihuayi.cn

[J02] 格式化输出
来源：http://px.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ua.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ra.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xk.nszjky.cn

TS:   d.toISOString()
来源：http://dz.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lz.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rr.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dl.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eq.huanxung.cn

[J03] 字符串解析为日期
来源：http://uz.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bz.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://li.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ch.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://ng.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gm.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xg.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ec.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pa.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://oz.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cn.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ds.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ku.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ej.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vv.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://an.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://re.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bk.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://mx.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://gz.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xk.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ti.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uz.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://tl.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fc.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://nn.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yu.9csxet.cn

[J06] 计算两时间之差
来源：http://hk.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://ld.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://uy.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ss.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rl.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lv.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://dn.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://nc.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://po.jctech888.com.cn

[J07] 比较两个日期
来源：http://mb.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://vy.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dz.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dv.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vc.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xv.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cv.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://po.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://wv.lnxyls.cn

[J08] 提取年月日与星期
来源：http://sv.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wn.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pi.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xo.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ks.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pa.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sq.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tr.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yi.muxihuayi.cn

[J09] 时区处理
来源：http://pi.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ev.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mn.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://th.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qs.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sv.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ao.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hk.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sh.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://fp.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bl.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zi.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cw.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oo.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ai.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kz.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zw.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yi.nicolike.cn

================================================================================
来源：http://ed.bookmarksfly.cn

K. JSON 与序列化
来源：http://yy.yuexingan06.cn

================================================================================
来源：http://zk.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://pc.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uw.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yk.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ev.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://hd.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sn.huanxung.cn

Go:   json.Marshal(obj)
来源：http://zy.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://om.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://to.9csxet.cn

[K02] JSON 字符串转对象
来源：http://xi.huanxung.cn

Py:   json.loads(s)
来源：http://ej.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cb.9csxet.cn

JS:   JSON.parse(s)
来源：http://mi.panjiajie.cn

TS:   JSON.parse(s)
来源：http://he.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jk.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://kk.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://di.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ak.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://uf.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yt.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://is.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pv.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oe.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xe.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ms.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yn.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dy.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://sb.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ia.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mb.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ko.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yg.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bs.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dr.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gc.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wf.chemitech.net.cn

[K05] 深拷贝对象
来源：http://wi.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://db.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://zw.hahajie.cn

JS:   structuredClone(obj)
来源：http://eq.szxytkj.cn

TS:   structuredClone(obj)
来源：http://mu.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cj.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rf.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gi.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ul.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://vh.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kd.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qe.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ep.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zh.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xp.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bb.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lg.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ah.huanxung.cn

[K07] 进制转换
来源：http://zm.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ge.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nj.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pu.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ha.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cy.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wc.yuntaijiaju.cn


<!-- 参考信息 -->