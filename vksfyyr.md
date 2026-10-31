代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://mj.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://is.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://go.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dh.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://gq.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hs.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ah.newstarts.cn

Go:   err.Error()
来源：http://zy.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://di.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://al.colortex.cn

[H09] 带错误码的异常
来源：http://fh.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mg.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tw.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://av.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uv.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nk.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://py.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://og.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oh.panjiajie.cn

[H10] 资源自动释放
来源：http://gs.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fy.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zt.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jt.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mq.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://so.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://do.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xv.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ln.wgjwhj.cn

================================================================================
来源：http://gy.shtwfgs.cn

I. 正则表达式
来源：http://km.muxihuayi.cn

================================================================================
来源：http://qx.gzmigu.cn

[I01] 判断是否匹配
来源：http://kl.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gx.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ks.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://su.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://uz.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xg.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yi.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://hu.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ag.shxzukj.cn

[I02] 提取所有匹配
来源：http://vt.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://kp.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yd.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tp.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://du.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tt.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vf.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://xw.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kt.shtwfgs.cn

[I03] 提取捕获分组
来源：http://jx.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tg.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xo.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xy.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://el.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://al.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ja.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mx.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fo.muxihuayi.cn

[I04] 正则替换
来源：http://vy.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bn.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://an.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fs.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rr.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pg.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sz.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qx.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ii.newstarts.cn

[I05] 按正则拆分
来源：http://va.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hg.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hr.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://fp.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://nn.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://wx.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ow.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bf.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sg.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gr.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cr.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://um.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nu.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tf.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aj.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yv.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://da.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://he.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fo.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lu.nszjky.cn

TS:   /error/gim
来源：http://pf.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ex.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ww.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://sv.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://of.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://oy.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mc.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xy.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rg.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vw.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aj.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mf.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fo.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://by.colortex.cn

================================================================================
来源：http://zm.lnxyls.cn

J. 日期与时间
来源：http://zs.shxzskj.cn

================================================================================
来源：http://eq.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://in.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mn.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yp.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://rq.asd995.cn

TS:   new Date();  Date.now()
来源：http://yz.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ds.shxzukj.cn

Go:   time.Now()
来源：http://hn.jctech888.com.cn

Ruby: Time.now
来源：http://ot.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uh.gzmigu.cn

[J02] 格式化输出
来源：http://yv.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yt.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aw.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bj.nszjky.cn

TS:   d.toISOString()
来源：http://hv.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nk.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yd.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dp.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hc.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://tt.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cx.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kr.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://mu.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://dt.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yt.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ig.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://md.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sx.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://oe.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vf.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bh.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kq.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://as.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aj.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ql.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ae.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yp.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ps.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://mi.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rd.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ub.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://zs.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rr.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://fd.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xj.521024.cn

[J06] 计算两时间之差
来源：http://uv.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://er.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://zi.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pe.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yw.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ct.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://ox.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://so.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://km.szxytkj.cn

[J07] 比较两个日期
来源：http://ze.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://fr.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cd.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ob.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yl.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mk.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zo.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cu.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://gw.szxytkj.cn

[J08] 提取年月日与星期
来源：http://kp.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fb.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rs.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ob.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ej.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yd.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ao.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mx.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tb.asd995.cn

[J09] 时区处理
来源：http://as.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gw.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://so.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://le.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ed.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rl.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pw.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pr.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qo.521024.cn

[J10] 取今天 / 本月第一天
来源：http://jz.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oe.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yd.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vw.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ds.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mq.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xz.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hk.muxihuayi.cn

================================================================================
来源：http://ag.hnjuh.cn

K. JSON 与序列化
来源：http://wz.shtwfgs.cn

================================================================================
来源：http://hj.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://on.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nt.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nf.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://db.521024.cn

TS:   JSON.stringify(obj)
来源：http://xu.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yp.hahajie.cn

Go:   json.Marshal(obj)
来源：http://kg.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vw.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ns.asd995.cn

[K02] JSON 字符串转对象
来源：http://mf.shtwfgs.cn

Py:   json.loads(s)
来源：http://uw.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tm.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://mh.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ae.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zb.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://jr.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ub.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ji.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://js.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qm.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ea.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lc.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gf.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bu.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cv.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wr.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pz.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://rl.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zd.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bv.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iu.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jt.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nx.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cq.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ke.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gh.szxytkj.cn

[K05] 深拷贝对象
来源：http://eb.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://bu.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://im.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://hq.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ka.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://va.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xd.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jf.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ax.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ex.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oh.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ez.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kw.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://at.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ay.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://el.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zp.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zw.panjiajie.cn

[K07] 进制转换
来源：http://nk.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zd.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ws.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cr.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tz.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ex.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wg.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xt.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lo.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://kg.asd995.cn

Py:   pickle.dumps(obj)
来源：http://ps.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vc.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ix.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://nv.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gh.szsharing.cn

Go:   encoding/gob
来源：http://zj.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ji.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lk.521024.cn

================================================================================
来源：http://hf.bookmarksfly.cn

L. 网络请求
来源：http://tu.newstarts.cn

================================================================================
来源：http://gg.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://pm.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gh.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sy.gzmigu.cn

JS:   await fetch(url)
来源：http://yi.colortex.cn

TS:   await fetch(url)
来源：http://kl.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wl.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ma.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ne.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cd.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://xh.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://id.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ya.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tl.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zb.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cv.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qv.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xz.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xq.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://up.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wd.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hl.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zg.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://de.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sb.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tn.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ad.shtwfgs.cn


<!-- 参考信息 -->