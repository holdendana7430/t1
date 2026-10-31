代发 wailian999

TS:   console.assert(x > 0);
来源：http://dp.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ep.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fb.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xe.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://xo.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://wk.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://vb.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kl.521024.cn

JS:   e.message;  e.stack
来源：http://on.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wu.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ax.521024.cn

Go:   err.Error()
来源：http://xk.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://dm.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://jr.huanxung.cn

[H09] 带错误码的异常
来源：http://wo.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vu.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://le.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rq.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ly.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uz.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fv.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ca.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jw.nszjky.cn

[H10] 资源自动释放
来源：http://fe.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vk.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bp.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pf.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dg.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qt.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://ag.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xi.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://it.chemitech.net.cn

================================================================================
来源：http://sa.yuntaijiaju.cn

I. 正则表达式
来源：http://ke.yuexingan06.cn

================================================================================
来源：http://qp.gzmigu.cn

[I01] 判断是否匹配
来源：http://sb.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fe.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bf.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://gx.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://tp.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fc.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wx.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://kx.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yu.muxihuayi.cn

[I02] 提取所有匹配
来源：http://fe.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://mf.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ks.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tz.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://qy.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yy.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rx.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://an.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://us.yuexingan06.cn

[I03] 提取捕获分组
来源：http://os.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xc.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wg.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wa.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://af.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zv.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zu.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ja.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zx.bjjhwx.cn

[I04] 正则替换
来源：http://he.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kv.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dx.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://di.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lt.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jb.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ss.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aw.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://ok.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pg.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xp.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://jg.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://vv.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ae.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ag.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pc.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qn.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cm.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ty.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ry.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vw.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vc.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bx.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ha.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ip.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fb.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://kq.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bg.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hd.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aa.jctech888.com.cn

TS:   /error/gim
来源：http://by.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fj.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ex.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://tp.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ik.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rd.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mb.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tg.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wi.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gb.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xr.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uu.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ov.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dp.huixiangedu.cn

================================================================================
来源：http://ev.nicolike.cn

J. 日期与时间
来源：http://mf.colortex.cn

================================================================================
来源：http://xi.colortex.cn

[J01] 获取当前时间
来源：http://la.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dg.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sw.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://gr.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://ku.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tb.newstarts.cn

Go:   time.Now()
来源：http://hl.gzmigu.cn

Ruby: Time.now
来源：http://ku.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oj.yuexingan06.cn

[J02] 格式化输出
来源：http://pm.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yu.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cs.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kp.yuexingan06.cn

TS:   d.toISOString()
来源：http://lh.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://td.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qr.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://on.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nw.huanxung.cn

[J03] 字符串解析为日期
来源：http://bh.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ik.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yu.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://px.521024.cn

TS:   new Date("2024-01-02")
来源：http://no.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ah.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zc.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://zm.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vk.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://fx.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dj.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ud.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://my.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://th.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yb.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cd.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iv.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hc.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://vv.521024.cn

Py:   now + timedelta(days=7)
来源：http://li.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cq.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cd.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rn.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ul.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lv.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://cj.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pq.nicolike.cn

[J06] 计算两时间之差
来源：http://qo.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://ug.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ea.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kc.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dn.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dn.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://ph.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://xe.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://wm.yuexingan06.cn

[J07] 比较两个日期
来源：http://uz.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://sp.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kv.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xu.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qt.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://me.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ov.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ca.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://qt.9csxet.cn

[J08] 提取年月日与星期
来源：http://fw.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lp.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://re.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lx.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vs.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gr.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://av.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ve.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wp.hnjuh.cn

[J09] 时区处理
来源：http://uj.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gh.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ir.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gx.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ak.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://va.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cq.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lr.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ph.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ms.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ep.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://op.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gb.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vb.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://op.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://md.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rb.nicolike.cn

================================================================================
来源：http://pk.bookmarksfly.cn

K. JSON 与序列化
来源：http://hd.panjiajie.cn

================================================================================
来源：http://qh.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://lj.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fx.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xn.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://gr.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://aw.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jp.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://xd.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bs.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dk.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://ro.haigaiapp.cn

Py:   json.loads(s)
来源：http://yg.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iy.lnxyls.cn

JS:   JSON.parse(s)
来源：http://od.hnjuh.cn

TS:   JSON.parse(s)
来源：http://vp.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pz.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://qu.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://tb.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uq.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ps.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dw.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fm.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nd.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uf.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zf.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hm.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kz.nicolike.cn

[K04] 读取 JSON 文件
来源：http://jt.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gh.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kz.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cy.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bk.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qi.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tf.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wk.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jc.newstarts.cn

[K05] 深拷贝对象
来源：http://nq.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://cq.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://uh.shxzskj.cn

JS:   structuredClone(obj)
来源：http://vr.huanxung.cn

TS:   structuredClone(obj)
来源：http://fx.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ce.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ze.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eb.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gd.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://fe.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ti.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qn.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kb.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wh.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://td.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wb.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vr.hahajie.cn

[K07] 进制转换
来源：http://dc.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uj.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sc.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rs.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ej.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://do.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nl.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sh.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gh.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://zl.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://am.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dc.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://nq.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://hg.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pr.jianghongdianzi.cn

Go:   encoding/gob
来源：http://fm.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://zs.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://on.yuexingan06.cn

================================================================================
来源：http://zv.hnjuh.cn

L. 网络请求
来源：http://fe.shxzukj.cn

================================================================================
来源：http://lu.huanxung.cn

[L01] 发送 GET 请求
来源：http://uc.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fe.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qk.shxzskj.cn

JS:   await fetch(url)
来源：http://lj.panjiajie.cn

TS:   await fetch(url)
来源：http://qk.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ly.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://us.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jv.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mr.asd995.cn

[L02] 发送 POST JSON
来源：http://ji.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xq.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mz.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mq.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yi.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ws.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tk.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ms.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dr.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ip.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://md.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hr.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lo.huanxung.cn


<!-- 参考信息 -->