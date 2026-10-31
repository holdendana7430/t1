代发 wailian999

JS:   class MyError extends Error {}
来源：http://od.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://xe.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://md.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nu.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://dj.colortex.cn

C#:   class MyException : Exception {}
来源：http://kp.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://wr.huanxung.cn

Py:   except ValueError as e:
来源：http://vr.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ec.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://my.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://mu.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://lh.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://co.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://ec.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fr.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://wu.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ls.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uw.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://os.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wk.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://np.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wc.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ko.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://hi.jianghongdianzi.cn

[H07] 断言
来源：http://re.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://hq.panjiajie.cn

PHP:  assert($x > 0);
来源：http://em.9csxet.cn

JS:   console.assert(x > 0);
来源：http://ov.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://bc.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://mh.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zi.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sj.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://nm.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://sl.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://ul.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dw.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://sm.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ey.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://li.haigaiapp.cn

Go:   err.Error()
来源：http://yd.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://bu.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://pv.szsharing.cn

[H09] 带错误码的异常
来源：http://vl.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yn.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wl.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://la.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kn.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vm.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hd.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eg.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ey.shxzskj.cn

[H10] 资源自动释放
来源：http://is.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sj.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zv.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ka.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xa.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ej.hahajie.cn

Go:   defer f.Close()
来源：http://ao.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ue.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bc.chemitech.net.cn

================================================================================
来源：http://pp.huixinmuqiang.cn

I. 正则表达式
来源：http://qm.wgjwhj.cn

================================================================================
来源：http://vb.bjjhwx.cn

[I01] 判断是否匹配
来源：http://sy.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ei.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sh.9csxet.cn

JS:   /\d+/.test(s)
来源：http://dp.huanxung.cn

TS:   /\d+/.test(s)
来源：http://dh.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mt.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://vo.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iu.asd995.cn

[I02] 提取所有匹配
来源：http://cp.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://eo.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gb.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iy.521024.cn

TS:   s.match(/\d+/g)
来源：http://rm.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mt.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ei.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://ag.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gk.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sz.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vu.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xy.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qb.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vv.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jz.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fj.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kc.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bh.szsharing.cn

[I04] 正则替换
来源：http://lm.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cd.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qj.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dg.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vj.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lf.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sc.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jj.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yp.bjjhwx.cn

[I05] 按正则拆分
来源：http://gx.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sl.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ar.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://le.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://kx.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://sv.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dg.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zm.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ka.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://so.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ax.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yh.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xm.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sr.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yb.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vr.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kx.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rj.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ic.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pg.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gu.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lw.huanxung.cn

TS:   /error/gim
来源：http://cx.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rc.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fw.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://ms.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xt.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://dm.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://us.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ma.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lu.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://os.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://to.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ud.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rv.panjiajie.cn

================================================================================
来源：http://nk.yuntaijiaju.cn

J. 日期与时间
来源：http://zr.huanxung.cn

================================================================================
来源：http://vi.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://by.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wg.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ek.nicolike.cn

JS:   new Date();  Date.now()
来源：http://fx.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://za.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ol.hahajie.cn

Go:   time.Now()
来源：http://fn.asd995.cn

Ruby: Time.now
来源：http://wq.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sp.lnxyls.cn

[J02] 格式化输出
来源：http://wr.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ja.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cd.huanxung.cn

TS:   d.toISOString()
来源：http://ru.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://za.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bj.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eh.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iz.lnxyls.cn

[J03] 字符串解析为日期
来源：http://zr.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wq.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kb.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ga.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://bf.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hu.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lh.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ls.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://et.colortex.cn

[J04] 时间戳与日期互转
来源：http://dl.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rg.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ct.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sq.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kz.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yi.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vp.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dm.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xw.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://cy.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://kb.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nc.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pc.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://at.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://hp.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zs.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://hb.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://it.nszjky.cn

[J06] 计算两时间之差
来源：http://rq.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://ye.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://ak.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xl.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rc.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://py.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://fv.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://au.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://su.szxytkj.cn

[J07] 比较两个日期
来源：http://oi.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ob.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ib.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qe.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qe.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ci.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bi.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pj.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://bk.shxzukj.cn

[J08] 提取年月日与星期
来源：http://cq.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zg.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xe.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cx.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gm.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ac.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kx.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://as.yuexingan06.cn

[J09] 时区处理
来源：http://ns.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hc.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qk.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://be.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yq.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cp.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lo.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hd.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://wr.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tp.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ql.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yl.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mo.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fq.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wv.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uh.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jo.shxzskj.cn

================================================================================
来源：http://bk.nicolike.cn

K. JSON 与序列化
来源：http://io.gzmigu.cn

================================================================================
来源：http://cv.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://lc.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ez.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dm.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://mg.asd995.cn

TS:   JSON.stringify(obj)
来源：http://fb.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zp.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://tr.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lk.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ri.521024.cn

[K02] JSON 字符串转对象
来源：http://wu.panjiajie.cn

Py:   json.loads(s)
来源：http://kx.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wc.szsharing.cn

JS:   JSON.parse(s)
来源：http://af.shxzskj.cn

TS:   JSON.parse(s)
来源：http://bc.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://no.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://mh.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://ce.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vi.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://wr.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mi.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jm.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xk.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://id.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rh.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cg.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bm.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://co.asd995.cn

[K04] 读取 JSON 文件
来源：http://oa.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jr.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iu.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xf.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rn.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://av.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pc.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pe.bjjhwx.cn

[K05] 深拷贝对象
来源：http://gq.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://jl.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ad.szsharing.cn

JS:   structuredClone(obj)
来源：http://dc.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://tk.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ef.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iu.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sh.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ms.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://mr.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kw.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fg.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ou.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gw.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lj.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gv.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hy.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sq.szxytkj.cn

[K07] 进制转换
来源：http://ju.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fw.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tu.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ou.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xi.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hn.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kd.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ot.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yq.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://bo.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://mq.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rr.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://jd.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://ej.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://or.hahajie.cn


<!-- 参考信息 -->