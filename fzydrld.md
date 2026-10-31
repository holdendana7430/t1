代发 wailian999

[H07] 断言
来源：http://ec.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://hc.hnjuh.cn

PHP:  assert($x > 0);
来源：http://ri.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://ki.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://yu.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://da.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tn.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hp.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://pp.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://rv.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://kb.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ey.hnjuh.cn

JS:   e.message;  e.stack
来源：http://lw.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cf.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://te.huixinmuqiang.cn

Go:   err.Error()
来源：http://ij.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://fy.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://up.asd995.cn

[H09] 带错误码的异常
来源：http://rq.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sr.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ui.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cn.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mp.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tb.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ym.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yk.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bn.haigaiapp.cn

[H10] 资源自动释放
来源：http://nw.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yc.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aa.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oh.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://it.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://or.wgjwhj.cn

Go:   defer f.Close()
来源：http://mq.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fb.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iv.muxihuayi.cn

================================================================================
来源：http://pp.szxytkj.cn

I. 正则表达式
来源：http://lm.huixinmuqiang.cn

================================================================================
来源：http://vp.szxytkj.cn

[I01] 判断是否匹配
来源：http://jj.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://be.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ug.colortex.cn

JS:   /\d+/.test(s)
来源：http://as.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://ha.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ag.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zl.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://xa.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gs.muxihuayi.cn

[I02] 提取所有匹配
来源：http://nz.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://vz.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pu.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jh.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://tr.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cg.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mc.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://mx.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cv.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ml.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pz.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rw.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ux.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jt.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hv.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wm.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qd.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rk.bjjhwx.cn

[I04] 正则替换
来源：http://ki.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://po.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yd.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zf.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qx.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://om.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dq.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jy.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ce.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://cu.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://am.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://up.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://te.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wv.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://xf.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mq.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ik.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zu.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kx.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ju.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://du.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xf.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ze.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ry.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ag.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ra.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://si.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://et.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dj.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aj.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jj.szxytkj.cn

TS:   /error/gim
来源：http://yz.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ou.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bl.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://df.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oi.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://ht.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bi.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rz.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kk.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uy.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ki.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jy.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vt.jctech888.com.cn

================================================================================
来源：http://jf.huixinmuqiang.cn

J. 日期与时间
来源：http://tq.shtwfgs.cn

================================================================================
来源：http://ee.huixiangedu.cn

[J01] 获取当前时间
来源：http://cy.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://na.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mg.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://ic.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://of.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://si.huixiangedu.cn

Go:   time.Now()
来源：http://ga.asd995.cn

Ruby: Time.now
来源：http://dc.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qa.yuntaijiaju.cn

[J02] 格式化输出
来源：http://hz.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cy.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iq.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cb.chemitech.net.cn

TS:   d.toISOString()
来源：http://ju.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jb.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://si.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xc.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ia.szsharing.cn

[J03] 字符串解析为日期
来源：http://ou.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://da.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oz.colortex.cn

JS:   new Date("2024-01-02")
来源：http://ux.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://xj.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://og.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hd.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cw.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hj.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://pp.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://al.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cn.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ic.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bq.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qp.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yq.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eu.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://be.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://kv.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ap.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lc.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ua.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fj.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://om.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pc.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://kd.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://so.muxihuayi.cn

[J06] 计算两时间之差
来源：http://nk.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://wu.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://il.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ff.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yj.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jb.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://se.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ms.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ik.haigaiapp.cn

[J07] 比较两个日期
来源：http://ej.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://fr.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mh.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yd.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hj.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://an.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eo.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uv.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bf.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://si.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ig.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://od.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iw.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pr.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qp.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://po.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mc.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.bjjhwx.cn

[J09] 时区处理
来源：http://bq.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ic.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ux.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ph.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tb.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hl.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fu.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mt.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kk.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://dl.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ku.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mq.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jo.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ok.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ea.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://me.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cc.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qp.bjjhwx.cn

================================================================================
来源：http://ds.shxzukj.cn

K. JSON 与序列化
来源：http://op.bookmarksfly.cn

================================================================================
来源：http://is.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://cb.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fy.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://um.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://jx.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://ot.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cn.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://xm.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ks.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gr.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://sg.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://rc.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://up.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://sj.szxytkj.cn

TS:   JSON.parse(s)
来源：http://bk.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tt.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://fa.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://kp.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mm.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://oa.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nf.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iy.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ug.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gg.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xa.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bp.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ua.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://co.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://cj.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hs.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lb.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ua.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yh.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hg.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ba.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mm.jctech888.com.cn

[K05] 深拷贝对象
来源：http://sz.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://oq.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://kd.nicolike.cn

JS:   structuredClone(obj)
来源：http://xe.lnxyls.cn

TS:   structuredClone(obj)
来源：http://cr.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://os.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wc.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jd.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pw.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://vk.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cm.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vv.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aw.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vx.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xs.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fk.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zm.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vp.szsharing.cn

[K07] 进制转换
来源：http://tk.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cv.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qr.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yi.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pu.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zs.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cm.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gz.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kq.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://tn.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://hr.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://be.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://hg.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://eu.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yf.huixinmuqiang.cn

Go:   encoding/gob
来源：http://gw.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://qy.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fj.colortex.cn

================================================================================
来源：http://ns.shtwfgs.cn

L. 网络请求
来源：http://gn.nicolike.cn

================================================================================
来源：http://hp.shxzukj.cn

[L01] 发送 GET 请求
来源：http://md.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pu.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tf.asd995.cn

JS:   await fetch(url)
来源：http://hh.chemitech.net.cn

TS:   await fetch(url)
来源：http://ne.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qd.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://zl.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hw.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yg.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://tj.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ge.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zw.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zj.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jd.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sz.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ol.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fs.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dl.huixinmuqiang.cn


<!-- 参考信息 -->