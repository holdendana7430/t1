代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dj.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://si.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ec.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://hp.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mn.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://iy.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jb.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ms.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://bp.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zb.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tm.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ys.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cu.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ac.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://eu.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://tw.nszjky.cn

[H07] 断言
来源：http://ue.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://pi.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://po.asd995.cn

JS:   console.assert(x > 0);
来源：http://ac.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://gk.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://ml.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yd.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nr.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://vy.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://re.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://xw.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pu.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://zz.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://og.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bj.szsharing.cn

Go:   err.Error()
来源：http://ge.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://gn.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://gi.nszjky.cn

[H09] 带错误码的异常
来源：http://xp.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pg.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fx.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jw.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bp.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iv.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ez.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://is.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lw.nszjky.cn

[H10] 资源自动释放
来源：http://ey.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ci.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dh.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pm.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lp.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tc.colortex.cn

Go:   defer f.Close()
来源：http://ws.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://st.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nm.nicolike.cn

================================================================================
来源：http://lw.shtwfgs.cn

I. 正则表达式
来源：http://ct.gzmigu.cn

================================================================================
来源：http://gq.newstarts.cn

[I01] 判断是否匹配
来源：http://bq.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ii.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rk.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://xn.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://gr.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mv.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vn.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://er.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://da.shxzskj.cn

[I02] 提取所有匹配
来源：http://qb.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://ar.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nh.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nu.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://nd.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zu.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sr.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://ny.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hj.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ry.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iv.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://du.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bh.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jc.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rh.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vl.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ce.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mr.colortex.cn

[I04] 正则替换
来源：http://fk.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nq.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lz.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rq.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lt.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kw.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zp.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ga.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ke.huixiangedu.cn

[I05] 按正则拆分
来源：http://eu.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rs.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cf.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://ee.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://je.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ps.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nz.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ff.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mc.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qe.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pe.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aq.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kl.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yf.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dk.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bq.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fk.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://al.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://sy.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mn.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sl.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yn.huixinmuqiang.cn

TS:   /error/gim
来源：http://hy.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ey.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gl.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://cg.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mj.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://mh.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ts.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://um.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bz.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pd.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iz.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kn.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jz.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pg.asd995.cn

================================================================================
来源：http://ey.nicolike.cn

J. 日期与时间
来源：http://ef.nszjky.cn

================================================================================
来源：http://xx.newstarts.cn

[J01] 获取当前时间
来源：http://bc.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ap.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fx.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://qn.nszjky.cn

TS:   new Date();  Date.now()
来源：http://el.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fp.muxihuayi.cn

Go:   time.Now()
来源：http://ph.nicolike.cn

Ruby: Time.now
来源：http://ik.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ad.huanxung.cn

[J02] 格式化输出
来源：http://eb.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jt.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wg.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jx.panjiajie.cn

TS:   d.toISOString()
来源：http://ej.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gw.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dp.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://la.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kl.nszjky.cn

[J03] 字符串解析为日期
来源：http://qo.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sg.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fg.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://ri.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://fl.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sk.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pa.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://vk.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://om.asd995.cn

[J04] 时间戳与日期互转
来源：http://bt.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ax.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cp.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ts.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vf.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wi.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qu.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gq.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wq.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://nw.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://em.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ms.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bp.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://zm.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ni.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://jz.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ys.521024.cn

[J06] 计算两时间之差
来源：http://il.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://fm.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://fx.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jo.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ab.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://le.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://qa.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://en.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://or.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://vn.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://qh.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lq.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vb.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dq.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jd.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://le.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gq.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://pt.newstarts.cn

[J08] 提取年月日与星期
来源：http://zc.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ja.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gk.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jh.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jp.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lr.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ho.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lb.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pj.shxzskj.cn

[J09] 时区处理
来源：http://oy.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://re.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://em.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dc.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kf.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zv.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ii.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ep.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nd.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://qv.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kf.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xn.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ev.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gb.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ir.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yk.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ms.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vf.asd995.cn

================================================================================
来源：http://eu.newstarts.cn

K. JSON 与序列化
来源：http://mt.hnjuh.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://yh.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pb.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ib.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://rp.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://me.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hw.newstarts.cn

Go:   json.Marshal(obj)
来源：http://vt.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wh.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ig.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://bi.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ke.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mk.shxzukj.cn

JS:   JSON.parse(s)
来源：http://wi.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://qs.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://il.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ff.colortex.cn

Ruby: JSON.parse(s)
来源：http://xf.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bv.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://sa.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ll.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ps.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ew.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ls.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://st.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ts.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cr.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fq.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://bq.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dj.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jo.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mx.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rl.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ed.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://li.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ym.9csxet.cn

[K05] 深拷贝对象
来源：http://xu.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://sy.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://tr.521024.cn

JS:   structuredClone(obj)
来源：http://vq.521024.cn

TS:   structuredClone(obj)
来源：http://le.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ug.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://df.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://th.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qj.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://zi.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oo.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lo.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zw.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://px.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tg.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hi.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zh.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ii.lnxyls.cn

[K07] 进制转换
来源：http://fq.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yc.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yv.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ln.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dp.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fq.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uj.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kk.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gz.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gi.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://eb.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lj.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://dk.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://uu.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wm.nicolike.cn

Go:   encoding/gob
来源：http://mk.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://lv.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fz.jctech888.com.cn

================================================================================
来源：http://to.huanxung.cn

L. 网络请求
来源：http://kp.huanxung.cn

================================================================================
来源：http://vu.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://jo.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sb.bookmarksfly.cn


<!-- 参考信息 -->