代发 wailian999

JS:   class MyError extends Error {}
来源：http://sw.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://lf.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://du.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nq.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://sk.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://or.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://gp.shxzskj.cn

Py:   except ValueError as e:
来源：http://pp.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kh.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://gf.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ez.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://ua.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pq.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://pg.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cm.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://ub.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://rq.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ut.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zz.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jx.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yd.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hi.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://yj.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://hu.szsharing.cn

[H07] 断言
来源：http://sw.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://uv.szsharing.cn

PHP:  assert($x > 0);
来源：http://pn.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://hj.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://rg.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ci.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vw.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://un.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://xf.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://rx.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://dw.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sg.shxzukj.cn

JS:   e.message;  e.stack
来源：http://ln.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ei.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ya.9csxet.cn

Go:   err.Error()
来源：http://rl.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://po.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://rn.szxytkj.cn

[H09] 带错误码的异常
来源：http://lr.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mw.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vp.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nl.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://av.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ya.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://al.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ur.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ox.gzmigu.cn

[H10] 资源自动释放
来源：http://uk.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zl.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ic.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xh.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hx.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ck.521024.cn

Go:   defer f.Close()
来源：http://er.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ij.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xe.lnxyls.cn

================================================================================
来源：http://zz.shxzskj.cn

I. 正则表达式
来源：http://uz.muxihuayi.cn

================================================================================
来源：http://kj.asd995.cn

[I01] 判断是否匹配
来源：http://pf.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vp.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://es.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://mv.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://cg.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fb.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gb.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://qj.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ap.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://cf.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://fx.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bg.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pq.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ow.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yu.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nv.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://km.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dz.bjjhwx.cn

[I03] 提取捕获分组
来源：http://tk.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bn.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hj.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yg.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uv.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wz.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yc.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ab.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uj.newstarts.cn

[I04] 正则替换
来源：http://xz.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dx.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wn.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hr.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://um.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://al.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sj.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mq.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hf.shxzskj.cn

[I05] 按正则拆分
来源：http://ct.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qk.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lr.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://oy.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://iz.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://hw.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pv.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ho.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qa.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pp.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bw.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jg.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rm.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ml.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://of.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qo.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zm.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uv.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://gs.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vh.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wz.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gi.shxzskj.cn

TS:   /error/gim
来源：http://jc.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dd.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://su.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://ht.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qt.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://mv.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://db.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ry.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mj.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://do.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tn.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hf.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dl.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dw.haigaiapp.cn

================================================================================
来源：http://zf.chemitech.net.cn

J. 日期与时间
来源：http://rb.colortex.cn

================================================================================
来源：http://cq.szxytkj.cn

[J01] 获取当前时间
来源：http://hk.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ej.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wp.nszjky.cn

JS:   new Date();  Date.now()
来源：http://fw.huanxung.cn

TS:   new Date();  Date.now()
来源：http://yg.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gx.9csxet.cn

Go:   time.Now()
来源：http://ai.shxzskj.cn

Ruby: Time.now
来源：http://cv.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vc.chemitech.net.cn

[J02] 格式化输出
来源：http://xv.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tp.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gh.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xk.bjjhwx.cn

TS:   d.toISOString()
来源：http://ce.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hx.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fr.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cs.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eh.shxzukj.cn

[J03] 字符串解析为日期
来源：http://hj.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://si.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cw.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://nf.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ul.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vg.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ap.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://hw.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pg.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://ml.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fg.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xo.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ph.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sh.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fy.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mm.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nh.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rq.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://yw.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://tv.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sq.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://af.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://jk.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kc.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ly.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hj.hahajie.cn

[J06] 计算两时间之差
来源：http://hn.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://mn.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ts.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jz.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ms.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ia.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://pn.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://tc.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://vm.huixiangedu.cn

[J07] 比较两个日期
来源：http://sk.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://pf.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kj.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oo.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fm.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nd.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xh.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qs.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://iy.nszjky.cn

[J08] 提取年月日与星期
来源：http://rj.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mo.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hb.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jb.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vm.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://in.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://io.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ow.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dy.huixinmuqiang.cn

[J09] 时区处理
来源：http://ty.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aj.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://in.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ws.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://po.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zd.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iy.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fj.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iv.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://kn.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qy.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sn.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ev.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bq.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ja.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://da.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wt.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uf.colortex.cn

================================================================================
来源：http://zk.jctech888.com.cn

K. JSON 与序列化
来源：http://ep.chemitech.net.cn

================================================================================
来源：http://uc.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://wx.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tf.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ec.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://fr.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://kx.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ds.asd995.cn

Go:   json.Marshal(obj)
来源：http://fi.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yc.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ja.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ho.nicolike.cn

Py:   json.loads(s)
来源：http://sl.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ao.colortex.cn

JS:   JSON.parse(s)
来源：http://sc.shxzukj.cn

TS:   JSON.parse(s)
来源：http://ml.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xr.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://hg.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://wr.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dt.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://bd.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rl.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bo.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hu.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fh.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yr.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aj.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ip.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mx.hahajie.cn

[K04] 读取 JSON 文件
来源：http://vi.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sy.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kb.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kj.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xi.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ib.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wx.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jm.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aq.hahajie.cn

[K05] 深拷贝对象
来源：http://si.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://da.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://on.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://pf.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://xb.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fs.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ut.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uk.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nh.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ll.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ox.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fc.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mt.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ul.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://no.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wk.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://de.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fw.huixinmuqiang.cn

[K07] 进制转换
来源：http://ir.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dt.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wt.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://da.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://la.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tu.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zf.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qg.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ap.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tt.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://bv.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lx.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://yl.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ax.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ay.newstarts.cn


<!-- 参考信息 -->