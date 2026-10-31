代发 wailian999

TS:   console.assert(x > 0);
来源：http://yf.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://ba.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://st.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gc.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://xh.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://yc.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://rr.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tj.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://fh.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bb.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qv.yuexingan06.cn

Go:   err.Error()
来源：http://gs.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ej.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://er.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ph.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aq.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bv.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://df.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iv.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oi.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rl.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mq.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lf.muxihuayi.cn

[H10] 资源自动释放
来源：http://tc.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aa.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mu.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mj.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ru.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ht.shtwfgs.cn

Go:   defer f.Close()
来源：http://vb.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sp.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jc.huixinmuqiang.cn

================================================================================
来源：http://jw.shtwfgs.cn

I. 正则表达式
来源：http://pt.bookmarksfly.cn

================================================================================
来源：http://hr.shtwfgs.cn

[I01] 判断是否匹配
来源：http://oe.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hb.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bp.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://lc.9csxet.cn

TS:   /\d+/.test(s)
来源：http://gp.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ny.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sq.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://nd.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vh.huanxung.cn

[I02] 提取所有匹配
来源：http://he.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://km.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://df.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hi.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://uj.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ly.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ps.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://fo.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://px.hahajie.cn

[I03] 提取捕获分组
来源：http://kg.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://il.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cj.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sr.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jj.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://re.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rx.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hv.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bb.gzmigu.cn

[I04] 正则替换
来源：http://bw.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ez.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vw.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wb.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mc.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://za.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cv.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ap.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bb.lnxyls.cn

[I05] 按正则拆分
来源：http://pg.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tq.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hy.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://ac.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://cd.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://yw.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bl.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dq.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://go.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uc.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uy.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kv.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zh.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cn.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qe.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://my.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jz.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://sz.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://me.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fx.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qe.szxytkj.cn

TS:   /error/gim
来源：http://im.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fb.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uo.asd995.cn

Ruby: s.scan(/error/i)
来源：http://yc.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://yb.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mw.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hi.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eb.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jv.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nw.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vy.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qm.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ej.gzmigu.cn

================================================================================
来源：http://zm.haigaiapp.cn

J. 日期与时间
来源：http://ig.521024.cn

================================================================================
来源：http://hc.asd995.cn

[J01] 获取当前时间
来源：http://pj.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gr.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sp.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://up.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://xs.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vz.szxytkj.cn

Go:   time.Now()
来源：http://li.521024.cn

Ruby: Time.now
来源：http://lc.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oe.asd995.cn

[J02] 格式化输出
来源：http://yy.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://na.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tf.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ys.colortex.cn

TS:   d.toISOString()
来源：http://oi.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tq.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://px.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ww.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ix.shxzskj.cn

[J03] 字符串解析为日期
来源：http://xf.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bg.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bs.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://xf.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://mo.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rg.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qz.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://dt.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xh.nicolike.cn

[J04] 时间戳与日期互转
来源：http://lq.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zx.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bd.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ou.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jp.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yz.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vn.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ap.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ev.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://bb.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://jm.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://du.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ua.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iq.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ap.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wx.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://kt.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://py.nicolike.cn

[J06] 计算两时间之差
来源：http://xo.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://qv.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://zq.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fj.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oh.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ca.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://uz.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://rj.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://gu.huanxung.cn

[J07] 比较两个日期
来源：http://fp.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://bp.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fy.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ts.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ta.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gb.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wm.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ji.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://ld.9csxet.cn

[J08] 提取年月日与星期
来源：http://wf.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kc.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://op.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rl.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ak.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jm.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cn.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jz.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eo.newstarts.cn

[J09] 时区处理
来源：http://cx.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sb.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qf.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bk.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://np.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gz.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ek.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dz.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qb.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://nw.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yw.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://op.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cr.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zs.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jn.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://th.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oq.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xs.chemitech.net.cn

================================================================================
来源：http://gt.haigaiapp.cn

K. JSON 与序列化
来源：http://we.yuntaijiaju.cn

================================================================================
来源：http://nm.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://md.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cg.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tk.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://fs.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://ky.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://an.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ez.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ko.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jt.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://mb.nszjky.cn

Py:   json.loads(s)
来源：http://sr.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://py.szsharing.cn

JS:   JSON.parse(s)
来源：http://qu.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://tk.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yc.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://jd.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://tl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://um.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://cr.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lx.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mb.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qw.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hd.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uw.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://go.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mj.nszjky.cn

[K04] 读取 JSON 文件
来源：http://tn.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ck.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oi.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ci.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gc.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ng.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sf.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pz.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://av.haigaiapp.cn

[K05] 深拷贝对象
来源：http://ov.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://ni.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://rg.shxzskj.cn

JS:   structuredClone(obj)
来源：http://qb.521024.cn

TS:   structuredClone(obj)
来源：http://dd.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vu.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tn.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jc.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ti.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://vo.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rs.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qj.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://te.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pj.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ea.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qm.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aj.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wz.szxytkj.cn

[K07] 进制转换
来源：http://ao.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bh.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cf.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wj.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hu.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yo.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://za.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ar.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ic.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://rq.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://rs.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sp.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://od.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://lg.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fm.newstarts.cn

Go:   encoding/gob
来源：http://rl.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://gx.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vl.nicolike.cn

================================================================================
来源：http://hd.bjjhwx.cn

L. 网络请求
来源：http://bs.9csxet.cn

================================================================================
来源：http://zh.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://zr.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zg.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aw.muxihuayi.cn

JS:   await fetch(url)
来源：http://so.nicolike.cn

TS:   await fetch(url)
来源：http://ps.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gd.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://hc.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nb.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jd.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://yb.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bz.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qf.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ir.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://os.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sw.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nk.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zg.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gq.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ml.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nu.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ad.szsharing.cn


<!-- 参考信息 -->