代发 wailian999

JS:   class MyError extends Error {}
来源：http://ek.szsharing.cn

TS:   class MyError extends Error {}
来源：http://yl.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://yd.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yp.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://lc.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://qb.muxihuayi.cn

[H05] 捕获特定类型
来源：http://no.hahajie.cn

Py:   except ValueError as e:
来源：http://yh.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mc.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://he.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qd.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wx.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xo.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://ov.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hf.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://fg.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://vc.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tx.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nr.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ow.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://de.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qd.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://vk.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://yb.jianghongdianzi.cn

[H07] 断言
来源：http://jp.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://ks.panjiajie.cn

PHP:  assert($x > 0);
来源：http://kb.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://qd.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://nl.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://pa.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vg.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://im.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://hu.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://sw.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://ml.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mj.9csxet.cn

JS:   e.message;  e.stack
来源：http://cu.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://du.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zk.huixinmuqiang.cn

Go:   err.Error()
来源：http://pr.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://uj.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://ev.shxzukj.cn

[H09] 带错误码的异常
来源：http://uh.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bs.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yj.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vc.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ff.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cg.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kl.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pc.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://au.asd995.cn

[H10] 资源自动释放
来源：http://qj.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://um.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lk.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fj.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ox.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lh.shtwfgs.cn

Go:   defer f.Close()
来源：http://ef.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ov.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zg.colortex.cn

================================================================================
来源：http://fu.shxzskj.cn

I. 正则表达式
来源：http://ho.haigaiapp.cn

================================================================================
来源：http://wd.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ll.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rm.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pv.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://kc.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://qw.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ho.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mq.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://rj.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ne.szsharing.cn

[I02] 提取所有匹配
来源：http://nd.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://qq.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ge.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tb.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://dx.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gb.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ki.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://hw.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://go.panjiajie.cn

[I03] 提取捕获分组
来源：http://qd.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bv.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ws.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://je.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sg.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zd.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bw.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lg.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://si.jctech888.com.cn

[I04] 正则替换
来源：http://fq.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mf.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iz.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ow.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nw.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://si.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vf.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ob.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pf.shxzskj.cn

[I05] 按正则拆分
来源：http://mz.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sh.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bt.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://tg.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://mj.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://td.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vc.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yc.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ab.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yf.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://um.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gg.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kv.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vl.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nq.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xt.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fv.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://wt.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yd.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ev.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lr.nicolike.cn

TS:   /error/gim
来源：http://jn.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xu.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lf.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://zq.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wy.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://nw.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oy.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ep.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://va.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yf.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jc.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wz.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fw.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yj.bookmarksfly.cn

================================================================================
来源：http://sk.newstarts.cn

J. 日期与时间
来源：http://pu.huanxung.cn

================================================================================
来源：http://bh.chemitech.net.cn

[J01] 获取当前时间
来源：http://se.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jt.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nj.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://cd.521024.cn

TS:   new Date();  Date.now()
来源：http://nk.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uv.huanxung.cn

Go:   time.Now()
来源：http://xc.bookmarksfly.cn

Ruby: Time.now
来源：http://wi.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://re.szxytkj.cn

[J02] 格式化输出
来源：http://du.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ho.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hx.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cr.panjiajie.cn

TS:   d.toISOString()
来源：http://vr.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sy.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cw.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ep.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jz.lnxyls.cn

[J03] 字符串解析为日期
来源：http://nl.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zc.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kd.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://pz.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://fz.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qw.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jw.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://hc.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pk.huanxung.cn

[J04] 时间戳与日期互转
来源：http://cn.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zb.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bv.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jm.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ok.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jb.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pk.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pn.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fr.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://oi.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://gd.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sw.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jm.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nm.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://zx.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ir.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://jy.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qy.szxytkj.cn

[J06] 计算两时间之差
来源：http://kq.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://en.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://qw.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yj.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bs.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cv.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://dt.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://jz.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://qp.shtwfgs.cn

[J07] 比较两个日期
来源：http://vc.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://yg.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rp.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ne.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nk.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jm.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ny.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ag.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ub.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://qo.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sf.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xs.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lk.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zr.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://na.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sa.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ha.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pz.bookmarksfly.cn

[J09] 时区处理
来源：http://qk.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://la.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tz.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yj.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dc.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kx.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xe.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://em.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kn.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://hg.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qx.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sb.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sp.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fu.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ln.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ey.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ex.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ql.shxzukj.cn

================================================================================
来源：http://ng.jctech888.com.cn

K. JSON 与序列化
来源：http://ll.colortex.cn

================================================================================
来源：http://ne.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://db.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fn.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zp.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://jy.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://uc.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qy.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ay.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sx.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qw.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://tv.bjjhwx.cn

Py:   json.loads(s)
来源：http://ki.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fm.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://an.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://dc.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lk.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://cp.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://eg.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xd.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bu.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yb.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://un.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xn.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ko.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rw.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vs.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hs.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oh.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://vo.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fv.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sc.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ei.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xh.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uo.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xi.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kk.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bl.yuexingan06.cn

[K05] 深拷贝对象
来源：http://su.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://xn.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://jz.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ks.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://in.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yt.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gk.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iv.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://co.asd995.cn

[K06] 解析 URL 查询串
来源：http://my.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://md.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fg.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hd.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ld.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cz.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sq.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hd.panjiajie.cn

[K07] 进制转换
来源：http://up.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hi.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ld.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dd.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pg.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ke.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gg.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xg.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gf.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://ue.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://je.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hd.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://fn.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://ec.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gd.jianghongdianzi.cn


<!-- 参考信息 -->