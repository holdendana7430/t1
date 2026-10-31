代发 wailian999

[H07] 断言
来源：http://wa.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://jv.asd995.cn

PHP:  assert($x > 0);
来源：http://pb.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://ep.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://lj.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://kz.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jd.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rz.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://hz.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://mo.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://on.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fy.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://tp.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kc.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ye.wgjwhj.cn

Go:   err.Error()
来源：http://zf.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://rc.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://cu.haigaiapp.cn

[H09] 带错误码的异常
来源：http://pt.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ic.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hn.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ew.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eh.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pi.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://be.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tr.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qv.yuexingan06.cn

[H10] 资源自动释放
来源：http://gz.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wu.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tc.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bs.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uc.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ku.szxytkj.cn

Go:   defer f.Close()
来源：http://xs.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jj.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lk.haigaiapp.cn

================================================================================
来源：http://ua.bookmarksfly.cn

I. 正则表达式
来源：http://md.jianghongdianzi.cn

================================================================================
来源：http://eo.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ww.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wl.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mi.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://jv.hahajie.cn

TS:   /\d+/.test(s)
来源：http://dx.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nb.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qb.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://po.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://an.shtwfgs.cn

[I02] 提取所有匹配
来源：http://rb.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://oz.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ua.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kr.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://ls.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hy.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ke.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://cr.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mp.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://lj.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yd.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nr.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oy.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zk.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ac.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yd.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ti.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pa.yuntaijiaju.cn

[I04] 正则替换
来源：http://iw.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jk.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qb.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ct.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gv.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://so.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zj.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vh.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dm.panjiajie.cn

[I05] 按正则拆分
来源：http://ku.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ni.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qu.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://tc.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ug.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://sh.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ca.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jc.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fk.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ud.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uz.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ay.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vl.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wu.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dm.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ry.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bb.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rh.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://cm.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xa.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fw.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ea.bookmarksfly.cn

TS:   /error/gim
来源：http://eb.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bh.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qy.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ro.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://nk.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fl.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ps.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://da.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pn.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ow.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vc.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ea.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sw.asd995.cn

================================================================================
来源：http://wt.newstarts.cn

J. 日期与时间
来源：http://dx.jianghongdianzi.cn

================================================================================
来源：http://pn.szxytkj.cn

[J01] 获取当前时间
来源：http://xs.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qa.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ro.hahajie.cn

JS:   new Date();  Date.now()
来源：http://dz.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://ak.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ph.wgjwhj.cn

Go:   time.Now()
来源：http://pd.newstarts.cn

Ruby: Time.now
来源：http://yg.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dx.panjiajie.cn

[J02] 格式化输出
来源：http://fz.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ve.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ow.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mq.lnxyls.cn

TS:   d.toISOString()
来源：http://ei.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cb.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bj.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kf.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lp.huanxung.cn

[J03] 字符串解析为日期
来源：http://yq.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qx.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sl.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://ty.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://xr.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nl.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://up.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://yi.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ru.colortex.cn

[J04] 时间戳与日期互转
来源：http://wc.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bu.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vs.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mn.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://is.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mw.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ff.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rk.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ae.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ec.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://sq.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gn.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hd.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tg.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://pb.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uj.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://gn.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lz.newstarts.cn

[J06] 计算两时间之差
来源：http://ra.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://dd.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://xv.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dn.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gl.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ye.521024.cn

Go:   end.Sub(start).Hours()
来源：http://iu.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://fs.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://zv.huanxung.cn

[J07] 比较两个日期
来源：http://qz.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://un.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bh.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yt.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bb.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gi.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://te.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://as.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://zn.nicolike.cn

[J08] 提取年月日与星期
来源：http://fw.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yi.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gt.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zc.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pl.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rn.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://st.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://go.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rr.shxzukj.cn

[J09] 时区处理
来源：http://ex.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nu.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bc.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ji.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zp.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pr.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cj.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tf.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yf.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://kq.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jv.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ir.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gx.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gw.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bv.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ka.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://on.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xm.yuexingan06.cn

================================================================================
来源：http://az.asd995.cn

K. JSON 与序列化
来源：http://qn.nicolike.cn

================================================================================
来源：http://gx.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://fm.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tb.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bf.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://yp.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://oq.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cu.asd995.cn

Go:   json.Marshal(obj)
来源：http://ga.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ks.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gs.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://jv.shtwfgs.cn

Py:   json.loads(s)
来源：http://kt.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gj.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://so.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://fo.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cp.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://tt.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://gv.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lv.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://ob.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nc.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yl.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ar.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lb.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ad.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ni.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iw.hahajie.cn

[K04] 读取 JSON 文件
来源：http://uu.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ri.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kx.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vg.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qv.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hr.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rw.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vn.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sk.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://kb.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://kh.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://tv.newstarts.cn

JS:   structuredClone(obj)
来源：http://dk.huanxung.cn

TS:   structuredClone(obj)
来源：http://hr.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rr.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nl.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://po.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xx.asd995.cn

[K06] 解析 URL 查询串
来源：http://ci.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aq.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rp.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://na.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wx.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zj.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wo.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ap.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tn.huixinmuqiang.cn

[K07] 进制转换
来源：http://fp.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rk.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kv.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hy.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ge.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xl.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ku.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vu.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://no.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://he.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://gt.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mk.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://qh.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://cg.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ec.gzmigu.cn

Go:   encoding/gob
来源：http://kk.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://ws.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pd.jianghongdianzi.cn

================================================================================
来源：http://wm.szsharing.cn

L. 网络请求
来源：http://ye.muxihuayi.cn

================================================================================
来源：http://pl.asd995.cn

[L01] 发送 GET 请求
来源：http://ri.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ww.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jk.yuexingan06.cn

JS:   await fetch(url)
来源：http://sf.nszjky.cn

TS:   await fetch(url)
来源：http://pq.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hv.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://aw.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ty.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kp.asd995.cn

[L02] 发送 POST JSON
来源：http://yh.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ia.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qu.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rp.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sq.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kq.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fc.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zd.bookmarksfly.cn


<!-- 参考信息 -->