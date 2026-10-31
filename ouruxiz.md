代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://mx.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://vo.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://ff.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gj.521024.cn

JS:   e.message;  e.stack
来源：http://qd.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gb.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wi.yuntaijiaju.cn

Go:   err.Error()
来源：http://eh.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://dn.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://wx.jctech888.com.cn

[H09] 带错误码的异常
来源：http://ys.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fs.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ec.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kp.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kb.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ul.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rh.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://js.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dn.colortex.cn

[H10] 资源自动释放
来源：http://as.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ma.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wd.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ik.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gr.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tp.shxzskj.cn

Go:   defer f.Close()
来源：http://qj.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kn.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vo.haigaiapp.cn

================================================================================
来源：http://rk.chemitech.net.cn

I. 正则表达式
来源：http://zg.gzmigu.cn

================================================================================
来源：http://xa.wgjwhj.cn

[I01] 判断是否匹配
来源：http://br.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://su.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tj.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://zn.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://ul.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fs.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jc.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://br.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xo.nszjky.cn

[I02] 提取所有匹配
来源：http://ex.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://ux.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cg.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vi.asd995.cn

TS:   s.match(/\d+/g)
来源：http://df.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xy.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://pi.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mc.shxzskj.cn

[I03] 提取捕获分组
来源：http://ug.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bv.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sb.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tc.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yw.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lv.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xh.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cf.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ed.gzmigu.cn

[I04] 正则替换
来源：http://zk.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uf.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fx.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rm.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pw.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jn.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xf.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zo.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ev.asd995.cn

[I05] 按正则拆分
来源：http://uc.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hj.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zq.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ns.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ed.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dj.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oq.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yj.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://po.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://it.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://li.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ze.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xk.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wx.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fe.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://py.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://ku.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://so.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xq.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qs.gzmigu.cn

TS:   /error/gim
来源：http://mg.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xx.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ru.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://ka.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gv.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ef.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yr.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qe.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ur.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ek.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tn.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bn.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rp.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://he.bjjhwx.cn

================================================================================
来源：http://ow.bjjhwx.cn

J. 日期与时间
来源：http://hv.nszjky.cn

================================================================================
来源：http://rg.bjjhwx.cn

[J01] 获取当前时间
来源：http://tj.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tw.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xe.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://ad.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ak.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wx.jctech888.com.cn

Go:   time.Now()
来源：http://xp.haigaiapp.cn

Ruby: Time.now
来源：http://kz.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qb.gzmigu.cn

[J02] 格式化输出
来源：http://cd.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ht.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fv.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rc.asd995.cn

TS:   d.toISOString()
来源：http://dr.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zx.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vl.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://it.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hl.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://jt.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zp.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://it.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://sc.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://lr.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xs.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xc.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://yc.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sg.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://wh.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kb.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ld.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rm.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ko.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jy.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mt.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dr.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qd.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://qq.asd995.cn

Py:   now + timedelta(days=7)
来源：http://bq.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ai.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ee.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jg.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://mm.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kj.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://jr.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gg.521024.cn

[J06] 计算两时间之差
来源：http://bu.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://iz.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://he.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uv.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://az.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lo.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://zd.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://yc.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://an.shtwfgs.cn

[J07] 比较两个日期
来源：http://ue.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://zg.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qi.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lj.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yd.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ix.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pq.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nu.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://uo.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://mm.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qq.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fk.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bs.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qb.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zg.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tm.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vk.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mq.muxihuayi.cn

[J09] 时区处理
来源：http://mf.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eh.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://va.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lp.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nc.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://un.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kn.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pw.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://hr.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sv.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nc.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hf.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sn.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qd.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fs.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ex.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zr.szxytkj.cn

================================================================================
来源：http://xj.gzmigu.cn

K. JSON 与序列化
来源：http://dn.bjjhwx.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://db.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lw.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gi.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://yh.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://or.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pw.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://tj.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hg.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lc.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://em.szxytkj.cn

Py:   json.loads(s)
来源：http://bz.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ap.nicolike.cn

JS:   JSON.parse(s)
来源：http://oe.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ao.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ke.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://zx.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://eo.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ul.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://cf.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://no.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://do.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vq.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sr.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://el.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://do.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nu.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://la.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://xc.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ab.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sd.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zb.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rj.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zr.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zb.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ol.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://is.9csxet.cn

[K05] 深拷贝对象
来源：http://um.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://ii.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://kl.hnjuh.cn

JS:   structuredClone(obj)
来源：http://bg.gzmigu.cn

TS:   structuredClone(obj)
来源：http://qj.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ve.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://am.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pq.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gv.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://bv.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mu.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ag.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://en.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tq.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ve.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fz.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sp.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sx.shxzskj.cn

[K07] 进制转换
来源：http://bf.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jl.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://av.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zk.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ei.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xw.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ip.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nt.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ts.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://il.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://xd.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xf.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://aq.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ql.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jh.wgjwhj.cn

Go:   encoding/gob
来源：http://oj.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://dz.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rd.hahajie.cn

================================================================================
来源：http://lz.chemitech.net.cn

L. 网络请求
来源：http://sa.hnjuh.cn

================================================================================
来源：http://tj.newstarts.cn

[L01] 发送 GET 请求
来源：http://za.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ud.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://na.shxzskj.cn

JS:   await fetch(url)
来源：http://nz.huanxung.cn

TS:   await fetch(url)
来源：http://ve.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pb.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://eq.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pt.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qc.gzmigu.cn

[L02] 发送 POST JSON
来源：http://ww.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ol.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ak.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ia.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bw.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cg.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hi.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ul.gzmigu.cn

[L03] 设置自定义请求头
来源：http://rj.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wd.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xk.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://al.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oi.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iw.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xe.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ej.yuntaijiaju.cn


<!-- 参考信息 -->