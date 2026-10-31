代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://wa.wgjwhj.cn

[H04] 自定义异常类型
来源：http://pr.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://af.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nh.nszjky.cn

JS:   class MyError extends Error {}
来源：http://tg.521024.cn

TS:   class MyError extends Error {}
来源：http://zl.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://fz.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tq.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://jb.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://wg.9csxet.cn

[H05] 捕获特定类型
来源：http://fi.shxzukj.cn

Py:   except ValueError as e:
来源：http://ol.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bm.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://io.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://ws.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://yz.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lk.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://xw.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pn.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://kp.521024.cn

Py:   value = d.get("k") or default
来源：http://qm.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xu.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xg.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ak.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zq.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jc.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://po.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://mj.hnjuh.cn

[H07] 断言
来源：http://uq.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://ec.shxzskj.cn

PHP:  assert($x > 0);
来源：http://cc.asd995.cn

JS:   console.assert(x > 0);
来源：http://ww.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://mf.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://zz.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ao.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qx.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://pa.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://an.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://ba.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mo.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://al.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jc.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ru.panjiajie.cn

Go:   err.Error()
来源：http://ho.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://bk.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://oz.lnxyls.cn

[H09] 带错误码的异常
来源：http://fl.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hc.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iu.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lr.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mq.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qj.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vk.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bf.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cs.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://wh.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yi.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://co.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vr.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ki.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zz.asd995.cn

Go:   defer f.Close()
来源：http://mz.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wr.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ah.nszjky.cn

================================================================================
来源：http://ly.521024.cn

I. 正则表达式
来源：http://qp.panjiajie.cn

================================================================================
来源：http://pm.nicolike.cn

[I01] 判断是否匹配
来源：http://ox.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fp.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eo.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ca.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ja.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fv.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wq.521024.cn

Ruby: s.match?(/\d+/)
来源：http://nd.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wn.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://lh.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://mf.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sf.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qq.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://bg.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rm.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ce.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://lw.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ox.521024.cn

[I03] 提取捕获分组
来源：http://rd.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://us.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ev.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://re.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lp.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wk.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jh.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bl.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wj.wgjwhj.cn

[I04] 正则替换
来源：http://cg.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ah.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bt.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uo.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hn.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://st.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dn.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://op.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cu.shxzskj.cn

[I05] 按正则拆分
来源：http://bx.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vm.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ah.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://hn.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://iv.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://hm.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pc.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ix.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://av.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iy.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yu.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xo.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xa.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iv.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pt.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ul.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ya.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://el.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://dm.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cf.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pn.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vf.szxytkj.cn

TS:   /error/gim
来源：http://dj.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fx.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wc.colortex.cn

Ruby: s.scan(/error/i)
来源：http://cb.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://su.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ca.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lb.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ce.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zk.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gs.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qt.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://up.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xz.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fr.huixiangedu.cn

================================================================================
来源：http://gs.newstarts.cn

J. 日期与时间
来源：http://ay.huixinmuqiang.cn

================================================================================
来源：http://tu.szxytkj.cn

[J01] 获取当前时间
来源：http://jw.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://es.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ml.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://qf.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://pz.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kv.yuntaijiaju.cn

Go:   time.Now()
来源：http://um.huixinmuqiang.cn

Ruby: Time.now
来源：http://br.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rl.szsharing.cn

[J02] 格式化输出
来源：http://dk.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ni.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ri.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qj.jctech888.com.cn

TS:   d.toISOString()
来源：http://dn.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sa.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oq.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gq.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xd.newstarts.cn

[J03] 字符串解析为日期
来源：http://ct.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ds.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cm.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://tu.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://fj.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://el.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wx.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://bz.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qf.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://me.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zp.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ik.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ul.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pg.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://is.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ds.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://er.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ym.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://dv.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://fp.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kf.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zy.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://td.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lt.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://hj.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dk.szxytkj.cn

[J06] 计算两时间之差
来源：http://rj.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://er.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://ix.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kn.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yt.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://en.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://df.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://om.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://yw.gzmigu.cn

[J07] 比较两个日期
来源：http://ix.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ux.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bf.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ce.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rd.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eo.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lg.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bi.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://qg.nszjky.cn

[J08] 提取年月日与星期
来源：http://cj.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tj.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bn.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cx.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wc.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kl.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xe.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rz.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ka.asd995.cn

[J09] 时区处理
来源：http://tn.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qv.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wz.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dv.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fa.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jh.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zi.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vg.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cr.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://os.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pe.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wa.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pg.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mx.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ks.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mf.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ku.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ga.shxzskj.cn

================================================================================
来源：http://ac.yuntaijiaju.cn

K. JSON 与序列化
来源：http://pa.huanxung.cn

================================================================================
来源：http://of.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://lv.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dj.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zp.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://it.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://dz.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sx.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://la.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bn.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vq.hahajie.cn

[K02] JSON 字符串转对象
来源：http://dt.shtwfgs.cn

Py:   json.loads(s)
来源：http://zz.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yt.szxytkj.cn

JS:   JSON.parse(s)
来源：http://rp.asd995.cn

TS:   JSON.parse(s)
来源：http://dg.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ra.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://ai.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://hx.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rm.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://io.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qh.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vn.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lh.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gm.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pb.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sx.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vi.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://id.szsharing.cn

[K04] 读取 JSON 文件
来源：http://po.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uk.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ad.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dr.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xo.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nq.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://et.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oh.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xw.haigaiapp.cn

[K05] 深拷贝对象
来源：http://la.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://fx.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://dt.lnxyls.cn

JS:   structuredClone(obj)
来源：http://aw.nicolike.cn

TS:   structuredClone(obj)
来源：http://os.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ol.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wy.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xx.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zz.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://hi.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pl.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rl.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wx.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qt.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uu.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oj.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qo.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://is.shtwfgs.cn

[K07] 进制转换
来源：http://sv.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hs.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jw.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ok.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pj.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dq.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fp.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jo.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nk.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://uk.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://qu.huanxung.cn


<!-- 参考信息 -->