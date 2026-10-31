代发 wailian999

Py:   value = d.get("k") or default
来源：http://nu.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xv.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sm.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xz.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wa.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://to.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://fd.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://xl.bookmarksfly.cn

[H07] 断言
来源：http://yn.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://qi.colortex.cn

PHP:  assert($x > 0);
来源：http://ph.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://nx.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://pz.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://hy.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cp.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ya.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ed.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://sd.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://eh.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ru.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://rk.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xa.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nc.jctech888.com.cn

Go:   err.Error()
来源：http://qh.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://yy.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://ic.hnjuh.cn

[H09] 带错误码的异常
来源：http://kl.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jg.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mk.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hk.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jv.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://su.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ja.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jy.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pp.newstarts.cn

[H10] 资源自动释放
来源：http://gq.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qo.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zv.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pg.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pz.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rm.chemitech.net.cn

Go:   defer f.Close()
来源：http://fk.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lu.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kp.huixinmuqiang.cn

================================================================================
来源：http://wt.jianghongdianzi.cn

I. 正则表达式
来源：http://bl.gzmigu.cn

================================================================================
来源：http://rd.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://ld.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://im.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fk.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://fs.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://pc.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ar.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ul.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://vc.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bc.nszjky.cn

[I02] 提取所有匹配
来源：http://yk.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://kd.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rv.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rm.521024.cn

TS:   s.match(/\d+/g)
来源：http://vm.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ta.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bs.521024.cn

Ruby: s.scan(/\d+/)
来源：http://jr.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zp.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://zd.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ha.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cf.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pi.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rg.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vm.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gn.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ep.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vs.szxytkj.cn

[I04] 正则替换
来源：http://rg.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bp.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ct.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pq.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pu.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ie.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://by.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rw.asd995.cn

[I05] 按正则拆分
来源：http://gr.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rd.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wp.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://fu.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://sg.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://cx.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ia.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ub.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sh.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://of.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rw.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rj.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ca.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zp.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tu.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://so.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pm.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lp.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://xt.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lj.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qg.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ok.bjjhwx.cn

TS:   /error/gim
来源：http://yc.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rz.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yv.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://ly.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ef.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://kw.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fo.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cv.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://md.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xz.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tv.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ct.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lz.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rj.asd995.cn

================================================================================
来源：http://cz.lnxyls.cn

J. 日期与时间
来源：http://sp.gzmigu.cn

================================================================================
来源：http://wi.shtwfgs.cn

[J01] 获取当前时间
来源：http://sc.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xa.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nv.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://yl.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://yw.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://if.521024.cn

Go:   time.Now()
来源：http://ey.shxzskj.cn

Ruby: Time.now
来源：http://mf.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://in.shtwfgs.cn

[J02] 格式化输出
来源：http://ge.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dk.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qu.huixiangedu.cn

TS:   d.toISOString()
来源：http://wp.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sc.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yj.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nx.szsharing.cn

[J03] 字符串解析为日期
来源：http://xx.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pw.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://px.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://we.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://kr.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ry.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ws.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zf.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://hi.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nh.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fs.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ng.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lx.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rh.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jj.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rt.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nb.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://mp.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://mv.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jn.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jd.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jw.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://bw.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rm.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://wv.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tc.huixiangedu.cn

[J06] 计算两时间之差
来源：http://sn.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://pi.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://ox.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jk.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://su.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vu.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://sk.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ul.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://za.wgjwhj.cn

[J07] 比较两个日期
来源：http://fh.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://bh.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://su.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mg.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://by.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sg.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gu.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ob.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ow.hnjuh.cn

[J08] 提取年月日与星期
来源：http://zx.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xa.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jh.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://om.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yj.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iw.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xq.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tr.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nc.muxihuayi.cn

[J09] 时区处理
来源：http://ld.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hd.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gz.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jh.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://px.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://va.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yc.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hm.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pj.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://oc.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rm.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sf.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kg.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xy.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bg.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pj.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ta.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sn.newstarts.cn

================================================================================
来源：http://kx.newstarts.cn

K. JSON 与序列化
来源：http://cf.huixinmuqiang.cn

================================================================================
来源：http://mt.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://ks.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gj.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mp.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://tx.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://bn.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xn.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ir.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aj.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aq.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://yf.lnxyls.cn

Py:   json.loads(s)
来源：http://di.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://im.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://mo.huanxung.cn

TS:   JSON.parse(s)
来源：http://fi.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hg.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://qh.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://sv.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ag.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://aj.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mw.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vt.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eo.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ab.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vy.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iw.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cl.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eh.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ps.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rd.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ie.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nm.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xa.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yu.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pr.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uj.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ai.shtwfgs.cn

[K05] 深拷贝对象
来源：http://nk.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ov.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://uw.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://if.panjiajie.cn

TS:   structuredClone(obj)
来源：http://ia.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ph.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ls.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zg.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qe.colortex.cn

[K06] 解析 URL 查询串
来源：http://nr.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://js.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://em.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bn.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kn.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oq.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bo.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bv.colortex.cn

[K07] 进制转换
来源：http://bf.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ci.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hq.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ri.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cc.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ln.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fi.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cb.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hm.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://yl.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://qm.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iy.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://lv.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://xv.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rc.haigaiapp.cn

Go:   encoding/gob
来源：http://sz.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://uq.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xl.9csxet.cn

================================================================================
来源：http://xi.chemitech.net.cn

L. 网络请求
来源：http://wc.szsharing.cn

================================================================================
来源：http://hv.nszjky.cn

[L01] 发送 GET 请求
来源：http://mj.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jx.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hb.nszjky.cn

JS:   await fetch(url)
来源：http://sb.szsharing.cn

TS:   await fetch(url)
来源：http://ex.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ue.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://vw.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mb.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://px.gzmigu.cn

[L02] 发送 POST JSON
来源：http://mz.haigaiapp.cn


<!-- 参考信息 -->