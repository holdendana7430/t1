代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ez.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://wi.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ug.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://aa.hahajie.cn

Py:   value = d.get("k") or default
来源：http://fj.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ec.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xb.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ij.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wh.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ct.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://zq.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://en.yuexingan06.cn

[H07] 断言
来源：http://wd.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://nh.gzmigu.cn

PHP:  assert($x > 0);
来源：http://iw.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://rs.huanxung.cn

TS:   console.assert(x > 0);
来源：http://vm.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://ms.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eo.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wv.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://qj.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ry.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://sk.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ej.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://la.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ub.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://us.yuntaijiaju.cn

Go:   err.Error()
来源：http://hr.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://yj.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://ti.szxytkj.cn

[H09] 带错误码的异常
来源：http://ui.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ic.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wf.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ez.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://as.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rk.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wb.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ly.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nn.panjiajie.cn

[H10] 资源自动释放
来源：http://yx.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pn.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qo.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hk.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ra.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qs.lnxyls.cn

Go:   defer f.Close()
来源：http://bg.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cx.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jg.hnjuh.cn

================================================================================
来源：http://bi.nicolike.cn

I. 正则表达式
来源：http://ng.yuexingan06.cn

================================================================================
来源：http://nd.szsharing.cn

[I01] 判断是否匹配
来源：http://ad.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ge.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ne.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://iz.colortex.cn

TS:   /\d+/.test(s)
来源：http://of.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nj.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://re.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://kx.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aw.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ma.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://al.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yv.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dx.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://mb.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ub.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://db.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://mp.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kh.huixiangedu.cn

[I03] 提取捕获分组
来源：http://hq.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://at.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xp.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://po.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://um.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sp.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ky.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pc.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ng.huixinmuqiang.cn

[I04] 正则替换
来源：http://jt.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kx.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://go.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vf.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vn.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jm.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rc.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tm.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pd.shtwfgs.cn

[I05] 按正则拆分
来源：http://gx.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jl.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nu.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://xp.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ys.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://vr.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zx.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wj.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wf.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sy.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yr.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ip.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yf.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cc.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vk.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jx.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qt.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uf.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://gw.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fh.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gy.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kh.colortex.cn

TS:   /error/gim
来源：http://xj.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dp.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://je.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://qx.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oz.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ub.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://en.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://is.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rk.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://to.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zm.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ce.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qv.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qq.521024.cn

================================================================================
来源：http://hz.hahajie.cn

J. 日期与时间
来源：http://de.nicolike.cn

================================================================================
来源：http://rc.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://sr.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ve.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pa.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://ii.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://yr.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tl.hnjuh.cn

Go:   time.Now()
来源：http://oq.jctech888.com.cn

Ruby: Time.now
来源：http://gb.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pc.chemitech.net.cn

[J02] 格式化输出
来源：http://rl.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ok.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dx.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pz.huixiangedu.cn

TS:   d.toISOString()
来源：http://ub.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sp.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ez.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rf.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://on.szsharing.cn

[J03] 字符串解析为日期
来源：http://ek.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://li.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uh.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ub.521024.cn

TS:   new Date("2024-01-02")
来源：http://qb.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pf.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jg.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://tv.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gn.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://hf.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gs.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sb.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dh.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lq.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cl.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ml.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wt.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nz.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://sk.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ou.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ca.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mr.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://op.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ry.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xg.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://br.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zx.szsharing.cn

[J06] 计算两时间之差
来源：http://si.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://bf.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://bk.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pu.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ab.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://sf.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://rf.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://wo.shtwfgs.cn

[J07] 比较两个日期
来源：http://uh.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ni.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bi.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cf.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fo.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fs.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fd.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://es.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://wr.panjiajie.cn

[J08] 提取年月日与星期
来源：http://zd.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://il.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://md.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bi.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xo.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vz.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dd.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ef.newstarts.cn

[J09] 时区处理
来源：http://gw.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://em.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aq.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jw.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tb.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pk.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://av.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uv.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://dk.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wi.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cb.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fj.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wi.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jr.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fs.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kk.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fy.muxihuayi.cn

================================================================================
来源：http://hw.nszjky.cn

K. JSON 与序列化
来源：http://jn.bjjhwx.cn

================================================================================
来源：http://hu.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://we.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aj.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yf.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://fl.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://ao.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xj.hahajie.cn

Go:   json.Marshal(obj)
来源：http://je.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bj.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bl.asd995.cn

[K02] JSON 字符串转对象
来源：http://xo.colortex.cn

Py:   json.loads(s)
来源：http://ge.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yz.shxzukj.cn

JS:   JSON.parse(s)
来源：http://qe.nszjky.cn

TS:   JSON.parse(s)
来源：http://vx.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://va.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://jr.newstarts.cn

Ruby: JSON.parse(s)
来源：http://oe.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zs.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://uu.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tf.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ua.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://te.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ut.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://py.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yt.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qq.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vk.szsharing.cn

[K04] 读取 JSON 文件
来源：http://no.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://er.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xk.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ns.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cc.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cv.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lg.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ig.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ky.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://rs.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://aj.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://hu.hnjuh.cn

JS:   structuredClone(obj)
来源：http://zg.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://nx.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rl.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hx.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mt.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cg.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://ss.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pc.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bt.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vo.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bl.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ma.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fb.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bl.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ei.hahajie.cn

[K07] 进制转换
来源：http://jk.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vy.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kk.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cr.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bi.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qv.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ta.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vy.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://av.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://dr.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://sv.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ae.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://mv.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://ut.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vl.gzmigu.cn

Go:   encoding/gob
来源：http://sv.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://et.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vw.shxzskj.cn

================================================================================
来源：http://rg.bookmarksfly.cn

L. 网络请求
来源：http://qf.szxytkj.cn

================================================================================
来源：http://uq.521024.cn

[L01] 发送 GET 请求
来源：http://gi.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cm.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ls.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://qe.newstarts.cn

TS:   await fetch(url)
来源：http://zz.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wf.asd995.cn


<!-- 参考信息 -->