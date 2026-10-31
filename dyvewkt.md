代发 wailian999

JS:   class MyError extends Error {}
来源：http://ha.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://as.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://zh.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ud.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://qu.colortex.cn

C#:   class MyException : Exception {}
来源：http://zq.jctech888.com.cn

[H05] 捕获特定类型
来源：http://hx.asd995.cn

Py:   except ValueError as e:
来源：http://ws.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ne.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://kx.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://cp.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://iu.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wp.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://dk.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ef.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://wj.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://vx.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://he.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ux.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wf.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ae.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lc.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://mn.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://qn.yuntaijiaju.cn

[H07] 断言
来源：http://pi.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://qk.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://fi.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://qv.huanxung.cn

TS:   console.assert(x > 0);
来源：http://bu.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://wz.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eb.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sc.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://yc.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://zl.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://sk.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yt.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://sk.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xm.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pp.newstarts.cn

Go:   err.Error()
来源：http://mu.521024.cn

Ruby: e.message;  e.backtrace
来源：http://cs.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://nb.521024.cn

[H09] 带错误码的异常
来源：http://om.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kv.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ws.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vb.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dv.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bu.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mj.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qb.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xe.bjjhwx.cn

[H10] 资源自动释放
来源：http://jl.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bc.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ag.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wt.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rr.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yq.shtwfgs.cn

Go:   defer f.Close()
来源：http://dq.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dn.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uz.jianghongdianzi.cn

================================================================================
来源：http://vl.colortex.cn

I. 正则表达式
来源：http://kh.nszjky.cn

================================================================================
来源：http://ud.gzmigu.cn

[I01] 判断是否匹配
来源：http://hx.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lo.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ew.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://fr.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://hz.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wf.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://el.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://is.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yv.huanxung.cn

[I02] 提取所有匹配
来源：http://mw.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://gw.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wu.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wi.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://zz.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wj.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sg.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ko.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://md.huanxung.cn

[I03] 提取捕获分组
来源：http://et.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nc.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eo.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wr.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ar.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bu.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ra.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qc.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qp.gzmigu.cn

[I04] 正则替换
来源：http://aa.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iq.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yh.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://km.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ul.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jv.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bu.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tj.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://me.bookmarksfly.cn

[I05] 按正则拆分
来源：http://lc.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://an.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kc.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://eu.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://we.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://nf.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gt.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rh.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rv.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mn.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vm.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yq.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gs.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://il.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iv.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nu.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ha.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bz.521024.cn

[I07] 忽略大小写与多行模式
来源：http://yt.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iy.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vi.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fj.chemitech.net.cn

TS:   /error/gim
来源：http://eb.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ok.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ci.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://sn.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uy.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ae.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zj.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://se.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mw.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pi.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gk.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sj.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ip.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yu.chemitech.net.cn

================================================================================
来源：http://lf.huixiangedu.cn

J. 日期与时间
来源：http://uv.521024.cn

================================================================================
来源：http://ej.lnxyls.cn

[J01] 获取当前时间
来源：http://tk.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ou.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xl.521024.cn

JS:   new Date();  Date.now()
来源：http://pf.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ye.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eq.huixiangedu.cn

Go:   time.Now()
来源：http://tz.szxytkj.cn

Ruby: Time.now
来源：http://wh.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ql.jianghongdianzi.cn

[J02] 格式化输出
来源：http://wd.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://to.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kt.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zy.jctech888.com.cn

TS:   d.toISOString()
来源：http://um.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pb.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rx.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vv.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ac.9csxet.cn

[J03] 字符串解析为日期
来源：http://gs.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pb.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uw.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ga.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ey.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ax.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yg.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://vf.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zi.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://ux.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yt.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kd.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tw.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xc.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zw.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xj.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vt.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nj.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://lg.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://dd.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yc.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xi.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ha.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://lh.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tn.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://vc.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mq.521024.cn

[J06] 计算两时间之差
来源：http://rc.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ce.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://wg.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ut.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yv.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zj.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://sn.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://rl.521024.cn

C#:   (end - start).TotalSeconds
来源：http://ky.newstarts.cn

[J07] 比较两个日期
来源：http://oe.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://my.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://la.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xg.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oa.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fc.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://js.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gd.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://ij.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://mi.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xd.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gf.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ff.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qb.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://od.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yv.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zl.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nd.wgjwhj.cn

[J09] 时区处理
来源：http://qa.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pn.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ib.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://er.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pm.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ec.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lw.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fy.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://kw.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ep.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rb.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eg.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qr.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fg.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rv.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sx.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aq.colortex.cn

================================================================================
来源：http://uw.huixiangedu.cn

K. JSON 与序列化
来源：http://qt.lnxyls.cn

================================================================================
来源：http://vw.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://hx.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oq.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uv.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://wg.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://lh.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://va.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://sr.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://du.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nn.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://wi.shxzukj.cn

Py:   json.loads(s)
来源：http://mh.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dg.asd995.cn

JS:   JSON.parse(s)
来源：http://hn.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://vi.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cm.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mz.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://kj.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://om.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://rw.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tw.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ih.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ko.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tj.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sr.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oa.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qw.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ab.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://dm.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lc.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tu.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ew.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ih.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xd.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uc.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qn.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qy.nicolike.cn

[K05] 深拷贝对象
来源：http://eo.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://nv.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ip.huanxung.cn

JS:   structuredClone(obj)
来源：http://na.szxytkj.cn

TS:   structuredClone(obj)
来源：http://mr.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ry.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zm.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tf.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nf.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ax.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pf.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nh.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bu.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rr.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sj.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://my.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yx.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ps.lnxyls.cn

[K07] 进制转换
来源：http://ul.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://st.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jv.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xv.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://em.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ws.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zf.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ja.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fy.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://hi.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://fv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ju.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gq.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://lj.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vw.chemitech.net.cn


<!-- 参考信息 -->