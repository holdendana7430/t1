代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qg.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bk.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://dh.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://wp.colortex.cn

[H07] 断言
来源：http://vx.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ll.gzmigu.cn

PHP:  assert($x > 0);
来源：http://nc.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ij.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://zg.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://fs.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ta.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wi.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://py.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ue.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://vx.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ol.huanxung.cn

JS:   e.message;  e.stack
来源：http://yy.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sq.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ik.nszjky.cn

Go:   err.Error()
来源：http://te.521024.cn

Ruby: e.message;  e.backtrace
来源：http://gm.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://lo.huixiangedu.cn

[H09] 带错误码的异常
来源：http://bs.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lq.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yd.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uw.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://js.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aq.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qz.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gd.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hm.shxzukj.cn

[H10] 资源自动释放
来源：http://go.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rp.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ri.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ey.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://le.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oi.lnxyls.cn

Go:   defer f.Close()
来源：http://yi.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lb.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uw.colortex.cn

================================================================================
来源：http://zk.szsharing.cn

I. 正则表达式
来源：http://px.muxihuayi.cn

================================================================================
来源：http://yy.jctech888.com.cn

[I01] 判断是否匹配
来源：http://gt.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qd.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uv.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://vk.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://pu.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pf.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wf.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://qm.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nv.bjjhwx.cn

[I02] 提取所有匹配
来源：http://sz.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://qf.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jj.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://in.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://ms.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wb.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://rz.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dw.521024.cn

[I03] 提取捕获分组
来源：http://pl.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nz.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://en.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vh.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zt.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zw.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lf.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zh.yuexingan06.cn

[I04] 正则替换
来源：http://vm.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mm.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://er.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yl.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qf.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ld.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wh.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eo.9csxet.cn

[I05] 按正则拆分
来源：http://ji.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nu.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hc.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://kq.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xv.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://gm.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qf.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tq.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mf.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oi.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ui.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wm.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hb.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nb.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wx.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fm.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wi.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tx.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://gp.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ed.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zh.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zi.9csxet.cn

TS:   /error/gim
来源：http://db.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rz.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pp.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://ao.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qi.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ot.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yy.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sj.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nz.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ij.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gq.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://he.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lt.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iw.hnjuh.cn

================================================================================
来源：http://yp.wgjwhj.cn

J. 日期与时间
来源：http://ag.colortex.cn

================================================================================
来源：http://mj.yuexingan06.cn

[J01] 获取当前时间
来源：http://dr.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ac.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jb.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://bh.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://xd.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uw.hnjuh.cn

Go:   time.Now()
来源：http://mf.521024.cn

Ruby: Time.now
来源：http://bo.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ch.huixiangedu.cn

[J02] 格式化输出
来源：http://yw.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ub.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nd.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jk.bookmarksfly.cn

TS:   d.toISOString()
来源：http://ov.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yc.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xy.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bk.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ng.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://yp.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aq.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yp.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://sq.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://zh.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ef.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ug.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://nc.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tx.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://zn.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ay.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zn.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ce.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ju.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kd.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bn.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qo.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://po.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://to.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://hd.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ry.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cw.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wj.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ur.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xf.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://zb.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://am.muxihuayi.cn

[J06] 计算两时间之差
来源：http://st.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://gd.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://pp.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vr.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jn.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dm.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://re.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://co.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://lt.haigaiapp.cn

[J07] 比较两个日期
来源：http://pp.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://be.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dq.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sd.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lc.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bf.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zs.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sj.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://bf.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://at.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zi.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://la.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sc.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dj.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vz.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xe.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oe.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ds.jctech888.com.cn

[J09] 时区处理
来源：http://hm.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mg.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ss.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pq.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ds.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mb.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hp.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pn.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fy.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://bf.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ys.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ip.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zm.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oe.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sj.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ru.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://px.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nn.newstarts.cn

================================================================================
来源：http://nf.muxihuayi.cn

K. JSON 与序列化
来源：http://uc.521024.cn

================================================================================
来源：http://nm.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://iw.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wm.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://je.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://bd.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://xq.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wy.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://ix.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nr.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fg.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ss.nicolike.cn

Py:   json.loads(s)
来源：http://bw.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qc.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://sp.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://iy.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xo.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://tc.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://vr.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kj.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://db.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qg.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xs.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://io.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vm.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zt.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cz.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dy.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://do.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://cb.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ng.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://je.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wg.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dh.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ta.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uv.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uw.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dj.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://sl.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://id.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://qe.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://qe.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://nb.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jn.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ug.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://em.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zo.nicolike.cn

[K06] 解析 URL 查询串
来源：http://eg.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fe.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cd.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zc.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ck.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://so.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aq.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wu.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cu.shxzskj.cn

[K07] 进制转换
来源：http://th.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://it.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bx.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sp.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ql.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ml.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vr.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cw.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ih.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://dp.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://xc.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://or.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://gx.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://hx.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sv.szsharing.cn

Go:   encoding/gob
来源：http://an.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://uf.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://om.bjjhwx.cn

================================================================================
来源：http://pw.yuexingan06.cn

L. 网络请求
来源：http://xt.hahajie.cn

================================================================================
来源：http://fv.panjiajie.cn

[L01] 发送 GET 请求
来源：http://ao.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qz.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gg.bookmarksfly.cn

JS:   await fetch(url)
来源：http://fl.jctech888.com.cn

TS:   await fetch(url)
来源：http://dn.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ql.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://ug.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wk.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://im.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://ja.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kc.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xl.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fb.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vw.szxytkj.cn


<!-- 参考信息 -->