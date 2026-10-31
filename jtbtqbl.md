代发 wailian999

Py:   value = d.get("k") or default
来源：http://fi.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tk.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ow.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fi.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gx.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ex.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ze.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://xi.shtwfgs.cn

[H07] 断言
来源：http://xr.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://pm.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ww.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://vb.nicolike.cn

TS:   console.assert(x > 0);
来源：http://an.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://lu.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cf.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lc.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://di.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://oc.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://wz.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cm.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://lm.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sp.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oo.asd995.cn

Go:   err.Error()
来源：http://or.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://fc.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ix.muxihuayi.cn

[H09] 带错误码的异常
来源：http://cj.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pt.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hl.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vn.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://el.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pn.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://an.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kb.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tp.huanxung.cn

[H10] 资源自动释放
来源：http://fq.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sh.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bz.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mf.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gj.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ml.huanxung.cn

Go:   defer f.Close()
来源：http://et.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ed.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nk.szxytkj.cn

================================================================================
来源：http://vp.wgjwhj.cn

I. 正则表达式
来源：http://jy.chemitech.net.cn

================================================================================
来源：http://xy.panjiajie.cn

[I01] 判断是否匹配
来源：http://jc.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wm.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fc.9csxet.cn

JS:   /\d+/.test(s)
来源：http://ma.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://zs.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uz.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mx.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://qq.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://es.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://nm.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://zd.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dj.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ql.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://iu.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ep.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dn.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://yn.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gl.nszjky.cn

[I03] 提取捕获分组
来源：http://dc.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bu.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tb.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hk.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lp.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zd.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jj.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bu.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hn.nszjky.cn

[I04] 正则替换
来源：http://bk.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ti.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://si.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ve.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qt.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fg.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ti.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://op.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eg.9csxet.cn

[I05] 按正则拆分
来源：http://or.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hv.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pq.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://za.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://ga.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://rz.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wo.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hi.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zv.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://de.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nz.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lp.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://db.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ko.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ot.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rn.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gg.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kz.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://ig.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qu.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://be.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wn.shxzukj.cn

TS:   /error/gim
来源：http://jk.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qu.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wg.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://qx.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ma.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://kl.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ta.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jb.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tz.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pe.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bd.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lo.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uo.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vm.szxytkj.cn

================================================================================
来源：http://mr.yuexingan06.cn

J. 日期与时间
来源：http://aa.jianghongdianzi.cn

================================================================================
来源：http://yg.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://zx.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yj.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ls.szsharing.cn

JS:   new Date();  Date.now()
来源：http://sv.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://cs.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://up.szxytkj.cn

Go:   time.Now()
来源：http://xx.wgjwhj.cn

Ruby: Time.now
来源：http://uz.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lq.chemitech.net.cn

[J02] 格式化输出
来源：http://pr.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jw.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tp.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eo.yuexingan06.cn

TS:   d.toISOString()
来源：http://qx.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xa.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tu.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qi.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vd.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://dg.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wr.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ki.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ze.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://yb.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ds.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://ib.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fu.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://gr.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ha.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pu.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kr.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dl.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lk.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jn.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mm.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qz.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://xu.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://ua.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jc.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hc.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vc.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ff.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ll.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://uh.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zd.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://pe.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ir.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://sf.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ah.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ad.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ix.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ld.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://pu.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ge.hnjuh.cn

[J07] 比较两个日期
来源：http://hc.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://rn.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ye.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kn.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dh.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kp.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tx.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nr.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.asd995.cn

[J08] 提取年月日与星期
来源：http://mm.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tg.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hm.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nn.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kq.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://be.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jl.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oy.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.huixiangedu.cn

[J09] 时区处理
来源：http://qc.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rv.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bw.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zo.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://at.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hh.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ie.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vl.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://os.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://cp.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zu.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ge.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eg.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gb.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ed.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xg.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://em.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iu.jianghongdianzi.cn

================================================================================
来源：http://ei.shxzukj.cn

K. JSON 与序列化
来源：http://wi.hnjuh.cn

================================================================================
来源：http://sn.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://vp.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ea.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dg.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://up.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://wj.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rm.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://st.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qq.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ev.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://af.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://hb.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nq.hahajie.cn

JS:   JSON.parse(s)
来源：http://kn.shxzskj.cn

TS:   JSON.parse(s)
来源：http://nr.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://td.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://fa.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://vt.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sv.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://xs.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dn.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wp.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rb.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uk.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tn.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mq.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ak.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dh.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://du.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bu.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yn.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vj.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hm.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wp.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vn.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ed.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hc.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://qc.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://zh.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://tz.gzmigu.cn

JS:   structuredClone(obj)
来源：http://vx.szxytkj.cn

TS:   structuredClone(obj)
来源：http://dv.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sb.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ua.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yv.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gp.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://bn.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sg.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pi.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zi.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oj.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ko.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fy.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pb.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dq.colortex.cn

[K07] 进制转换
来源：http://hj.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ec.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tj.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oh.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ql.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rt.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wz.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://un.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pi.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://jn.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://uw.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fd.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://jy.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://su.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rt.hahajie.cn

Go:   encoding/gob
来源：http://oq.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://xu.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ki.colortex.cn

================================================================================
来源：http://zd.gzmigu.cn

L. 网络请求
来源：http://zq.9csxet.cn

================================================================================
来源：http://hb.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://tj.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pq.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ml.szsharing.cn

JS:   await fetch(url)
来源：http://ot.nszjky.cn

TS:   await fetch(url)
来源：http://qo.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ii.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://lb.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zu.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ej.9csxet.cn

[L02] 发送 POST JSON
来源：http://ll.panjiajie.cn


<!-- 参考信息 -->