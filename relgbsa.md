代发 wailian999

[H07] 断言
来源：http://ym.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://iv.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://xp.9csxet.cn

JS:   console.assert(x > 0);
来源：http://rz.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://dx.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://fv.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ca.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eg.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://dz.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://py.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://tz.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://co.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://zu.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xv.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kr.yuntaijiaju.cn

Go:   err.Error()
来源：http://wk.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://bg.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yb.newstarts.cn

[H09] 带错误码的异常
来源：http://cu.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tv.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xq.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ix.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pi.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ug.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mn.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oj.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yl.muxihuayi.cn

[H10] 资源自动释放
来源：http://rd.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qf.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zh.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ak.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xw.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ha.huixiangedu.cn

Go:   defer f.Close()
来源：http://ch.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://my.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vr.asd995.cn

================================================================================
来源：http://je.521024.cn

I. 正则表达式
来源：http://tx.yuexingan06.cn

================================================================================
来源：http://nq.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://dc.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vg.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hi.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://pn.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://cu.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://au.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bb.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://ct.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cs.lnxyls.cn

[I02] 提取所有匹配
来源：http://la.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://fm.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mb.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xc.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ek.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fg.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qh.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://md.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tb.newstarts.cn

[I03] 提取捕获分组
来源：http://eb.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bq.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://he.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xs.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uj.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ck.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sh.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rg.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cy.huixinmuqiang.cn

[I04] 正则替换
来源：http://aw.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zx.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pn.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hr.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xh.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ep.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ip.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yu.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zp.wgjwhj.cn

[I05] 按正则拆分
来源：http://zf.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xr.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ie.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://df.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://wo.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fl.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ef.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lh.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vv.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ho.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sw.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://om.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ms.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zz.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vs.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eb.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uj.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ja.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wv.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ig.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sc.hnjuh.cn

TS:   /error/gim
来源：http://zy.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qh.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://an.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://aq.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xm.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zu.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://er.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uj.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hl.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yj.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zk.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yz.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nc.hahajie.cn

================================================================================
来源：http://vr.gzmigu.cn

J. 日期与时间
来源：http://jo.hnjuh.cn

================================================================================
来源：http://du.szsharing.cn

[J01] 获取当前时间
来源：http://ms.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ub.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wb.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://xm.9csxet.cn

TS:   new Date();  Date.now()
来源：http://he.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qg.haigaiapp.cn

Go:   time.Now()
来源：http://ow.shxzukj.cn

Ruby: Time.now
来源：http://zo.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lz.bookmarksfly.cn

[J02] 格式化输出
来源：http://ny.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://af.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zr.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://be.9csxet.cn

TS:   d.toISOString()
来源：http://qb.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://he.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sx.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eq.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oo.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ho.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lt.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vt.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://re.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://po.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vq.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wx.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://ov.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vj.asd995.cn

[J04] 时间戳与日期互转
来源：http://ao.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uy.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ru.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hc.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kq.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tr.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xp.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qo.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hb.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://mz.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://uj.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vc.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mv.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fo.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://nc.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sc.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://lf.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wi.nszjky.cn

[J06] 计算两时间之差
来源：http://nj.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://us.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://qt.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aj.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ll.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://uc.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://pn.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://pz.jctech888.com.cn

[J07] 比较两个日期
来源：http://db.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://mm.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://go.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://md.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ca.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fr.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tk.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bn.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://gf.nszjky.cn

[J08] 提取年月日与星期
来源：http://uu.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xh.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zu.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xx.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nt.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tz.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wy.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hr.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cv.hnjuh.cn

[J09] 时区处理
来源：http://ed.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wq.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xy.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hg.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pd.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hc.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pi.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ai.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://gv.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ud.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tj.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ls.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mj.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bn.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ef.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://no.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xt.nszjky.cn

================================================================================
来源：http://wc.shxzukj.cn

K. JSON 与序列化
来源：http://sa.asd995.cn

================================================================================
来源：http://uk.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ut.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ro.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gs.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://jt.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://sy.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ma.colortex.cn

Go:   json.Marshal(obj)
来源：http://hg.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yz.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cf.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://ve.521024.cn

Py:   json.loads(s)
来源：http://ps.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aw.9csxet.cn

JS:   JSON.parse(s)
来源：http://pe.hnjuh.cn

TS:   JSON.parse(s)
来源：http://ni.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qi.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mw.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://yl.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xy.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pq.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mx.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ht.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lr.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zg.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pe.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ke.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ux.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://xa.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fn.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://di.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ot.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ac.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rx.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wk.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rk.jctech888.com.cn

[K05] 深拷贝对象
来源：http://is.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://hj.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://wt.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://gt.nicolike.cn

TS:   structuredClone(obj)
来源：http://xi.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xo.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dr.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rx.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vv.szsharing.cn

[K06] 解析 URL 查询串
来源：http://df.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ev.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zk.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vm.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ak.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vd.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sm.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pl.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pf.hahajie.cn

[K07] 进制转换
来源：http://al.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ay.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aw.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vo.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tc.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hb.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zi.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://da.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://qi.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://qo.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://of.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ta.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ft.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ad.nszjky.cn

Go:   encoding/gob
来源：http://fh.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://cj.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jh.lnxyls.cn

================================================================================
来源：http://dc.szxytkj.cn

L. 网络请求
来源：http://uo.newstarts.cn

================================================================================
来源：http://vi.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://qe.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oc.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xp.9csxet.cn

JS:   await fetch(url)
来源：http://ao.newstarts.cn

TS:   await fetch(url)
来源：http://wb.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hb.521024.cn

Go:   resp, err := http.Get(url)
来源：http://xa.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yb.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://it.9csxet.cn

[L02] 发送 POST JSON
来源：http://ap.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yo.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qj.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sc.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jg.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://au.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qb.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fi.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ob.gzmigu.cn


<!-- 参考信息 -->