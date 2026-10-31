代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://za.shxzukj.cn

[H04] 自定义异常类型
来源：http://ge.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://gd.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tu.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://yn.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://tc.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oq.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://yf.huanxung.cn

C#:   class MyException : Exception {}
来源：http://sp.shxzskj.cn

[H05] 捕获特定类型
来源：http://ab.huixiangedu.cn

Py:   except ValueError as e:
来源：http://jw.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://re.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://tp.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://jr.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://jz.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kt.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://pm.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://be.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://cn.newstarts.cn

Py:   value = d.get("k") or default
来源：http://wf.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jk.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://et.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ub.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fy.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://il.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://fp.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://tl.szxytkj.cn

[H07] 断言
来源：http://br.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://wl.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://hu.szsharing.cn

JS:   console.assert(x > 0);
来源：http://fb.hahajie.cn

TS:   console.assert(x > 0);
来源：http://qq.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://fc.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ct.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ty.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://rf.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://qs.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://as.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kw.nicolike.cn

JS:   e.message;  e.stack
来源：http://kz.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ob.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xn.bookmarksfly.cn

Go:   err.Error()
来源：http://xl.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://dm.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://al.jctech888.com.cn

[H09] 带错误码的异常
来源：http://yy.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rc.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mx.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bm.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bp.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mh.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rd.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zm.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ql.shtwfgs.cn

[H10] 资源自动释放
来源：http://dn.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kr.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://in.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kn.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ca.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bz.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://ly.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mh.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ou.muxihuayi.cn

================================================================================
来源：http://gt.muxihuayi.cn

I. 正则表达式
来源：http://cu.shtwfgs.cn

================================================================================
来源：http://wz.asd995.cn

[I01] 判断是否匹配
来源：http://xh.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ml.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ci.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ee.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://sd.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pa.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://en.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://hr.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ww.hahajie.cn

[I02] 提取所有匹配
来源：http://ky.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://ho.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ol.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rj.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://bm.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jq.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yn.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ma.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hx.haigaiapp.cn

[I03] 提取捕获分组
来源：http://qg.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kj.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iy.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ur.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hk.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sq.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gi.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mz.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kr.bookmarksfly.cn

[I04] 正则替换
来源：http://kn.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://co.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ib.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qr.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sv.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fc.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dj.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tr.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zj.521024.cn

[I05] 按正则拆分
来源：http://sk.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mw.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vs.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://un.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ur.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://wf.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yy.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dy.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vz.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hq.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rr.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kb.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pu.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qk.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ke.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ez.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vq.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wa.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://cj.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tc.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oo.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vd.9csxet.cn

TS:   /error/gim
来源：http://uq.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qp.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bc.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://ko.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sg.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://kb.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ca.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mw.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qp.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ba.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qw.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jp.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zl.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.panjiajie.cn

================================================================================
来源：http://pz.yuexingan06.cn

J. 日期与时间
来源：http://uh.huixinmuqiang.cn

================================================================================
来源：http://jb.nszjky.cn

[J01] 获取当前时间
来源：http://oe.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rd.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ek.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://xm.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://eu.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fl.nicolike.cn

Go:   time.Now()
来源：http://go.szxytkj.cn

Ruby: Time.now
来源：http://sn.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://og.521024.cn

[J02] 格式化输出
来源：http://wo.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zt.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tb.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eg.nicolike.cn

TS:   d.toISOString()
来源：http://pf.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pn.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iq.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bt.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jl.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://tl.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qs.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vb.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://wl.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://xz.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qv.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fg.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://dz.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ff.asd995.cn

[J04] 时间戳与日期互转
来源：http://hy.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rh.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yq.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rw.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ur.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pg.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qm.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rh.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kf.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://tz.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://xu.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hk.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jy.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://je.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://qp.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ge.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://ok.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://em.shxzukj.cn

[J06] 计算两时间之差
来源：http://qq.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://xv.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://wy.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rs.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bd.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ue.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://sn.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://nt.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://wq.asd995.cn

[J07] 比较两个日期
来源：http://kx.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://ra.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jj.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ef.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tg.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gl.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yd.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zy.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://qr.gzmigu.cn

[J08] 提取年月日与星期
来源：http://fl.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ew.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ki.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iy.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cy.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qs.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wi.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ur.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uq.huixinmuqiang.cn

[J09] 时区处理
来源：http://cj.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://md.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ct.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ur.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cd.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hn.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dd.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yn.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://uw.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ot.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tq.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sf.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oz.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tv.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kt.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bm.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.muxihuayi.cn

================================================================================
来源：http://ik.chemitech.net.cn

K. JSON 与序列化
来源：http://po.huixiangedu.cn

================================================================================
来源：http://co.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://um.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ib.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vg.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://bh.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://iq.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yl.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://qk.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lv.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://md.nszjky.cn

[K02] JSON 字符串转对象
来源：http://ay.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://sa.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kv.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ri.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://on.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hq.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://ei.colortex.cn

Ruby: JSON.parse(s)
来源：http://qq.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rk.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://jz.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nr.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://id.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vw.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ka.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oq.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nv.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tc.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://no.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://bh.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oq.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hp.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://az.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dc.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pi.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nw.521024.cn

[K05] 深拷贝对象
来源：http://lv.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://we.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://jn.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://jz.nszjky.cn

TS:   structuredClone(obj)
来源：http://us.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pd.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hr.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qu.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jx.521024.cn

[K06] 解析 URL 查询串
来源：http://hw.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zz.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bm.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ex.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://en.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pt.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ox.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ji.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xd.gzmigu.cn

[K07] 进制转换
来源：http://ez.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ks.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pd.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://co.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wh.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ur.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://si.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ma.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dw.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://fw.colortex.cn

Py:   pickle.dumps(obj)
来源：http://jw.huixiangedu.cn


<!-- 参考信息 -->