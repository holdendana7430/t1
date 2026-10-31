代发 wailian999

Py:   value = d.get("k") or default
来源：http://oe.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ep.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://at.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cz.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ic.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lt.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://th.colortex.cn

[H07] 断言
来源：http://rk.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://nb.shxzskj.cn

PHP:  assert($x > 0);
来源：http://rr.nicolike.cn

JS:   console.assert(x > 0);
来源：http://fk.9csxet.cn

TS:   console.assert(x > 0);
来源：http://eb.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://ey.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lj.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ve.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://sm.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://qb.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://ij.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uv.asd995.cn

JS:   e.message;  e.stack
来源：http://zs.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jr.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://so.nszjky.cn

Go:   err.Error()
来源：http://ur.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://oc.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://xt.gzmigu.cn

[H09] 带错误码的异常
来源：http://ue.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sd.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rg.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gw.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bj.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ml.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xl.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bw.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yd.huixiangedu.cn

[H10] 资源自动释放
来源：http://dq.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ts.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gz.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vs.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kl.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ol.hnjuh.cn

Go:   defer f.Close()
来源：http://zk.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cv.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tr.asd995.cn

================================================================================
来源：http://ko.9csxet.cn

I. 正则表达式
来源：http://be.hnjuh.cn

================================================================================
来源：http://kc.wgjwhj.cn

[I01] 判断是否匹配
来源：http://os.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qs.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xw.nicolike.cn

JS:   /\d+/.test(s)
来源：http://qg.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://ej.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jh.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ap.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://jv.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pa.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ls.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://us.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gh.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jw.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://hn.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lm.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nc.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://uv.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ek.newstarts.cn

[I03] 提取捕获分组
来源：http://js.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pt.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kv.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gl.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ny.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ff.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rv.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sj.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iq.shtwfgs.cn

[I04] 正则替换
来源：http://jv.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hf.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hr.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cb.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pj.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wu.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ol.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lf.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gx.bjjhwx.cn

[I05] 按正则拆分
来源：http://zs.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://on.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gc.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wt.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://fw.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://wq.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tp.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pa.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bn.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://js.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://be.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://er.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ts.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ub.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nb.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ee.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yn.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rg.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://yw.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mn.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yi.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tv.szxytkj.cn

TS:   /error/gim
来源：http://ag.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lk.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mm.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://uw.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xu.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://nk.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qq.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qt.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tp.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ak.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hn.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ll.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qt.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ju.jctech888.com.cn

================================================================================
来源：http://lk.asd995.cn

J. 日期与时间
来源：http://py.yuntaijiaju.cn

================================================================================
来源：http://ce.asd995.cn

[J01] 获取当前时间
来源：http://ju.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rn.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sk.colortex.cn

JS:   new Date();  Date.now()
来源：http://tf.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ip.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://op.shtwfgs.cn

Go:   time.Now()
来源：http://bu.chemitech.net.cn

Ruby: Time.now
来源：http://ol.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.nicolike.cn

[J02] 格式化输出
来源：http://hh.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rm.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lt.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ws.panjiajie.cn

TS:   d.toISOString()
来源：http://rx.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zk.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://li.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://il.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nc.colortex.cn

[J03] 字符串解析为日期
来源：http://yc.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mt.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dj.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://qb.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ez.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fd.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ei.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://vy.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uq.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://jx.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rk.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fw.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ej.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cj.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vm.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ui.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mz.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qa.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://re.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://oo.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ut.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bk.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kj.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://yv.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qd.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://qu.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://na.panjiajie.cn

[J06] 计算两时间之差
来源：http://fi.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://ye.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://cb.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://la.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ge.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ye.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://yk.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://gn.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://kk.chemitech.net.cn

[J07] 比较两个日期
来源：http://az.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://de.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xl.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lp.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ka.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gy.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jm.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iu.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://wt.nicolike.cn

[J08] 提取年月日与星期
来源：http://il.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sf.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nr.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://el.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ua.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ac.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hd.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gf.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://be.newstarts.cn

[J09] 时区处理
来源：http://ik.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xk.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ax.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ze.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mi.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iu.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://el.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hl.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://da.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ew.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bl.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cm.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qd.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fv.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jt.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xd.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wb.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nj.nszjky.cn

================================================================================
来源：http://wl.szsharing.cn

K. JSON 与序列化
来源：http://gn.newstarts.cn

================================================================================
来源：http://yf.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://gt.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ia.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ox.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://us.asd995.cn

TS:   JSON.stringify(obj)
来源：http://yt.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nz.huanxung.cn

Go:   json.Marshal(obj)
来源：http://nk.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gp.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jm.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://bd.huanxung.cn

Py:   json.loads(s)
来源：http://gm.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tl.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://sv.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://uz.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cc.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://pv.huanxung.cn

Ruby: JSON.parse(s)
来源：http://cs.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lo.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://sb.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cr.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dk.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bl.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zy.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://io.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hq.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://le.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ep.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://pk.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tp.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qh.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jt.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://of.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zc.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rp.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gh.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kv.huixiangedu.cn

[K05] 深拷贝对象
来源：http://uf.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://jj.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://fa.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://mm.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://tl.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ew.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xy.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://im.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ji.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://yb.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qm.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iq.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gu.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://np.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xs.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mt.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ee.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ir.9csxet.cn

[K07] 进制转换
来源：http://sl.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pv.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jk.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nf.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xh.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qq.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ow.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sn.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ga.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://if.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://wq.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gg.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://vt.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ac.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dm.nicolike.cn

Go:   encoding/gob
来源：http://vy.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://st.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nx.hahajie.cn

================================================================================
来源：http://lo.chemitech.net.cn

L. 网络请求
来源：http://ka.wgjwhj.cn

================================================================================
来源：http://vc.lnxyls.cn

[L01] 发送 GET 请求
来源：http://fc.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gn.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fd.panjiajie.cn

JS:   await fetch(url)
来源：http://jc.gzmigu.cn

TS:   await fetch(url)
来源：http://tt.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ds.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://xs.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ia.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cc.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://bv.jianghongdianzi.cn


<!-- 参考信息 -->