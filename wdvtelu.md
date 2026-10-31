代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wg.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://pf.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mv.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://cq.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://jk.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rc.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ez.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vl.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mk.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qk.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://wo.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://xe.shxzskj.cn

[H07] 断言
来源：http://hx.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://to.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://aj.szsharing.cn

JS:   console.assert(x > 0);
来源：http://xi.newstarts.cn

TS:   console.assert(x > 0);
来源：http://aq.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://kj.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qd.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kc.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://ay.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://qd.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://vt.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iu.newstarts.cn

JS:   e.message;  e.stack
来源：http://pe.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vp.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dr.asd995.cn

Go:   err.Error()
来源：http://gk.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://qb.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://gb.nicolike.cn

[H09] 带错误码的异常
来源：http://ls.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xh.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ro.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ga.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mr.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nn.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ag.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tq.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ro.hnjuh.cn

[H10] 资源自动释放
来源：http://oh.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mr.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ss.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://km.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xa.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qi.yuexingan06.cn

Go:   defer f.Close()
来源：http://sp.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nq.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ck.szxytkj.cn

================================================================================
来源：http://pe.gzmigu.cn

I. 正则表达式
来源：http://fg.szxytkj.cn

================================================================================
来源：http://hq.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ku.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ee.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vb.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://dj.9csxet.cn

TS:   /\d+/.test(s)
来源：http://mp.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qe.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ep.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://gv.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://am.colortex.cn

[I02] 提取所有匹配
来源：http://dj.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://lt.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vn.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ss.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://hx.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ga.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mk.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ra.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vp.shtwfgs.cn

[I03] 提取捕获分组
来源：http://eo.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mw.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ga.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mr.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yj.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lh.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cx.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ze.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yf.jctech888.com.cn

[I04] 正则替换
来源：http://vk.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://er.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tc.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kw.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vu.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://de.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pk.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://na.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pq.panjiajie.cn

[I05] 按正则拆分
来源：http://ag.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bm.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zl.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://bx.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://sf.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://lr.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iv.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uf.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hc.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dx.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vk.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fq.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rr.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lx.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gg.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pp.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ju.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lb.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://wc.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ey.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://em.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yg.lnxyls.cn

TS:   /error/gim
来源：http://gz.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ao.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jf.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://jk.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hy.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://nk.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jk.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://go.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wc.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yg.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gs.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ge.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jd.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sv.shxzskj.cn

================================================================================
来源：http://rn.yuntaijiaju.cn

J. 日期与时间
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://ff.chemitech.net.cn

[J01] 获取当前时间
来源：http://ei.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ci.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://up.asd995.cn

JS:   new Date();  Date.now()
来源：http://sh.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://zg.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cy.haigaiapp.cn

Go:   time.Now()
来源：http://wf.yuntaijiaju.cn

Ruby: Time.now
来源：http://lb.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yc.colortex.cn

[J02] 格式化输出
来源：http://ra.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vn.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bj.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://my.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://pm.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sj.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://od.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wa.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ua.shxzukj.cn

[J03] 字符串解析为日期
来源：http://ca.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nf.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xx.asd995.cn

JS:   new Date("2024-01-02")
来源：http://oi.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://kp.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bi.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kk.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://ym.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dd.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://lo.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sl.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://or.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lu.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ts.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ll.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qn.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nk.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://em.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ob.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://xs.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hl.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://md.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dv.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://ey.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zn.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://wz.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ir.muxihuayi.cn

[J06] 计算两时间之差
来源：http://oi.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ip.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://jj.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ao.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ji.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qe.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://gz.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://oy.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://yy.9csxet.cn

[J07] 比较两个日期
来源：http://mu.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://fz.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pd.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qh.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gl.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cz.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oz.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://uc.newstarts.cn

[J08] 提取年月日与星期
来源：http://ox.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nx.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bt.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wb.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xt.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bq.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sd.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cb.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jc.9csxet.cn

[J09] 时区处理
来源：http://sh.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mv.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ig.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zx.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cu.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zc.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://va.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ij.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://zz.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vj.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oj.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bf.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mg.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fs.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://el.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gm.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zb.newstarts.cn

================================================================================
来源：http://dz.muxihuayi.cn

K. JSON 与序列化
来源：http://nb.chemitech.net.cn

================================================================================
来源：http://zw.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://wq.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zr.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://va.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://yt.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://wv.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wr.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://cr.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qj.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qb.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://gb.colortex.cn

Py:   json.loads(s)
来源：http://ab.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ah.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://id.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://by.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zb.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://rv.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://uz.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wc.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://yy.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ul.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tl.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ut.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ke.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://py.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://or.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qg.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jl.9csxet.cn

[K04] 读取 JSON 文件
来源：http://lq.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vg.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bc.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tb.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vw.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yk.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cc.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dp.nszjky.cn

[K05] 深拷贝对象
来源：http://dc.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://dk.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://fh.panjiajie.cn

JS:   structuredClone(obj)
来源：http://rj.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://uo.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rl.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://or.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tb.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nq.hahajie.cn

[K06] 解析 URL 查询串
来源：http://hh.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xw.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lr.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://am.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yh.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tg.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xt.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qy.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dn.szsharing.cn

[K07] 进制转换
来源：http://uk.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xn.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tt.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mn.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ek.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jw.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ym.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://li.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mp.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://xi.521024.cn

Py:   pickle.dumps(obj)
来源：http://yo.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ix.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://zn.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://br.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pz.wgjwhj.cn

Go:   encoding/gob
来源：http://gk.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://pv.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jn.newstarts.cn

================================================================================
来源：http://qz.haigaiapp.cn

L. 网络请求
来源：http://pr.521024.cn

================================================================================
来源：http://wj.lnxyls.cn

[L01] 发送 GET 请求
来源：http://ys.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vx.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gb.newstarts.cn

JS:   await fetch(url)
来源：http://lv.colortex.cn

TS:   await fetch(url)
来源：http://pq.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ut.huanxung.cn


<!-- 参考信息 -->