代发 wailian999

JS:   class MyError extends Error {}
来源：http://xg.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://xv.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://rt.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jo.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://yp.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://js.huanxung.cn

[H05] 捕获特定类型
来源：http://fh.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://cw.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://if.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://wh.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://lr.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://vp.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ps.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://bu.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xx.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://cv.huanxung.cn

Py:   value = d.get("k") or default
来源：http://tp.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ra.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xd.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jb.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qc.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ml.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://yh.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://ua.yuexingan06.cn

[H07] 断言
来源：http://ll.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://tl.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ub.nszjky.cn

JS:   console.assert(x > 0);
来源：http://bg.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://kn.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://kz.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kk.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://az.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://yu.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://nr.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://hd.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kl.panjiajie.cn

JS:   e.message;  e.stack
来源：http://zw.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gg.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eu.bjjhwx.cn

Go:   err.Error()
来源：http://oj.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://qo.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://rm.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://up.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fi.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pf.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bi.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tb.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ha.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pd.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ip.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vr.yuexingan06.cn

[H10] 资源自动释放
来源：http://vx.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://en.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gf.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zr.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ee.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zf.gzmigu.cn

Go:   defer f.Close()
来源：http://hp.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eq.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ld.bjjhwx.cn

================================================================================
来源：http://kz.nicolike.cn

I. 正则表达式
来源：http://jy.szxytkj.cn

================================================================================
来源：http://fz.hahajie.cn

[I01] 判断是否匹配
来源：http://bk.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xd.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nk.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://pq.newstarts.cn

TS:   /\d+/.test(s)
来源：http://pu.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hf.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ld.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://lx.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ew.shtwfgs.cn

[I02] 提取所有匹配
来源：http://xy.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://iz.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pz.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tu.asd995.cn

TS:   s.match(/\d+/g)
来源：http://xl.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yc.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ij.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://jw.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://se.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ks.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mk.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fj.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cz.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ue.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ig.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yg.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ga.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yi.lnxyls.cn

[I04] 正则替换
来源：http://us.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ic.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://re.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qy.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nr.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xq.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://um.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wk.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nb.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://sg.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://us.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tp.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ge.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://mv.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vw.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sl.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vq.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ai.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tg.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nd.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fv.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://is.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dt.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rm.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uy.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://ae.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cm.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://up.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ap.lnxyls.cn

TS:   /error/gim
来源：http://ok.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bt.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jq.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://xr.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://my.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://uw.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ko.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vg.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bg.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mz.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mi.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mc.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lf.szsharing.cn

================================================================================
来源：http://xf.panjiajie.cn

J. 日期与时间
来源：http://lr.jctech888.com.cn

================================================================================
来源：http://xq.yuexingan06.cn

[J01] 获取当前时间
来源：http://wc.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zp.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mw.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://tt.szsharing.cn

TS:   new Date();  Date.now()
来源：http://ip.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vb.shtwfgs.cn

Go:   time.Now()
来源：http://jv.newstarts.cn

Ruby: Time.now
来源：http://gn.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tt.521024.cn

[J02] 格式化输出
来源：http://iu.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gg.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gh.bjjhwx.cn

TS:   d.toISOString()
来源：http://oo.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zo.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nt.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ow.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://rs.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ae.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yl.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://dy.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://as.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xp.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dr.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://sv.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kr.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ab.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dh.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ql.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vg.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pr.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://td.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qm.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jn.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sq.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://zx.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://vc.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rp.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://if.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xu.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://zg.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bk.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://op.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gv.muxihuayi.cn

[J06] 计算两时间之差
来源：http://sg.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://bk.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://ot.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wi.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fv.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yn.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://by.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://uk.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ab.huixiangedu.cn

[J07] 比较两个日期
来源：http://fg.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://pv.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sj.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yp.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fg.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://su.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qk.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dc.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://yi.asd995.cn

[J08] 提取年月日与星期
来源：http://xn.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zj.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yv.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lk.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://do.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tz.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ja.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dq.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ta.yuexingan06.cn

[J09] 时区处理
来源：http://nd.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://in.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eo.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xw.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sr.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gl.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iy.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rq.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://hx.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xb.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fx.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bd.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xd.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://in.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dn.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ws.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ck.muxihuayi.cn

================================================================================
来源：http://if.shxzskj.cn

K. JSON 与序列化
来源：http://yj.nszjky.cn

================================================================================
来源：http://of.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ul.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ki.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qp.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://hz.asd995.cn

TS:   JSON.stringify(obj)
来源：http://iu.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mv.nicolike.cn

Go:   json.Marshal(obj)
来源：http://cu.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ad.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ub.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://cx.jctech888.com.cn

Py:   json.loads(s)
来源：http://ft.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://et.panjiajie.cn

JS:   JSON.parse(s)
来源：http://hl.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://pv.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cp.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ux.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://bo.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qp.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://uq.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fm.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uc.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yl.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vt.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yn.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://of.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fw.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vw.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://th.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://no.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bg.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pc.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fz.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ug.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cv.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kb.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lz.shxzukj.cn

[K05] 深拷贝对象
来源：http://xm.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://pd.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://wm.521024.cn

JS:   structuredClone(obj)
来源：http://te.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://fv.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cy.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gn.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nk.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aj.szsharing.cn

[K06] 解析 URL 查询串
来源：http://hx.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hw.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bp.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tj.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://re.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fe.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://up.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gf.asd995.cn

[K07] 进制转换
来源：http://sr.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xe.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iv.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ls.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fb.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bh.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ba.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ip.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qd.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://xl.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://zw.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jf.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://rj.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://mt.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iy.bookmarksfly.cn


<!-- 参考信息 -->