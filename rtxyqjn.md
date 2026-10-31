代发 wailian999

TS:   throw new Error("错误信息");
来源：http://eo.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nm.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gr.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ut.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kr.bjjhwx.cn

[H04] 自定义异常类型
来源：http://fx.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://jf.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://su.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ge.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://ju.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://to.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yb.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://nl.hahajie.cn

C#:   class MyException : Exception {}
来源：http://lh.hahajie.cn

[H05] 捕获特定类型
来源：http://zo.nicolike.cn

Py:   except ValueError as e:
来源：http://tk.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hl.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ck.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://sx.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://sl.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ht.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://dj.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://un.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://ap.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://yi.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jw.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ep.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mf.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cd.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qe.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://oa.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://nw.newstarts.cn

[H07] 断言
来源：http://ww.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://yj.asd995.cn

PHP:  assert($x > 0);
来源：http://xi.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://pk.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://ke.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://dw.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lp.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ao.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://fb.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://if.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://wc.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ac.nszjky.cn

JS:   e.message;  e.stack
来源：http://fd.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lu.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xi.jctech888.com.cn

Go:   err.Error()
来源：http://xf.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://wd.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://wr.hahajie.cn

[H09] 带错误码的异常
来源：http://ke.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dl.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://om.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rh.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pr.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ma.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lr.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cu.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vc.bookmarksfly.cn

[H10] 资源自动释放
来源：http://ph.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zo.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vd.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zm.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dh.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mn.huixiangedu.cn

Go:   defer f.Close()
来源：http://ky.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tt.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ea.haigaiapp.cn

================================================================================
来源：http://jq.shxzukj.cn

I. 正则表达式
来源：http://nm.yuexingan06.cn

================================================================================
来源：http://jt.nszjky.cn

[I01] 判断是否匹配
来源：http://hx.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xe.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wm.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://kk.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://wt.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gd.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ct.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://gq.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.huixiangedu.cn

[I02] 提取所有匹配
来源：http://vi.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ly.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aw.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hq.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://wf.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gm.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bl.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://km.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xk.lnxyls.cn

[I03] 提取捕获分组
来源：http://ky.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fx.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nw.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ga.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://od.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xd.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://os.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ss.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fv.bookmarksfly.cn

[I04] 正则替换
来源：http://zi.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yw.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://by.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dr.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ai.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uy.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yb.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ku.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cx.newstarts.cn

[I05] 按正则拆分
来源：http://cb.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xo.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eb.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ng.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://se.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://bo.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ic.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bw.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lm.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iv.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xh.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jn.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ab.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vs.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qn.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ek.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uo.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vq.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://ul.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ed.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ef.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ai.lnxyls.cn

TS:   /error/gim
来源：http://fs.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cu.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rf.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ik.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mt.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://si.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vg.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gv.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://de.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aj.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fc.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vr.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://os.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ox.bjjhwx.cn

================================================================================
来源：http://sy.szxytkj.cn

J. 日期与时间
来源：http://lk.yuexingan06.cn

================================================================================
来源：http://yt.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://lq.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hd.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qn.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://vo.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://sa.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rl.bjjhwx.cn

Go:   time.Now()
来源：http://kp.9csxet.cn

Ruby: Time.now
来源：http://mk.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hd.asd995.cn

[J02] 格式化输出
来源：http://wn.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ef.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fh.521024.cn

TS:   d.toISOString()
来源：http://vk.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dk.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xg.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ca.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xe.hahajie.cn

[J03] 字符串解析为日期
来源：http://py.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sa.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uy.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://eu.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://uy.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wz.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dc.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://og.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gk.nszjky.cn

[J04] 时间戳与日期互转
来源：http://jg.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xr.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xa.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ib.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fk.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nu.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vr.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pj.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fx.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://rv.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://cm.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iw.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lq.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zr.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://gk.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://ba.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fb.chemitech.net.cn

[J06] 计算两时间之差
来源：http://xi.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://ti.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://mv.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ow.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kl.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pe.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://co.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://za.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://db.jctech888.com.cn

[J07] 比较两个日期
来源：http://wv.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://yv.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mp.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qo.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pd.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yx.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://or.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://bk.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://qg.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mj.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pp.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qb.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kr.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vq.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ka.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hc.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cs.shtwfgs.cn

[J09] 时区处理
来源：http://tf.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bs.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rv.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fp.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vl.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oo.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pj.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ij.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pc.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://du.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fh.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yx.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xd.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ix.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gc.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oh.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qg.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yf.huanxung.cn

================================================================================
来源：http://kn.9csxet.cn

K. JSON 与序列化
来源：http://vt.colortex.cn

================================================================================
来源：http://nc.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://wk.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gk.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://of.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://yw.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://hj.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://fv.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wl.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hu.521024.cn

[K02] JSON 字符串转对象
来源：http://ev.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ea.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fj.521024.cn

JS:   JSON.parse(s)
来源：http://el.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://qd.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lj.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://wq.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://cy.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ug.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://el.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pi.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hp.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bv.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bw.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rb.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://id.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ut.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oo.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://mo.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wi.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nh.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ps.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yj.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bi.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ql.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://na.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ie.shtwfgs.cn

[K05] 深拷贝对象
来源：http://jk.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://bn.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://vu.hahajie.cn

JS:   structuredClone(obj)
来源：http://rh.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://vp.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ii.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qt.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mz.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dx.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://dk.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://be.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sa.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vp.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cp.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zi.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ce.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://co.shxzskj.cn

[K07] 进制转换
来源：http://si.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ci.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yh.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gk.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gm.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xl.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://do.jianghongdianzi.cn


<!-- 参考信息 -->