代发 wailian999

[H07] 断言
来源：http://zn.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://xq.521024.cn

PHP:  assert($x > 0);
来源：http://ai.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://my.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://fq.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://tk.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gq.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vs.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://an.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://av.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://nx.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ug.colortex.cn

JS:   e.message;  e.stack
来源：http://rl.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ix.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yt.shxzskj.cn

Go:   err.Error()
来源：http://zo.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ab.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://nq.lnxyls.cn

[H09] 带错误码的异常
来源：http://gc.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ko.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fq.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lx.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ji.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ns.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nz.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ne.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bg.hahajie.cn

[H10] 资源自动释放
来源：http://lr.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pb.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qx.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gy.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kw.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://bl.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vv.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ss.shxzskj.cn

================================================================================
来源：http://zn.gzmigu.cn

I. 正则表达式
来源：http://ce.colortex.cn

================================================================================
来源：http://aq.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://px.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://de.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ck.hahajie.cn

JS:   /\d+/.test(s)
来源：http://tn.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://tf.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kk.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qf.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://dc.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rn.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://nz.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://bo.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dn.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qu.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://ox.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xz.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qr.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://tu.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qw.hahajie.cn

[I03] 提取捕获分组
来源：http://jo.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lq.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://df.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pi.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kq.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yt.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nc.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xb.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xj.bookmarksfly.cn

[I04] 正则替换
来源：http://ze.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://so.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rm.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sh.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pt.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jp.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gf.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://if.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eh.panjiajie.cn

[I05] 按正则拆分
来源：http://uj.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://az.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vg.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://qx.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://bw.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://yw.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lj.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lg.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://di.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gq.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xs.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ut.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ox.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aa.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wb.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jc.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ur.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oc.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://mb.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://do.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bu.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vi.lnxyls.cn

TS:   /error/gim
来源：http://hu.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fc.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ut.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://xu.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jl.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://zg.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vx.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gt.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gc.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ad.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://if.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qf.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gv.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sg.panjiajie.cn

================================================================================
来源：http://mk.gzmigu.cn

J. 日期与时间
来源：http://qb.shxzukj.cn

================================================================================
来源：http://ui.lnxyls.cn

[J01] 获取当前时间
来源：http://ay.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dw.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lc.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://dh.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://su.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xd.yuntaijiaju.cn

Go:   time.Now()
来源：http://gf.muxihuayi.cn

Ruby: Time.now
来源：http://ls.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sq.colortex.cn

[J02] 格式化输出
来源：http://yx.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kz.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pq.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qq.newstarts.cn

TS:   d.toISOString()
来源：http://gl.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://av.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://on.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://is.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nh.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://dc.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cm.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wh.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://jf.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://dd.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gh.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pa.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://qs.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rc.hahajie.cn

[J04] 时间戳与日期互转
来源：http://vy.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ci.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nb.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ae.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sc.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gv.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oa.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bs.521024.cn

[J05] 时间加减（加 7 天）
来源：http://yf.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://nz.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ov.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cd.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jr.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://io.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rn.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://cz.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tc.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ux.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://wl.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://xz.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pk.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hs.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oh.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://yd.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://yj.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://ii.yuexingan06.cn

[J07] 比较两个日期
来源：http://ff.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vp.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://va.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bc.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tn.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://so.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fd.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ed.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://un.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://sl.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://df.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rf.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nu.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kh.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ex.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hm.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://am.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pi.nszjky.cn

[J09] 时区处理
来源：http://ph.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nm.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ly.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hk.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fx.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cw.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vl.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mf.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://eg.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cy.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://um.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dd.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mx.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qe.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://un.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dy.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ig.hnjuh.cn

================================================================================
来源：http://np.panjiajie.cn

K. JSON 与序列化
来源：http://gp.nicolike.cn

================================================================================
来源：http://xf.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://np.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ag.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hm.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://gf.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://xo.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vh.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://ed.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jq.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://up.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://lq.9csxet.cn

Py:   json.loads(s)
来源：http://al.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lc.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ok.nicolike.cn

TS:   JSON.parse(s)
来源：http://cy.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gk.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://mc.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://dy.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zi.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://xq.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eu.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pf.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sp.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sb.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ku.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qh.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pp.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://te.szsharing.cn

[K04] 读取 JSON 文件
来源：http://ng.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pb.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uf.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tq.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oh.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tu.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://du.gzmigu.cn

[K05] 深拷贝对象
来源：http://fv.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://va.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://iu.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://ts.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://az.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sv.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yz.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uq.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kb.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://wl.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ig.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mx.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nb.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nw.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rc.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cd.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zm.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aj.nicolike.cn

[K07] 进制转换
来源：http://ao.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jw.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sh.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yi.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eh.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yr.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jd.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gn.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lk.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://lj.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://ws.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ke.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ax.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://wt.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rs.muxihuayi.cn

Go:   encoding/gob
来源：http://wa.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://je.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bf.haigaiapp.cn

================================================================================
来源：http://zc.hahajie.cn

L. 网络请求
来源：http://yd.chemitech.net.cn

================================================================================
来源：http://gy.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://go.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yz.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ef.szxytkj.cn

JS:   await fetch(url)
来源：http://qw.wgjwhj.cn

TS:   await fetch(url)
来源：http://uf.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://za.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://bx.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jl.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uo.hahajie.cn

[L02] 发送 POST JSON
来源：http://rt.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gq.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ld.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mt.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zl.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uy.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://so.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vu.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ql.nicolike.cn


<!-- 参考信息 -->