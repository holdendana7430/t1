代发 wailian999

TS:   console.assert(x > 0);
来源：http://cm.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://as.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hs.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ar.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://rd.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://kc.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://wh.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rs.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://bs.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pd.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nc.szsharing.cn

Go:   err.Error()
来源：http://kq.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://cy.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://hd.hnjuh.cn

[H09] 带错误码的异常
来源：http://zz.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ok.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bd.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iv.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nl.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yu.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oa.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vl.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ts.bookmarksfly.cn

[H10] 资源自动释放
来源：http://on.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://li.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xz.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tj.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nq.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ld.hnjuh.cn

Go:   defer f.Close()
来源：http://wk.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://se.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kj.huixinmuqiang.cn

================================================================================
来源：http://si.szxytkj.cn

I. 正则表达式
来源：http://uv.nicolike.cn

================================================================================
来源：http://wm.newstarts.cn

[I01] 判断是否匹配
来源：http://hf.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fs.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zf.colortex.cn

JS:   /\d+/.test(s)
来源：http://xx.9csxet.cn

TS:   /\d+/.test(s)
来源：http://kh.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sm.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dr.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://fs.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://at.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://md.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://tu.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ue.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qt.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://dr.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qw.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tf.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://tc.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yf.yuexingan06.cn

[I03] 提取捕获分组
来源：http://pi.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gf.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mj.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gk.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ut.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://db.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jo.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wl.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qu.asd995.cn

[I04] 正则替换
来源：http://fu.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://in.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dp.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pf.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://la.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ux.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oh.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jq.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://to.521024.cn

[I05] 按正则拆分
来源：http://rz.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vl.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ji.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://fi.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://qh.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://ft.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jv.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jg.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fl.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kr.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xz.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jl.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://av.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ya.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vp.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ow.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ar.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uf.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://pn.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gw.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jk.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cc.newstarts.cn

TS:   /error/gim
来源：http://mp.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://em.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bs.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://pd.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zq.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://yu.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fw.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kt.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yv.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dy.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aw.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gy.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wa.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lf.chemitech.net.cn

================================================================================
来源：http://cj.wgjwhj.cn

J. 日期与时间
来源：http://at.shxzukj.cn

================================================================================
来源：http://ej.szsharing.cn

[J01] 获取当前时间
来源：http://ts.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wh.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ab.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://zv.asd995.cn

TS:   new Date();  Date.now()
来源：http://rx.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fl.9csxet.cn

Go:   time.Now()
来源：http://sm.haigaiapp.cn

Ruby: Time.now
来源：http://py.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://td.lnxyls.cn

[J02] 格式化输出
来源：http://pz.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gr.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zb.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wi.gzmigu.cn

TS:   d.toISOString()
来源：http://qt.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bp.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://to.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vj.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bl.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://sk.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://la.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ep.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://ed.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://zi.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pt.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xm.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://kp.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kp.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://yp.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bq.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rn.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oo.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gl.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cc.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ik.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sf.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bl.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://wl.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://ee.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yb.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rj.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dw.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ie.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nm.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://ky.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pt.chemitech.net.cn

[J06] 计算两时间之差
来源：http://tq.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://na.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://op.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sb.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ga.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yj.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://hz.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://be.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://ct.521024.cn

[J07] 比较两个日期
来源：http://na.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hq.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jg.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://er.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pk.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oi.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gz.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fq.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://at.colortex.cn

[J08] 提取年月日与星期
来源：http://hl.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rq.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ln.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qt.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dr.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dn.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ex.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kn.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kv.huanxung.cn

[J09] 时区处理
来源：http://eq.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pk.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hv.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jg.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://an.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yf.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ex.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://rh.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://me.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zy.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yd.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wp.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xy.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ju.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fm.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ng.huixiangedu.cn

================================================================================
来源：http://ss.shxzskj.cn

K. JSON 与序列化
来源：http://wu.huixinmuqiang.cn

================================================================================
来源：http://vl.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://ip.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ha.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iy.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://tc.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://je.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cy.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://bi.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ri.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fn.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://mz.shtwfgs.cn

Py:   json.loads(s)
来源：http://xu.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vd.9csxet.cn

JS:   JSON.parse(s)
来源：http://gq.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://zu.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lg.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://jg.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://sd.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ig.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ls.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xg.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mg.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ox.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ng.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xx.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qk.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vj.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pd.colortex.cn

[K04] 读取 JSON 文件
来源：http://ye.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rq.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uo.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uo.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ht.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://br.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kr.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pk.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mc.521024.cn

[K05] 深拷贝对象
来源：http://ik.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://or.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://ko.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://lv.newstarts.cn

TS:   structuredClone(obj)
来源：http://wx.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cx.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wp.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hg.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qt.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://wt.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rn.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uj.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jq.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xk.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ks.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rh.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xa.chemitech.net.cn

[K07] 进制转换
来源：http://rj.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yb.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bc.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yq.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uk.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ec.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dk.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ni.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mw.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://yr.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://wx.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ed.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://aq.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fr.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jn.haigaiapp.cn

Go:   encoding/gob
来源：http://ff.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://ux.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yb.hahajie.cn

================================================================================
来源：http://ef.newstarts.cn

L. 网络请求
来源：http://hx.9csxet.cn

================================================================================
来源：http://bi.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://lg.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pf.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ll.newstarts.cn

JS:   await fetch(url)
来源：http://gf.nszjky.cn

TS:   await fetch(url)
来源：http://vl.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cp.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://qi.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oz.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ew.nicolike.cn

[L02] 发送 POST JSON
来源：http://ub.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pi.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fk.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bq.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jf.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zf.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://il.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hf.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://pd.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://im.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hk.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qe.chemitech.net.cn


<!-- 参考信息 -->