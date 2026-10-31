代发 wailian999

TS:   console.assert(x > 0);
来源：http://np.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://gv.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ks.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kf.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://ea.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://vw.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://dt.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kr.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://em.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vd.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fo.colortex.cn

Go:   err.Error()
来源：http://ev.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://le.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://su.szsharing.cn

[H09] 带错误码的异常
来源：http://nf.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lc.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yp.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yg.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jf.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jv.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gl.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hn.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hu.szxytkj.cn

[H10] 资源自动释放
来源：http://es.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zs.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ng.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gk.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wq.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rs.huanxung.cn

Go:   defer f.Close()
来源：http://ll.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hx.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qa.huixiangedu.cn

================================================================================
来源：http://fw.bookmarksfly.cn

I. 正则表达式
来源：http://io.bookmarksfly.cn

================================================================================
来源：http://uq.nicolike.cn

[I01] 判断是否匹配
来源：http://av.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hu.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ma.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://gb.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://rl.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kq.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tl.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://gr.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fp.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://rn.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://br.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yw.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sk.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://ol.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uk.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tq.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ur.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wgjwhj.cn

[I03] 提取捕获分组
来源：http://cb.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ne.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jg.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gb.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kj.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lc.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://up.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gs.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vf.shtwfgs.cn

[I04] 正则替换
来源：http://qf.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mh.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gu.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xw.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hq.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oj.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://th.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://as.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://un.huixiangedu.cn

[I05] 按正则拆分
来源：http://qr.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dk.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zf.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://bi.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://kf.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://aw.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gk.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mm.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://da.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://us.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://li.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kr.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ed.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fw.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://om.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fx.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ew.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gi.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://yr.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kg.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sr.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mk.gzmigu.cn

TS:   /error/gim
来源：http://pp.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tr.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://am.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ql.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nl.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://ry.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qy.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jj.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sr.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ft.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ew.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pd.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://di.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://on.jctech888.com.cn

================================================================================
来源：http://dr.bookmarksfly.cn

J. 日期与时间
来源：http://vd.521024.cn

================================================================================
来源：http://ep.nszjky.cn

[J01] 获取当前时间
来源：http://rw.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zb.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yo.asd995.cn

JS:   new Date();  Date.now()
来源：http://te.newstarts.cn

TS:   new Date();  Date.now()
来源：http://tm.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rq.colortex.cn

Go:   time.Now()
来源：http://ej.521024.cn

Ruby: Time.now
来源：http://nu.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qy.haigaiapp.cn

[J02] 格式化输出
来源：http://yi.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hw.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ly.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sp.chemitech.net.cn

TS:   d.toISOString()
来源：http://ox.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gb.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://du.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ri.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://qk.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vy.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nb.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://ki.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://sl.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jn.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jz.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://dg.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bv.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://ps.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cb.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ls.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sk.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uv.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xr.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://co.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ho.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wz.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://nw.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://kf.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ek.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zs.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vd.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fk.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bp.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ze.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jx.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ej.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://ia.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://ct.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sg.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ym.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qw.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://jb.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ah.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://tt.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://az.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://gg.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ec.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hx.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ho.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mi.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mn.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://if.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://gc.huanxung.cn

[J08] 提取年月日与星期
来源：http://fz.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ty.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zl.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dc.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ki.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://za.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fn.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qt.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xh.muxihuayi.cn

[J09] 时区处理
来源：http://cg.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vp.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bf.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pa.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xl.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://po.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jz.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wi.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fm.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://if.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zz.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yu.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gv.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xs.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jn.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qd.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qh.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hq.szsharing.cn

================================================================================
来源：http://af.huanxung.cn

K. JSON 与序列化
来源：http://of.wgjwhj.cn

================================================================================
来源：http://qg.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://kr.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kr.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qt.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://kk.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ok.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ye.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://ef.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://na.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kb.szsharing.cn

[K02] JSON 字符串转对象
来源：http://gi.newstarts.cn

Py:   json.loads(s)
来源：http://bc.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sh.szxytkj.cn

JS:   JSON.parse(s)
来源：http://bk.shxzskj.cn

TS:   JSON.parse(s)
来源：http://rl.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yr.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://bk.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://ru.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rb.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://mk.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jg.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jz.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bv.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sl.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oc.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ad.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eg.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ds.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://kx.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://av.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ci.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ev.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://da.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bu.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wh.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://en.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kx.nszjky.cn

[K05] 深拷贝对象
来源：http://lc.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://fl.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.huanxung.cn

JS:   structuredClone(obj)
来源：http://ki.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://im.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xf.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jv.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://op.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fc.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ii.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ra.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xm.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://so.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tt.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://md.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cd.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ov.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pv.gzmigu.cn

[K07] 进制转换
来源：http://ys.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pb.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ih.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xe.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jc.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cm.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qe.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zv.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kp.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://xj.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://yd.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dx.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://xo.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://ih.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ri.bjjhwx.cn

Go:   encoding/gob
来源：http://ca.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://ku.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gq.chemitech.net.cn

================================================================================
来源：http://vx.nszjky.cn

L. 网络请求
来源：http://md.panjiajie.cn

================================================================================
来源：http://sp.521024.cn

[L01] 发送 GET 请求
来源：http://sf.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rp.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qc.chemitech.net.cn

JS:   await fetch(url)
来源：http://qp.panjiajie.cn

TS:   await fetch(url)
来源：http://an.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ax.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://gs.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ff.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://br.shxzukj.cn

[L02] 发送 POST JSON
来源：http://bg.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lf.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ms.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dt.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://du.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hs.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zx.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sj.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mg.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://nr.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sf.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tt.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gb.yuexingan06.cn


<!-- 参考信息 -->