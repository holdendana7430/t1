代发 wailian999

[H07] 断言
来源：http://cn.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://uw.gzmigu.cn

PHP:  assert($x > 0);
来源：http://wm.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ml.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://vi.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://uv.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vp.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yq.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://ht.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://rv.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://zg.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://af.hnjuh.cn

JS:   e.message;  e.stack
来源：http://mi.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rg.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ir.hahajie.cn

Go:   err.Error()
来源：http://ks.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://yk.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://jx.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://rl.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ee.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yg.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nr.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ed.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vg.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pa.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zw.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wr.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://vn.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ih.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://py.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://am.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ea.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fp.chemitech.net.cn

Go:   defer f.Close()
来源：http://ks.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kw.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tf.bjjhwx.cn

================================================================================
来源：http://cq.9csxet.cn

I. 正则表达式
来源：http://cn.huanxung.cn

================================================================================
来源：http://fj.wgjwhj.cn

[I01] 判断是否匹配
来源：http://ab.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fh.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://po.hahajie.cn

JS:   /\d+/.test(s)
来源：http://vs.newstarts.cn

TS:   /\d+/.test(s)
来源：http://mg.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ql.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jg.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://gh.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zi.panjiajie.cn

[I02] 提取所有匹配
来源：http://ez.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://fc.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mk.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lq.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://cl.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xe.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wq.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://io.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vs.jctech888.com.cn

[I03] 提取捕获分组
来源：http://tr.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://va.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xe.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oq.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iy.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eq.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vz.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dn.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ll.panjiajie.cn

[I04] 正则替换
来源：http://hp.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gq.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zf.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hh.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ma.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rh.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bx.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eg.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cl.newstarts.cn

[I05] 按正则拆分
来源：http://jq.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xd.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://si.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://rc.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://wt.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://rt.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dt.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rt.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xg.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qr.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ec.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ey.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ck.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yc.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oj.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ze.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tn.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xr.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://le.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ae.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wy.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iu.jianghongdianzi.cn

TS:   /error/gim
来源：http://jq.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yt.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tk.521024.cn

Ruby: s.scan(/error/i)
来源：http://cx.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ik.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ta.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yi.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jj.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xl.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://md.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ww.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tx.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fk.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://en.newstarts.cn

================================================================================
来源：http://hr.haigaiapp.cn

J. 日期与时间
来源：http://cx.shtwfgs.cn

================================================================================
来源：http://gh.yuexingan06.cn

[J01] 获取当前时间
来源：http://xr.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lg.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xc.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://gx.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://mm.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ac.huixiangedu.cn

Go:   time.Now()
来源：http://xz.szxytkj.cn

Ruby: Time.now
来源：http://wz.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eb.nszjky.cn

[J02] 格式化输出
来源：http://yx.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://no.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.chemitech.net.cn

TS:   d.toISOString()
来源：http://th.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hh.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://px.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hm.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wp.hnjuh.cn

[J03] 字符串解析为日期
来源：http://nw.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gx.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nf.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://bv.521024.cn

TS:   new Date("2024-01-02")
来源：http://yt.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://it.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ds.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://yt.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kn.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ey.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ni.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kc.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hj.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jo.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mq.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://et.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yn.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ui.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://ny.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://re.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ke.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xp.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ht.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://ie.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ji.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://kv.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vb.huixiangedu.cn

[J06] 计算两时间之差
来源：http://vj.521024.cn

Py:   (end - start).total_seconds()
来源：http://dm.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://nc.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gg.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ny.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gf.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://pj.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://zn.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://el.wgjwhj.cn

[J07] 比较两个日期
来源：http://oo.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://se.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iw.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tl.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nu.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ho.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yz.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bd.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://zg.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://dj.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vj.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qa.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cw.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qc.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tq.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bi.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://io.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fq.wgjwhj.cn

[J09] 时区处理
来源：http://qw.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uj.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sv.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cz.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zi.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hv.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ti.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://he.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://bo.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cy.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ew.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oz.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xx.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mq.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mw.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oz.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://md.bjjhwx.cn

================================================================================
来源：http://wd.wgjwhj.cn

K. JSON 与序列化
来源：http://uc.shtwfgs.cn

================================================================================
来源：http://ba.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://pv.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://my.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://en.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ic.asd995.cn

TS:   JSON.stringify(obj)
来源：http://dk.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xx.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://ni.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gd.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aj.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://to.hahajie.cn

Py:   json.loads(s)
来源：http://uw.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ii.521024.cn

JS:   JSON.parse(s)
来源：http://nx.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://gk.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hx.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://su.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://zn.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hw.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://uf.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vy.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eg.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zt.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zk.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nv.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zd.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zi.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uz.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://bi.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yn.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uj.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nt.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://km.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fz.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nz.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://av.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pa.asd995.cn

[K05] 深拷贝对象
来源：http://go.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ff.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://dr.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ir.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://ng.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hu.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zt.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hh.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ae.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://hs.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rh.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xv.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gg.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ir.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ml.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://np.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tj.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ld.shxzukj.cn

[K07] 进制转换
来源：http://tm.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://et.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rz.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yf.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yz.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wf.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dz.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://te.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://cc.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://gb.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kf.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://lv.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://dd.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rd.huixinmuqiang.cn

Go:   encoding/gob
来源：http://wg.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://zp.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hr.bjjhwx.cn

================================================================================
来源：http://lh.huixinmuqiang.cn

L. 网络请求
来源：http://bm.yuexingan06.cn

================================================================================
来源：http://lr.lnxyls.cn

[L01] 发送 GET 请求
来源：http://jk.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lf.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tt.nszjky.cn

JS:   await fetch(url)
来源：http://vd.wgjwhj.cn

TS:   await fetch(url)
来源：http://tj.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ee.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://uv.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bl.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ln.szsharing.cn

[L02] 发送 POST JSON
来源：http://fe.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bh.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tu.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ad.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vg.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zc.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xo.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cb.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qd.szxytkj.cn


<!-- 参考信息 -->