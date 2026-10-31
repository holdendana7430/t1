代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://df.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ss.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://vy.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tx.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ra.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hn.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gj.521024.cn

Go:   err.Error()
来源：http://xt.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://le.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://lc.panjiajie.cn

[H09] 带错误码的异常
来源：http://id.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ka.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ap.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zb.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pv.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fr.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://if.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pu.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qt.shtwfgs.cn

[H10] 资源自动释放
来源：http://ty.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hr.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lh.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bl.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cd.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dz.yuexingan06.cn

Go:   defer f.Close()
来源：http://uu.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cp.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qd.jctech888.com.cn

================================================================================
来源：http://zh.huanxung.cn

I. 正则表达式
来源：http://sv.newstarts.cn

================================================================================
来源：http://rl.muxihuayi.cn

[I01] 判断是否匹配
来源：http://zu.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dq.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vh.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://nh.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://lc.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pf.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gw.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://mi.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zj.huixiangedu.cn

[I02] 提取所有匹配
来源：http://fb.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://nv.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ns.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aw.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://zq.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uz.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pj.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://wj.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bb.nicolike.cn

[I03] 提取捕获分组
来源：http://pi.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dq.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oo.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hk.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dr.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://df.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nt.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gt.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cw.wgjwhj.cn

[I04] 正则替换
来源：http://eu.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wy.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ib.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ya.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rz.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ub.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zq.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kf.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oj.panjiajie.cn

[I05] 按正则拆分
来源：http://mo.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sf.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uh.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://sx.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://lo.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://fc.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pj.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://an.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rn.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mb.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tk.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rr.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wa.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aw.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ru.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qm.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mz.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fh.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://qn.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ds.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ms.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://by.shtwfgs.cn

TS:   /error/gim
来源：http://kp.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eo.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ko.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://qt.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ve.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://gj.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mj.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ug.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gy.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ff.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zr.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://de.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oo.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ew.hahajie.cn

================================================================================
来源：http://ug.haigaiapp.cn

J. 日期与时间
来源：http://wv.nszjky.cn

================================================================================
来源：http://rl.huixiangedu.cn

[J01] 获取当前时间
来源：http://fn.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xx.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yw.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://ng.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ao.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pn.huanxung.cn

Go:   time.Now()
来源：http://wm.chemitech.net.cn

Ruby: Time.now
来源：http://kx.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qr.yuexingan06.cn

[J02] 格式化输出
来源：http://ft.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ub.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ep.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mg.szsharing.cn

TS:   d.toISOString()
来源：http://bq.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hy.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cx.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ii.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ce.hahajie.cn

[J03] 字符串解析为日期
来源：http://hd.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://er.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hv.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://nl.asd995.cn

TS:   new Date("2024-01-02")
来源：http://fz.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yt.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ix.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://lk.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wy.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://zc.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mm.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dc.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xn.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dr.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vi.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cl.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rv.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gp.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://qn.asd995.cn

Py:   now + timedelta(days=7)
来源：http://jn.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ud.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vq.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fr.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ds.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://cw.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gz.shtwfgs.cn

[J06] 计算两时间之差
来源：http://vq.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://bl.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://vs.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yy.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mm.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vt.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://xg.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ty.521024.cn

C#:   (end - start).TotalSeconds
来源：http://vm.szxytkj.cn

[J07] 比较两个日期
来源：http://ei.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://ev.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nu.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kg.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nv.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ib.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ax.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hd.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ze.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ki.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zt.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vj.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://so.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://px.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tl.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://om.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hl.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hj.newstarts.cn

[J09] 时区处理
来源：http://ah.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ez.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cu.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qj.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://of.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ou.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xw.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fy.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nb.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ft.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://af.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zu.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qf.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pl.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qo.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ne.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ng.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ww.newstarts.cn

================================================================================
来源：http://lm.lnxyls.cn

K. JSON 与序列化
来源：http://ng.chemitech.net.cn

================================================================================
来源：http://ly.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://gr.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kd.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fe.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://lo.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://lu.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lr.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://zd.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hl.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qe.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://gd.panjiajie.cn

Py:   json.loads(s)
来源：http://rb.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qh.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://tg.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://py.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://er.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://wi.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://dv.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jt.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://oo.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ku.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eq.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ov.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wj.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lp.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pu.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sw.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wt.nicolike.cn

[K04] 读取 JSON 文件
来源：http://la.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://az.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://op.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ty.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ic.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gk.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ip.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ww.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ec.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://dm.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://ju.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://pa.szsharing.cn

JS:   structuredClone(obj)
来源：http://sg.szsharing.cn

TS:   structuredClone(obj)
来源：http://kf.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nx.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ij.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xy.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mr.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://kh.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rl.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vj.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qg.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pd.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://be.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yb.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yg.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bp.huixinmuqiang.cn

[K07] 进制转换
来源：http://hg.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kj.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sq.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fc.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jq.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qv.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uu.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gi.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eq.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://pp.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ct.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nl.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://cp.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://jz.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wo.yuexingan06.cn

Go:   encoding/gob
来源：http://nz.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://tw.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qi.jctech888.com.cn

================================================================================
来源：http://ik.yuntaijiaju.cn

L. 网络请求
来源：http://du.szsharing.cn

================================================================================
来源：http://wo.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ul.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rm.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nj.shxzskj.cn

JS:   await fetch(url)
来源：http://gv.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://rn.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xj.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://cg.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rk.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://st.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ed.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://og.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mi.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eu.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zn.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mf.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ku.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hw.nicolike.cn

[L03] 设置自定义请求头
来源：http://mr.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wt.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vj.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rb.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ql.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cv.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uh.yuexingan06.cn


<!-- 参考信息 -->