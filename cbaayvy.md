代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://to.nszjky.cn

[H04] 自定义异常类型
来源：http://qd.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://sz.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jq.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://tn.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://do.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://vx.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ye.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://gm.szsharing.cn

C#:   class MyException : Exception {}
来源：http://qd.yuexingan06.cn

[H05] 捕获特定类型
来源：http://nf.nszjky.cn

Py:   except ValueError as e:
来源：http://bj.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fw.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://sy.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://uj.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://px.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kv.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://rc.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lq.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://ve.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://xz.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://co.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qo.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wq.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zf.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ds.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://hn.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://gn.bookmarksfly.cn

[H07] 断言
来源：http://wq.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://uu.nicolike.cn

PHP:  assert($x > 0);
来源：http://ks.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://ve.hahajie.cn

TS:   console.assert(x > 0);
来源：http://rr.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://ze.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vf.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pd.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://va.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ai.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://ie.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://as.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://bt.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sm.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bo.newstarts.cn

Go:   err.Error()
来源：http://jo.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://qo.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://id.nicolike.cn

[H09] 带错误码的异常
来源：http://yq.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zb.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sc.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vh.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ru.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xv.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cv.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ys.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qh.shxzukj.cn

[H10] 资源自动释放
来源：http://ep.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gr.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eh.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iy.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jx.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iz.shxzskj.cn

Go:   defer f.Close()
来源：http://vy.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gg.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qu.colortex.cn

================================================================================
来源：http://is.asd995.cn

I. 正则表达式
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://aj.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://px.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oh.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ku.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://vm.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://jf.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sd.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zp.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://wh.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jg.colortex.cn

[I02] 提取所有匹配
来源：http://sa.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://zq.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sd.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ze.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://qq.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qg.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fw.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://lb.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ks.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ih.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pe.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fr.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qj.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jb.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vr.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mf.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bp.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xu.521024.cn

[I04] 正则替换
来源：http://dk.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zp.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xf.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gy.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tg.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pn.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wb.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mm.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jl.shtwfgs.cn

[I05] 按正则拆分
来源：http://ar.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://of.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kr.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://vl.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://pe.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://ul.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vz.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tl.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vj.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hf.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cv.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gk.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mn.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ex.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tq.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pd.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xi.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rd.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://yi.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tp.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vw.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jc.jianghongdianzi.cn

TS:   /error/gim
来源：http://ke.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ph.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xf.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://qs.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ml.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://sr.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vu.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ft.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ej.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fp.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vz.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zl.shxzukj.cn

================================================================================
来源：http://yb.yuntaijiaju.cn

J. 日期与时间
来源：http://vg.nicolike.cn

================================================================================
来源：http://eu.bjjhwx.cn

[J01] 获取当前时间
来源：http://ag.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yq.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ui.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://hh.huanxung.cn

TS:   new Date();  Date.now()
来源：http://qc.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hl.9csxet.cn

Go:   time.Now()
来源：http://rt.lnxyls.cn

Ruby: Time.now
来源：http://id.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zo.shtwfgs.cn

[J02] 格式化输出
来源：http://gr.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cx.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://js.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vs.wgjwhj.cn

TS:   d.toISOString()
来源：http://sp.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ea.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://om.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ss.hnjuh.cn

[J03] 字符串解析为日期
来源：http://lq.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vr.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kj.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://pf.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://of.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ti.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lh.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://xw.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yn.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://kp.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ab.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qd.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iy.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zk.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ap.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ru.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mw.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hj.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://ow.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://th.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nf.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zh.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wc.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ed.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kt.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://st.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cl.chemitech.net.cn

[J06] 计算两时间之差
来源：http://et.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://ud.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://km.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rs.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kd.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ae.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://kj.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://gt.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://qn.szxytkj.cn

[J07] 比较两个日期
来源：http://if.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ev.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kd.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iw.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://st.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vu.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ay.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qn.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://fu.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://tv.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kj.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sr.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nw.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://te.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lz.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ih.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mu.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mu.jianghongdianzi.cn

[J09] 时区处理
来源：http://pe.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qh.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://if.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://do.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sy.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yi.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mb.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gr.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xu.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://hg.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hg.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ks.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mz.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://je.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xw.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rn.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wb.asd995.cn

================================================================================
来源：http://dh.shxzukj.cn

K. JSON 与序列化
来源：http://fs.haigaiapp.cn

================================================================================
来源：http://xh.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://ug.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eq.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://au.colortex.cn

JS:   JSON.stringify(obj)
来源：http://zq.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://gq.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ub.nszjky.cn

Go:   json.Marshal(obj)
来源：http://gw.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xq.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dw.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://an.bookmarksfly.cn

Py:   json.loads(s)
来源：http://cx.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gy.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://gk.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://og.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mq.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://gd.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://zi.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nn.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://fp.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wt.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iy.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ko.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ji.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pg.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pf.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hg.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qx.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://tk.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cu.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tv.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wf.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bq.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qz.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://st.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ao.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rm.jctech888.com.cn

[K05] 深拷贝对象
来源：http://mm.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://pg.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://da.newstarts.cn

JS:   structuredClone(obj)
来源：http://rn.asd995.cn

TS:   structuredClone(obj)
来源：http://gl.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lo.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pn.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oc.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xv.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://qn.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gb.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dx.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://om.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qz.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fy.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://su.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jx.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pd.nszjky.cn

[K07] 进制转换
来源：http://el.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bc.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wp.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hq.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jq.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oe.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bg.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jv.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kr.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://tr.521024.cn

Py:   pickle.dumps(obj)
来源：http://ek.nszjky.cn


<!-- 参考信息 -->