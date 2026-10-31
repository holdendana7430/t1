代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://qo.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://xa.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://cg.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://da.szsharing.cn

JS:   e.message;  e.stack
来源：http://gx.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yt.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ga.shtwfgs.cn

Go:   err.Error()
来源：http://gq.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://gl.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://in.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ms.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://al.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wp.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nb.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fh.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ka.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fg.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://am.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jr.yuexingan06.cn

[H10] 资源自动释放
来源：http://wb.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qv.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ua.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tc.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ol.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ro.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://lo.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qb.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kq.wgjwhj.cn

================================================================================
来源：http://nn.colortex.cn

I. 正则表达式
来源：http://mg.jctech888.com.cn

================================================================================
来源：http://iy.bjjhwx.cn

[I01] 判断是否匹配
来源：http://no.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jj.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zw.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://qr.newstarts.cn

TS:   /\d+/.test(s)
来源：http://py.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oe.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pq.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ez.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tf.shxzskj.cn

[I02] 提取所有匹配
来源：http://le.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://hg.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gs.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vn.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://jq.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hh.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://er.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ab.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cr.panjiajie.cn

[I03] 提取捕获分组
来源：http://fd.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fi.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fk.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cj.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vn.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ae.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tb.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xu.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qo.shtwfgs.cn

[I04] 正则替换
来源：http://rs.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fm.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kp.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gm.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ry.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fm.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ap.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dp.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vk.shtwfgs.cn

[I05] 按正则拆分
来源：http://re.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oh.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://an.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://dp.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://uk.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xj.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wl.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wb.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uf.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sv.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xk.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://in.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://if.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kl.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dt.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zi.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://tk.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ag.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mf.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nf.lnxyls.cn

TS:   /error/gim
来源：http://hf.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hb.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qu.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://nc.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oh.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://ea.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hi.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lr.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lr.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jy.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pc.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sc.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qc.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://md.bjjhwx.cn

================================================================================
来源：http://fe.huanxung.cn

J. 日期与时间
来源：http://yh.panjiajie.cn

================================================================================
来源：http://ol.bookmarksfly.cn

[J01] 获取当前时间
来源：http://dr.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pq.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cm.huanxung.cn

JS:   new Date();  Date.now()
来源：http://ez.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://gk.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gc.nszjky.cn

Go:   time.Now()
来源：http://te.szsharing.cn

Ruby: Time.now
来源：http://xn.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jh.newstarts.cn

[J02] 格式化输出
来源：http://zf.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://do.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cb.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dj.huanxung.cn

TS:   d.toISOString()
来源：http://zu.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kl.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xt.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eh.panjiajie.cn

[J03] 字符串解析为日期
来源：http://pj.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mf.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ry.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://le.asd995.cn

TS:   new Date("2024-01-02")
来源：http://qa.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mx.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vf.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://lp.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pi.nicolike.cn

[J04] 时间戳与日期互转
来源：http://mv.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yn.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ug.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vq.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yz.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vw.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sj.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lr.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cg.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://wa.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://cg.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lk.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yb.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yg.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://eh.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zx.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://jl.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sq.9csxet.cn

[J06] 计算两时间之差
来源：http://vt.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://cx.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://tl.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fo.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gx.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qq.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://lp.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://xf.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://am.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://bn.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ye.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fy.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qh.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bd.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jz.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kk.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://av.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://lm.shxzskj.cn

[J08] 提取年月日与星期
来源：http://ee.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dj.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zw.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jy.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ci.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ku.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jv.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wn.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kb.hahajie.cn

[J09] 时区处理
来源：http://za.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://af.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fv.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kc.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wg.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bt.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qa.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dg.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fw.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://hn.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cx.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ne.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sg.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zi.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mo.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lv.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xl.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yu.haigaiapp.cn

================================================================================
来源：http://un.asd995.cn

K. JSON 与序列化
来源：http://rh.bookmarksfly.cn

================================================================================
来源：http://io.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://cv.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ds.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hr.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://wi.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://gb.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fs.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://xd.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vd.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iw.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ei.521024.cn

Py:   json.loads(s)
来源：http://nz.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nj.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://um.panjiajie.cn

TS:   JSON.parse(s)
来源：http://de.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ze.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://su.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://ky.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mn.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://nl.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eb.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jk.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qj.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rj.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rd.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pe.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dg.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ws.asd995.cn

[K04] 读取 JSON 文件
来源：http://jn.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cg.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qo.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rq.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://to.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wz.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qk.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ae.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hj.shxzukj.cn

[K05] 深拷贝对象
来源：http://tu.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://qg.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://el.hahajie.cn

JS:   structuredClone(obj)
来源：http://un.521024.cn

TS:   structuredClone(obj)
来源：http://bh.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xb.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ti.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ir.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fx.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://pn.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yj.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://js.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ha.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qw.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zv.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mm.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nq.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hp.chemitech.net.cn

[K07] 进制转换
来源：http://rh.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ge.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zi.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zs.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uv.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uy.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ls.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pw.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://oi.521024.cn

Py:   pickle.dumps(obj)
来源：http://ae.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qz.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bs.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tn.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dq.jianghongdianzi.cn

Go:   encoding/gob
来源：http://io.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ds.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qo.huixiangedu.cn

================================================================================
来源：http://hh.shxzukj.cn

L. 网络请求
来源：http://yb.lnxyls.cn

================================================================================
来源：http://en.asd995.cn

[L01] 发送 GET 请求
来源：http://pv.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cz.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://io.muxihuayi.cn

JS:   await fetch(url)
来源：http://vx.jctech888.com.cn

TS:   await fetch(url)
来源：http://jy.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wh.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://wk.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hb.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ld.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://ih.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xu.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hk.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mo.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vw.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zu.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wa.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ir.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zv.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://fd.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lg.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ma.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sw.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lq.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fj.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ks.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ym.9csxet.cn


<!-- 参考信息 -->