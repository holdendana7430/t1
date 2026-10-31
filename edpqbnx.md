代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://pg.nicolike.cn

[H04] 自定义异常类型
来源：http://ud.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://vu.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cc.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ga.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://lg.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://dc.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://br.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://zn.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://kf.asd995.cn

[H05] 捕获特定类型
来源：http://ln.521024.cn

Py:   except ValueError as e:
来源：http://ww.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fi.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://cz.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://fu.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://iy.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ao.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://xl.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lb.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://up.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://yn.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wy.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sm.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rt.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ia.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ih.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://uh.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://xu.jctech888.com.cn

[H07] 断言
来源：http://tt.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://iw.panjiajie.cn

PHP:  assert($x > 0);
来源：http://yo.hahajie.cn

JS:   console.assert(x > 0);
来源：http://ia.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://ze.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://nj.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gg.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://ri.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://ex.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://rj.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ka.gzmigu.cn

JS:   e.message;  e.stack
来源：http://kn.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ck.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ud.lnxyls.cn

Go:   err.Error()
来源：http://ut.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ww.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://wt.muxihuayi.cn

[H09] 带错误码的异常
来源：http://ul.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oh.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mc.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ye.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rr.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://at.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xe.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ju.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kf.521024.cn

[H10] 资源自动释放
来源：http://od.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bu.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vq.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ku.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ps.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qw.muxihuayi.cn

Go:   defer f.Close()
来源：http://oh.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ia.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uc.chemitech.net.cn

================================================================================
来源：http://mt.bjjhwx.cn

I. 正则表达式
来源：http://bg.shtwfgs.cn

================================================================================
来源：http://kb.shxzukj.cn

[I01] 判断是否匹配
来源：http://kc.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kc.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ax.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://gy.newstarts.cn

TS:   /\d+/.test(s)
来源：http://ug.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yp.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gg.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://nz.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wd.shxzukj.cn

[I02] 提取所有匹配
来源：http://bh.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://za.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ay.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wu.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://ux.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mq.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ul.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://tq.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lg.muxihuayi.cn

[I03] 提取捕获分组
来源：http://tj.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ba.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://va.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pi.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ru.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uk.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ub.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cj.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ev.szsharing.cn

[I04] 正则替换
来源：http://qg.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rs.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zu.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xf.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sd.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mz.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uo.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lk.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nv.bjjhwx.cn

[I05] 按正则拆分
来源：http://vc.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kz.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qk.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://wq.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://lg.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://ew.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zu.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cv.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pe.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fp.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cj.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ez.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ol.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sc.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jj.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vq.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wp.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bx.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://xb.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://od.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://et.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zi.haigaiapp.cn

TS:   /error/gim
来源：http://ks.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dn.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sp.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://jl.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rp.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://vt.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tf.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uo.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gy.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hm.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ne.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ft.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bw.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hd.huixinmuqiang.cn

================================================================================
来源：http://tr.huixiangedu.cn

J. 日期与时间
来源：http://jz.lnxyls.cn

================================================================================
来源：http://ou.haigaiapp.cn

[J01] 获取当前时间
来源：http://gt.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zs.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://we.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://um.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://qi.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tl.szxytkj.cn

Go:   time.Now()
来源：http://vh.newstarts.cn

Ruby: Time.now
来源：http://yc.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ht.jctech888.com.cn

[J02] 格式化输出
来源：http://bj.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yc.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mw.chemitech.net.cn

TS:   d.toISOString()
来源：http://dl.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qu.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sn.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nh.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tp.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://sx.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bu.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nd.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://lm.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ty.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kb.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fu.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://jq.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rw.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://zk.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fi.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uj.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dt.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qr.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kf.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jz.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qs.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oz.521024.cn

[J05] 时间加减（加 7 天）
来源：http://da.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ys.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iy.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ez.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://vs.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fk.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://zd.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qq.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://xf.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://da.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://ur.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dp.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bz.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://sb.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://ll.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ss.newstarts.cn

[J07] 比较两个日期
来源：http://mr.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://my.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://et.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xh.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://au.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dy.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ow.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ba.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://cx.shxzskj.cn

[J08] 提取年月日与星期
来源：http://aw.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://if.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zl.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tj.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://db.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://us.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jf.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oi.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rp.hahajie.cn

[J09] 时区处理
来源：http://vy.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bc.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lk.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ql.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xg.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bn.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ul.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ol.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ml.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://pd.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gm.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nr.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nv.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ps.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dn.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://we.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dp.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pc.yuexingan06.cn

================================================================================
来源：http://tr.szsharing.cn

K. JSON 与序列化
来源：http://he.nicolike.cn

================================================================================
来源：http://ef.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://zw.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mz.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ke.colortex.cn

JS:   JSON.stringify(obj)
来源：http://fo.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://iq.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pb.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://wx.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nt.newstarts.cn

[K02] JSON 字符串转对象
来源：http://rp.colortex.cn

Py:   json.loads(s)
来源：http://ha.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kc.shxzskj.cn

JS:   JSON.parse(s)
来源：http://cg.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://yp.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bd.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://kb.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://hy.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qu.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://am.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lk.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rh.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gb.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gn.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dl.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vd.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tp.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sf.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://tv.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yu.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://da.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nh.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xb.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aa.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iy.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://to.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vm.hahajie.cn

[K05] 深拷贝对象
来源：http://bc.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://kz.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://vh.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ls.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://it.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sx.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bd.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kz.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ex.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://rh.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dz.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://am.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bz.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jq.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hu.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mp.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ds.jctech888.com.cn

[K07] 进制转换
来源：http://vf.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ur.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oi.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://em.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hh.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xl.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oh.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gw.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://um.asd995.cn

Py:   pickle.dumps(obj)
来源：http://jc.huixinmuqiang.cn


<!-- 参考信息 -->