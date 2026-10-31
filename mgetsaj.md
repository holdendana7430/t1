代发 wailian999

JS:   class MyError extends Error {}
来源：http://ec.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://je.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://eo.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ch.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://is.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://ss.nszjky.cn

[H05] 捕获特定类型
来源：http://yd.huanxung.cn

Py:   except ValueError as e:
来源：http://qe.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zp.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://il.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://nv.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://wf.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ta.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://wt.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ai.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://bz.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://gb.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vc.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ya.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mi.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yi.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bb.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://at.521024.cn

C#:   obj?.A?.B ?? default
来源：http://yk.szsharing.cn

[H07] 断言
来源：http://pk.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://te.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://so.newstarts.cn

JS:   console.assert(x > 0);
来源：http://qy.nszjky.cn

TS:   console.assert(x > 0);
来源：http://qv.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://ur.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vg.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ce.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://uy.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://jl.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://mi.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ta.colortex.cn

JS:   e.message;  e.stack
来源：http://jn.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iq.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sk.colortex.cn

Go:   err.Error()
来源：http://sd.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://ml.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://vf.lnxyls.cn

[H09] 带错误码的异常
来源：http://ye.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ug.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ux.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ux.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vg.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wv.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ns.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dn.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ul.nicolike.cn

[H10] 资源自动释放
来源：http://ub.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iq.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qj.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dd.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vg.bookmarksfly.cn

Go:   defer f.Close()
来源：http://qw.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://at.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zl.huixiangedu.cn

================================================================================
来源：http://zt.huixiangedu.cn

I. 正则表达式
来源：http://dx.hnjuh.cn

================================================================================
来源：http://jj.jctech888.com.cn

[I01] 判断是否匹配
来源：http://mk.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ss.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nx.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://pd.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://st.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tc.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kg.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://ha.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://br.bjjhwx.cn

[I02] 提取所有匹配
来源：http://uk.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://xt.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pg.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ko.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://zz.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vi.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vv.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://tm.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fm.colortex.cn

[I03] 提取捕获分组
来源：http://da.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xw.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://es.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://if.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qm.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ta.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://na.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tz.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xr.szsharing.cn

[I04] 正则替换
来源：http://om.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rv.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zh.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kt.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iu.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bl.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aw.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vw.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://za.colortex.cn

[I05] 按正则拆分
来源：http://rp.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xm.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://sb.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://uk.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ox.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://da.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iy.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bm.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oo.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gf.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tj.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jl.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cw.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mj.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mg.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sj.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hy.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://lt.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tu.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dm.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pt.shxzskj.cn

TS:   /error/gim
来源：http://hv.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dk.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ff.colortex.cn

Ruby: s.scan(/error/i)
来源：http://qx.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zm.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://bk.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gr.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ev.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wb.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fy.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tq.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://go.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://os.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wg.bjjhwx.cn

================================================================================
来源：http://vc.huixiangedu.cn

J. 日期与时间
来源：http://wb.huanxung.cn

================================================================================
来源：http://mw.shtwfgs.cn

[J01] 获取当前时间
来源：http://ah.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://it.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sw.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://vw.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://zp.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yg.gzmigu.cn

Go:   time.Now()
来源：http://if.wgjwhj.cn

Ruby: Time.now
来源：http://er.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ml.colortex.cn

[J02] 格式化输出
来源：http://ga.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://to.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gt.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mv.shxzskj.cn

TS:   d.toISOString()
来源：http://wp.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vm.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zp.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jn.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uh.asd995.cn

[J03] 字符串解析为日期
来源：http://to.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mo.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://om.asd995.cn

JS:   new Date("2024-01-02")
来源：http://lr.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://nc.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ln.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pt.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://qc.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jt.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://bz.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ls.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ss.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ky.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wb.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mf.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lg.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fx.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ae.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://oz.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ev.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cx.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://og.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fk.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ue.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rm.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://nd.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xv.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://yg.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://lp.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://bt.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://to.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xh.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eu.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://bw.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://ja.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://xj.szxytkj.cn

[J07] 比较两个日期
来源：http://cu.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://at.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zl.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ip.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sd.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fw.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mp.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nn.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://go.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://lm.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fd.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ns.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fk.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ym.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ez.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vd.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fc.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ly.lnxyls.cn

[J09] 时区处理
来源：http://yk.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gm.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ex.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ru.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wk.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ep.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nu.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cc.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cs.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://ty.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://su.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xw.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://za.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nl.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zr.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pp.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://um.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lc.huixiangedu.cn

================================================================================
来源：http://ta.shxzukj.cn

K. JSON 与序列化
来源：http://ci.nszjky.cn

================================================================================
来源：http://sb.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://ru.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lp.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zu.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://hd.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://oo.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sz.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://vw.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://it.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://de.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://lk.hahajie.cn

Py:   json.loads(s)
来源：http://cq.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mu.521024.cn

JS:   JSON.parse(s)
来源：http://wz.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://ar.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tc.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://yz.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ud.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qs.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://cx.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://za.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wb.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gc.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yg.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://le.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fe.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yn.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dm.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://fs.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xz.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fo.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lc.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sf.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pg.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bm.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hl.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ml.shxzskj.cn

[K05] 深拷贝对象
来源：http://qi.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://vs.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://yw.9csxet.cn

JS:   structuredClone(obj)
来源：http://ib.521024.cn

TS:   structuredClone(obj)
来源：http://gt.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qe.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sk.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kj.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fb.huanxung.cn

[K06] 解析 URL 查询串
来源：http://ej.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qk.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qc.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://il.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rz.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sc.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jy.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yb.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cj.shtwfgs.cn

[K07] 进制转换
来源：http://ue.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bx.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://li.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yw.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ea.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bd.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pk.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dq.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lz.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://ql.asd995.cn

Py:   pickle.dumps(obj)
来源：http://bj.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://js.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://nw.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ge.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pn.hnjuh.cn


<!-- 参考信息 -->