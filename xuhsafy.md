代发 wailian999

TS:   console.assert(x > 0);
来源：http://hd.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://nz.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lr.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lc.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://ui.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://an.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://ah.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://im.szxytkj.cn

JS:   e.message;  e.stack
来源：http://kg.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jx.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sb.gzmigu.cn

Go:   err.Error()
来源：http://ho.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://tf.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://of.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ve.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kx.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cp.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zt.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ds.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tk.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://un.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vi.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yz.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://ps.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mj.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zg.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://er.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kt.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hu.szxytkj.cn

Go:   defer f.Close()
来源：http://vl.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iq.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://te.jctech888.com.cn

================================================================================
来源：http://po.gzmigu.cn

I. 正则表达式
来源：http://bi.521024.cn

================================================================================
来源：http://dd.bjjhwx.cn

[I01] 判断是否匹配
来源：http://rd.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ny.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://is.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://ie.szsharing.cn

TS:   /\d+/.test(s)
来源：http://tr.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pw.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wi.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://bf.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rm.lnxyls.cn

[I02] 提取所有匹配
来源：http://ax.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://py.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wj.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iy.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://zn.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ak.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rv.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://hl.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nu.huanxung.cn

[I03] 提取捕获分组
来源：http://wh.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ya.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://be.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ws.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lx.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ib.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jz.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mo.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tg.lnxyls.cn

[I04] 正则替换
来源：http://sd.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bb.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://de.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rk.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xa.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wf.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jy.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gj.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kq.colortex.cn

[I05] 按正则拆分
来源：http://wy.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cy.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jz.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://sz.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://xi.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ff.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tr.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fr.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nc.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lc.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lc.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rs.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gq.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ie.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://je.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vs.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oz.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://jq.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ba.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sy.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fm.jianghongdianzi.cn

TS:   /error/gim
来源：http://km.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ip.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wx.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://lb.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yz.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://sc.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xp.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ad.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mu.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fl.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hp.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oa.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hf.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rc.hnjuh.cn

================================================================================
来源：http://xh.bookmarksfly.cn

J. 日期与时间
来源：http://ji.yuexingan06.cn

================================================================================
来源：http://dl.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://zg.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://na.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ut.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ai.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://cq.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ru.panjiajie.cn

Go:   time.Now()
来源：http://mu.colortex.cn

Ruby: Time.now
来源：http://yc.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ol.szxytkj.cn

[J02] 格式化输出
来源：http://ma.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://va.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cl.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ok.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://zx.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cq.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nl.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://md.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://sm.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ox.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dr.521024.cn

JS:   new Date("2024-01-02")
来源：http://gk.asd995.cn

TS:   new Date("2024-01-02")
来源：http://nd.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nt.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tg.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ol.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pc.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://jr.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bm.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uy.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lf.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tb.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ch.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rl.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uw.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pl.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://ie.colortex.cn

Py:   now + timedelta(days=7)
来源：http://gg.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bx.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vw.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://np.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://zt.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fd.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://nl.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ie.chemitech.net.cn

[J06] 计算两时间之差
来源：http://jx.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://uz.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://il.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ue.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mb.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://qj.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://ra.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ws.bjjhwx.cn

[J07] 比较两个日期
来源：http://ud.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://bz.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hc.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://re.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://du.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zw.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xn.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ek.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://it.gzmigu.cn

[J08] 提取年月日与星期
来源：http://kf.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gi.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ln.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ag.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ej.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qu.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tn.wgjwhj.cn

[J09] 时区处理
来源：http://tj.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rm.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rr.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gu.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nh.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wy.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dr.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hw.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oy.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://ee.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wy.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hs.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qg.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ds.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rn.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sz.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sc.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ri.huixiangedu.cn

================================================================================
来源：http://rx.nicolike.cn

K. JSON 与序列化
来源：http://ty.yuntaijiaju.cn

================================================================================
来源：http://ok.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://gn.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wz.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.asd995.cn

JS:   JSON.stringify(obj)
来源：http://qy.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://lp.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gj.9csxet.cn

Go:   json.Marshal(obj)
来源：http://gw.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fh.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tx.newstarts.cn

[K02] JSON 字符串转对象
来源：http://zz.chemitech.net.cn

Py:   json.loads(s)
来源：http://cc.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wj.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://xp.hnjuh.cn

TS:   JSON.parse(s)
来源：http://xz.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xh.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://an.hahajie.cn

Ruby: JSON.parse(s)
来源：http://zc.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nv.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://ob.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://od.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vn.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lr.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iy.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ll.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://en.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zh.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ga.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://cw.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ph.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qi.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wc.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zu.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zr.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ll.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hg.colortex.cn

[K05] 深拷贝对象
来源：http://wt.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://vo.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://ye.hahajie.cn

JS:   structuredClone(obj)
来源：http://wd.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ip.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yl.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gd.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qu.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wy.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://rq.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ms.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wd.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qn.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://up.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ni.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bm.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fs.colortex.cn

[K07] 进制转换
来源：http://sc.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ni.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mq.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nh.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ig.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yq.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://av.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nw.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://go.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://xh.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://ca.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zt.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://kn.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://rl.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://io.szsharing.cn

Go:   encoding/gob
来源：http://mf.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://kx.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kt.521024.cn

================================================================================
来源：http://zw.muxihuayi.cn

L. 网络请求
来源：http://dl.9csxet.cn

================================================================================
来源：http://iy.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://eo.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ak.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rb.shxzskj.cn

JS:   await fetch(url)
来源：http://kd.wgjwhj.cn

TS:   await fetch(url)
来源：http://dy.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ss.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://fs.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kn.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zo.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://pd.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hl.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://un.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nr.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lm.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qd.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qs.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tg.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yn.gzmigu.cn

[L03] 设置自定义请求头
来源：http://vk.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nd.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vm.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sc.lnxyls.cn


<!-- 参考信息 -->