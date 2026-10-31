代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zx.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://qd.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ms.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://wm.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://gb.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zq.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ov.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ux.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jz.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cv.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://mc.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://oq.huixinmuqiang.cn

[H07] 断言
来源：http://ia.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://on.shxzukj.cn

PHP:  assert($x > 0);
来源：http://hg.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://qc.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://oh.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://ud.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ye.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fv.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://uc.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://sy.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://vd.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ku.shxzukj.cn

JS:   e.message;  e.stack
来源：http://tr.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hv.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://my.panjiajie.cn

Go:   err.Error()
来源：http://ga.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://gy.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://pr.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://rr.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ah.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oq.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://os.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bv.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://br.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lv.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ik.nszjky.cn

[H10] 资源自动释放
来源：http://xt.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cz.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ea.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nz.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kd.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://li.haigaiapp.cn

Go:   defer f.Close()
来源：http://cs.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://br.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ro.shtwfgs.cn

================================================================================
来源：http://il.jctech888.com.cn

I. 正则表达式
来源：http://fh.nicolike.cn

================================================================================
来源：http://dn.chemitech.net.cn

[I01] 判断是否匹配
来源：http://ot.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ye.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tb.hahajie.cn

JS:   /\d+/.test(s)
来源：http://mo.szsharing.cn

TS:   /\d+/.test(s)
来源：http://yz.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mn.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vi.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://rs.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ay.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://wq.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://qd.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zb.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qz.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://uj.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fb.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ce.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://ge.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hf.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sl.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ec.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pq.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pf.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ds.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zh.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fn.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vp.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rf.gzmigu.cn

[I04] 正则替换
来源：http://rx.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uc.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mq.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kc.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lt.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bx.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kn.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sd.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jw.huanxung.cn

[I05] 按正则拆分
来源：http://ge.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yh.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://em.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ax.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://bj.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://fu.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xv.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ev.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nd.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kk.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://km.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uu.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ix.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zh.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hn.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eu.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ym.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://an.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://td.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qn.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nk.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aq.nicolike.cn

TS:   /error/gim
来源：http://po.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jn.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://zi.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://um.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://pd.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ll.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tz.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cs.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vn.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vn.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://re.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sr.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ps.jianghongdianzi.cn

================================================================================
来源：http://er.huixinmuqiang.cn

J. 日期与时间
来源：http://cg.9csxet.cn

================================================================================
来源：http://zw.chemitech.net.cn

[J01] 获取当前时间
来源：http://ma.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hb.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gy.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ub.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://jk.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eo.hahajie.cn

Go:   time.Now()
来源：http://or.huanxung.cn

Ruby: Time.now
来源：http://zs.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bb.shxzukj.cn

[J02] 格式化输出
来源：http://xu.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rk.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ol.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mq.huanxung.cn

TS:   d.toISOString()
来源：http://sq.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://na.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gy.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://on.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gc.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://om.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://km.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yf.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://mb.521024.cn

TS:   new Date("2024-01-02")
来源：http://eb.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zu.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sb.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://la.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gm.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://te.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ig.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rg.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ww.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ef.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wj.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hh.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cw.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zt.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://zi.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://tq.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nh.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nz.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ey.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://eg.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sa.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://xa.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://or.colortex.cn

[J06] 计算两时间之差
来源：http://sh.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://bh.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://nc.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xc.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://au.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sb.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ur.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://qb.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://in.newstarts.cn

[J07] 比较两个日期
来源：http://kk.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://de.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kj.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oh.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xe.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vf.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zv.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zg.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://fy.nicolike.cn

[J08] 提取年月日与星期
来源：http://ds.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cv.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ed.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ri.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://we.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ex.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ch.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wy.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mn.newstarts.cn

[J09] 时区处理
来源：http://ri.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sr.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ms.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jp.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pw.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wu.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pv.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rq.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://nv.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ky.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wd.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ya.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ed.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lm.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://an.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://om.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pk.huanxung.cn

================================================================================
来源：http://yl.huixiangedu.cn

K. JSON 与序列化
来源：http://wg.nszjky.cn

================================================================================
来源：http://ci.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ip.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xh.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://we.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://xm.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ej.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wa.nicolike.cn

Go:   json.Marshal(obj)
来源：http://vq.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jy.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qz.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://xn.huanxung.cn

Py:   json.loads(s)
来源：http://vh.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eg.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://np.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://bx.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fb.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://nv.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://mq.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jn.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://vp.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://il.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pw.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://it.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nf.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xa.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://au.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xk.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dp.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://nq.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tg.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aa.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pe.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gq.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jt.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mf.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sc.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ni.hnjuh.cn

[K05] 深拷贝对象
来源：http://ei.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://jl.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://de.hahajie.cn

JS:   structuredClone(obj)
来源：http://rz.szxytkj.cn

TS:   structuredClone(obj)
来源：http://vb.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pe.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jw.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://th.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vr.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://yi.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kb.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mc.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xk.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tq.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pi.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gv.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rm.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ho.hahajie.cn

[K07] 进制转换
来源：http://at.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ss.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uq.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qg.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wr.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mt.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://al.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jn.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oi.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://bf.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://hu.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ic.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://bu.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://gq.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://by.gzmigu.cn

Go:   encoding/gob
来源：http://yp.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://dl.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ev.bookmarksfly.cn

================================================================================
来源：http://bc.newstarts.cn

L. 网络请求
来源：http://fp.lnxyls.cn

================================================================================
来源：http://dn.szsharing.cn

[L01] 发送 GET 请求
来源：http://co.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ql.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://um.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://el.muxihuayi.cn

TS:   await fetch(url)
来源：http://ip.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dv.asd995.cn


<!-- 参考信息 -->