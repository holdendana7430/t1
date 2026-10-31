代发 wailian999

[H07] 断言
来源：http://ri.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://bp.lnxyls.cn

PHP:  assert($x > 0);
来源：http://rf.nszjky.cn

JS:   console.assert(x > 0);
来源：http://jf.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://ft.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://ix.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bc.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ap.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://oe.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://xo.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://gc.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iw.nicolike.cn

JS:   e.message;  e.stack
来源：http://ea.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lp.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ms.bookmarksfly.cn

Go:   err.Error()
来源：http://rs.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://ez.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://lh.shtwfgs.cn

[H09] 带错误码的异常
来源：http://rg.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mt.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hb.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zl.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vs.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yc.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://va.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ce.haigaiapp.cn

[H10] 资源自动释放
来源：http://pj.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ta.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lt.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ip.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ba.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xf.nicolike.cn

Go:   defer f.Close()
来源：http://ws.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nm.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zp.lnxyls.cn

================================================================================
来源：http://mg.yuexingan06.cn

I. 正则表达式
来源：http://ri.shtwfgs.cn

================================================================================
来源：http://ac.wgjwhj.cn

[I01] 判断是否匹配
来源：http://wu.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fs.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jt.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://qs.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://at.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aw.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bb.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://gz.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://is.szsharing.cn

[I02] 提取所有匹配
来源：http://bu.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://kb.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kp.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://km.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://qj.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jk.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uy.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://eb.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lg.szsharing.cn

[I03] 提取捕获分组
来源：http://gh.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yx.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://io.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mz.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bn.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lx.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zy.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://im.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mh.chemitech.net.cn

[I04] 正则替换
来源：http://vv.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://re.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wo.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://by.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zj.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zv.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qu.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sd.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fn.shxzskj.cn

[I05] 按正则拆分
来源：http://yg.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uv.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pm.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://nr.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://vu.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://wp.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vu.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rh.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lu.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zr.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zf.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hm.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sn.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ca.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bh.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xh.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ly.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://sc.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jd.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ws.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cb.haigaiapp.cn

TS:   /error/gim
来源：http://gd.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sx.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qh.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://qk.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cc.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://hw.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oy.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wc.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pt.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rt.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qu.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hn.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hx.muxihuayi.cn

================================================================================
来源：http://jr.bjjhwx.cn

J. 日期与时间
来源：http://ap.shxzskj.cn

================================================================================
来源：http://jz.shxzukj.cn

[J01] 获取当前时间
来源：http://ar.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wo.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yn.huanxung.cn

JS:   new Date();  Date.now()
来源：http://in.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://zb.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hr.muxihuayi.cn

Go:   time.Now()
来源：http://ll.jianghongdianzi.cn

Ruby: Time.now
来源：http://sj.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kw.9csxet.cn

[J02] 格式化输出
来源：http://ax.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jk.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hf.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://id.9csxet.cn

TS:   d.toISOString()
来源：http://oj.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pj.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aq.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ke.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vw.huanxung.cn

[J03] 字符串解析为日期
来源：http://tw.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mg.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://op.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://pu.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://sn.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tr.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ac.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://xc.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yi.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://mn.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zi.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hw.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wh.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fr.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yg.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sh.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yw.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ff.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ko.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://ez.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://js.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ij.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hi.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://rl.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kr.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://mj.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ly.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://tz.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://em.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://xs.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dx.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ay.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tk.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://xr.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ns.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://rc.panjiajie.cn

[J07] 比较两个日期
来源：http://bm.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qe.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kj.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xc.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lq.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jf.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ve.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://cc.newstarts.cn

[J08] 提取年月日与星期
来源：http://kt.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nz.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dg.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tg.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bt.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://us.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kl.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nz.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cz.newstarts.cn

[J09] 时区处理
来源：http://dj.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nb.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zx.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gv.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kh.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ep.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wo.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ks.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://sj.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bj.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cx.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ri.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aj.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pf.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ew.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://px.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jl.hahajie.cn

================================================================================
来源：http://wg.newstarts.cn

K. JSON 与序列化
来源：http://qf.521024.cn

================================================================================
来源：http://wo.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://lw.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mn.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iw.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://jv.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://lz.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wu.szsharing.cn

Go:   json.Marshal(obj)
来源：http://cq.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xo.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://dh.shxzskj.cn

Py:   json.loads(s)
来源：http://db.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ah.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://sb.szsharing.cn

TS:   JSON.parse(s)
来源：http://nn.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dg.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://hx.521024.cn

Ruby: JSON.parse(s)
来源：http://hc.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bx.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ux.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://np.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cl.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sw.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jq.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qj.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gs.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://be.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zi.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ih.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hy.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dk.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xc.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mn.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nh.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vz.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qq.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jx.newstarts.cn

[K05] 深拷贝对象
来源：http://xf.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://uq.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://hz.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://so.9csxet.cn

TS:   structuredClone(obj)
来源：http://ou.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sj.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lh.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wl.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://un.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://ko.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ar.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cb.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gy.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fr.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yv.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oi.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kb.shxzukj.cn

[K07] 进制转换
来源：http://ul.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://io.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fn.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ne.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ie.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ui.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jo.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hq.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ny.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://mb.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://tu.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ag.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://hn.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://rc.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ld.panjiajie.cn

Go:   encoding/gob
来源：http://nm.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://hm.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fw.szxytkj.cn

================================================================================
来源：http://io.jctech888.com.cn

L. 网络请求
来源：http://tz.wgjwhj.cn

================================================================================
来源：http://vl.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://ay.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cg.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wr.shxzukj.cn

JS:   await fetch(url)
来源：http://is.chemitech.net.cn

TS:   await fetch(url)
来源：http://tm.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lv.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://up.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gu.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gm.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://hb.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pz.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://np.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://er.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pw.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fl.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rs.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cw.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vw.shtwfgs.cn


<!-- 参考信息 -->