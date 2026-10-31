代发 wailian999

JS:   class MyError extends Error {}
来源：http://el.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://my.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://dg.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ie.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://mx.nszjky.cn

C#:   class MyException : Exception {}
来源：http://qs.huixiangedu.cn

[H05] 捕获特定类型
来源：http://jb.521024.cn

Py:   except ValueError as e:
来源：http://fs.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://co.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://zv.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://yy.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://tp.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bv.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://js.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://of.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://fg.huanxung.cn

Py:   value = d.get("k") or default
来源：http://is.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yj.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hw.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bw.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fx.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dc.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://sl.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://je.huixiangedu.cn

[H07] 断言
来源：http://as.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://wp.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://nf.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://xf.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://kc.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://yv.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rn.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rd.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://jx.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://jx.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://oq.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://px.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://zx.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ts.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wi.gzmigu.cn

Go:   err.Error()
来源：http://um.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://ts.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://bq.9csxet.cn

[H09] 带错误码的异常
来源：http://kp.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ex.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gv.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gq.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zk.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rc.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pn.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://je.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qn.hnjuh.cn

[H10] 资源自动释放
来源：http://vq.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lg.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lf.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ry.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ij.wgjwhj.cn

Go:   defer f.Close()
来源：http://fk.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tk.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zv.9csxet.cn

================================================================================
来源：http://ge.bookmarksfly.cn

I. 正则表达式
来源：http://mw.huanxung.cn

================================================================================
来源：http://vh.nszjky.cn

[I01] 判断是否匹配
来源：http://ps.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hn.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wi.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://de.521024.cn

TS:   /\d+/.test(s)
来源：http://uy.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://co.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vt.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://mc.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://az.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://xq.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://nb.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oc.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xb.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://lw.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pd.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ri.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ld.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://es.huixiangedu.cn

[I03] 提取捕获分组
来源：http://yw.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pg.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hl.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tg.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wb.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yw.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rm.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kx.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yw.521024.cn

[I04] 正则替换
来源：http://yb.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lm.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ob.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mb.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://od.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ka.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bg.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bt.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://op.hnjuh.cn

[I05] 按正则拆分
来源：http://df.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qn.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jx.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://io.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://rs.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://to.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tp.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jx.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ph.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qp.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jk.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://er.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ec.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qh.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ob.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tg.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uu.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ld.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ub.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pt.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pl.nszjky.cn

TS:   /error/gim
来源：http://ey.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fj.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wl.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://pw.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jy.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://bt.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ix.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xm.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bp.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yv.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uy.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dv.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uu.haigaiapp.cn

================================================================================
来源：http://lk.lnxyls.cn

J. 日期与时间
来源：http://fi.huixinmuqiang.cn

================================================================================
来源：http://sn.asd995.cn

[J01] 获取当前时间
来源：http://ii.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zm.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xf.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://vr.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://pf.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fj.yuntaijiaju.cn

Go:   time.Now()
来源：http://xk.newstarts.cn

Ruby: Time.now
来源：http://oq.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xi.hahajie.cn

[J02] 格式化输出
来源：http://li.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vq.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://am.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xk.wgjwhj.cn

TS:   d.toISOString()
来源：http://lr.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kg.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ke.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qd.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://va.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://rv.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ib.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mk.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://dw.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://ls.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cy.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ma.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://nm.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yj.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://lj.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xd.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gw.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://np.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nr.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jl.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lv.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jl.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xg.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://qs.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://qw.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ne.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uv.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yy.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://nq.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nm.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://lh.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kk.wgjwhj.cn

[J06] 计算两时间之差
来源：http://qo.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://dr.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://lq.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zm.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sy.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://at.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://mg.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://sn.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://rn.asd995.cn

[J07] 比较两个日期
来源：http://tp.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://nm.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yx.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aq.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ny.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lr.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fk.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ly.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://yu.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://lf.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://us.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bk.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qj.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rn.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lh.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jd.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sl.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qe.wgjwhj.cn

[J09] 时区处理
来源：http://xg.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xs.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rm.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aj.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ng.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yy.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jo.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mq.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oa.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://jl.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://in.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mm.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://as.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yh.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pi.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tz.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tx.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iw.chemitech.net.cn

================================================================================
来源：http://px.haigaiapp.cn

K. JSON 与序列化
来源：http://yk.yuntaijiaju.cn

================================================================================
来源：http://xr.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://wk.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://se.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gc.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://sz.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://gz.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bn.521024.cn

Go:   json.Marshal(obj)
来源：http://tz.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bw.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fx.9csxet.cn

[K02] JSON 字符串转对象
来源：http://zm.wgjwhj.cn

Py:   json.loads(s)
来源：http://or.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sn.gzmigu.cn

JS:   JSON.parse(s)
来源：http://nk.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://zl.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ps.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://fu.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://uu.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fi.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://uh.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ur.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dp.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sv.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tq.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://as.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ex.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qf.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nb.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://hk.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ec.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://un.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eq.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ze.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ye.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nt.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://px.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ou.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ha.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://vo.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://cu.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://rp.hahajie.cn

TS:   structuredClone(obj)
来源：http://ke.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tx.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zm.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oy.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pb.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://iz.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qw.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pm.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xf.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vq.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iz.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yz.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ck.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mq.hnjuh.cn

[K07] 进制转换
来源：http://va.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kt.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pc.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ti.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yi.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zt.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nx.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nx.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ah.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://ue.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://vq.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hg.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://sx.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://uy.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wa.huanxung.cn


<!-- 参考信息 -->