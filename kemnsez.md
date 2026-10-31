代发 wailian999

Py:   value = d.get("k") or default
来源：http://ql.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zw.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dg.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fw.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lm.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oo.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://mp.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://zr.nszjky.cn

[H07] 断言
来源：http://hw.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://wf.hnjuh.cn

PHP:  assert($x > 0);
来源：http://wo.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://vw.521024.cn

TS:   console.assert(x > 0);
来源：http://kz.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://xc.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pu.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hx.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://wl.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://nq.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://hk.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pg.huanxung.cn

JS:   e.message;  e.stack
来源：http://oi.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lj.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gb.newstarts.cn

Go:   err.Error()
来源：http://na.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://jt.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://zh.szxytkj.cn

[H09] 带错误码的异常
来源：http://nb.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xi.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xt.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jk.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qu.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sv.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://as.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ub.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vy.nicolike.cn

[H10] 资源自动释放
来源：http://mu.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fz.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://as.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oc.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dl.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sq.huanxung.cn

Go:   defer f.Close()
来源：http://tr.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uy.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zt.9csxet.cn

================================================================================
来源：http://re.shxzskj.cn

I. 正则表达式
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://ef.bjjhwx.cn

[I01] 判断是否匹配
来源：http://ql.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vd.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fj.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://yq.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://al.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rt.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vo.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://yg.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oa.gzmigu.cn

[I02] 提取所有匹配
来源：http://ml.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://sz.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wp.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qr.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://wu.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pm.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fg.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://gg.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xc.szsharing.cn

[I03] 提取捕获分组
来源：http://uz.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pz.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zf.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ks.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sq.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zx.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ss.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vc.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ew.szsharing.cn

[I04] 正则替换
来源：http://fj.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hw.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fm.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dm.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xi.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sm.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ng.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yr.521024.cn

[I05] 按正则拆分
来源：http://qp.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qm.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xp.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://eb.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://qg.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://dx.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xo.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://df.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qw.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nc.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xr.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://la.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qy.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://li.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xr.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://io.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fj.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jx.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://mo.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://di.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pu.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qv.9csxet.cn

TS:   /error/gim
来源：http://sw.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iz.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qw.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://ok.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pw.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://tp.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cg.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jo.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cu.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uy.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uh.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://la.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xu.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yp.newstarts.cn

================================================================================
来源：http://dk.newstarts.cn

J. 日期与时间
来源：http://pd.asd995.cn

================================================================================
来源：http://iz.shxzukj.cn

[J01] 获取当前时间
来源：http://bz.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gm.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://el.521024.cn

JS:   new Date();  Date.now()
来源：http://ew.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://nw.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://we.wgjwhj.cn

Go:   time.Now()
来源：http://zc.nicolike.cn

Ruby: Time.now
来源：http://ut.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ym.asd995.cn

[J02] 格式化输出
来源：http://ki.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ds.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fb.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ui.newstarts.cn

TS:   d.toISOString()
来源：http://fx.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xz.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://su.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ei.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://go.colortex.cn

[J03] 字符串解析为日期
来源：http://ve.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://we.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mk.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ka.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://gf.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ld.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lp.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://mp.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gr.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://et.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wx.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eb.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xj.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nq.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fa.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fw.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xz.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sp.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://fv.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://qs.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ov.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rd.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ds.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://we.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xo.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://le.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://md.bjjhwx.cn

[J06] 计算两时间之差
来源：http://jf.521024.cn

Py:   (end - start).total_seconds()
来源：http://np.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://hu.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cr.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bc.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://up.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://mo.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://dh.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://gc.colortex.cn

[J07] 比较两个日期
来源：http://bt.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://xd.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cs.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ht.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://te.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tx.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xq.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://is.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://nb.szsharing.cn

[J08] 提取年月日与星期
来源：http://xk.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kz.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ip.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lv.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://do.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ik.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tl.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ha.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bs.bjjhwx.cn

[J09] 时区处理
来源：http://lf.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ov.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mf.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vm.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ox.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ln.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xc.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mf.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://io.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://tt.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dx.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://in.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iy.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vh.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eg.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xi.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oj.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ka.muxihuayi.cn

================================================================================
来源：http://fq.hnjuh.cn

K. JSON 与序列化
来源：http://ub.yuexingan06.cn

================================================================================
来源：http://qv.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ip.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wx.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cv.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://hd.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://tw.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://bm.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nc.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vh.hahajie.cn

[K02] JSON 字符串转对象
来源：http://va.jctech888.com.cn

Py:   json.loads(s)
来源：http://ch.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://py.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://hn.hnjuh.cn

TS:   JSON.parse(s)
来源：http://fh.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://de.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://qv.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://li.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vr.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://fq.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kn.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rg.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ap.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zn.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hm.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ma.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ld.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dq.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://tn.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ga.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yi.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jw.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bb.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fy.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://um.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kn.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mq.jctech888.com.cn

[K05] 深拷贝对象
来源：http://dk.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://wl.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ti.nicolike.cn

JS:   structuredClone(obj)
来源：http://su.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ad.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://do.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gg.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wn.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://al.asd995.cn

[K06] 解析 URL 查询串
来源：http://xs.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vh.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xo.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rn.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://la.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ce.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lm.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lw.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kr.nszjky.cn

[K07] 进制转换
来源：http://yq.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qu.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eu.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://am.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rk.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pe.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ql.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jm.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uh.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://vm.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://nj.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kg.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zs.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://dm.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dd.hnjuh.cn

Go:   encoding/gob
来源：http://hf.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://rv.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fx.chemitech.net.cn

================================================================================
来源：http://bv.yuexingan06.cn

L. 网络请求
来源：http://yq.huixinmuqiang.cn

================================================================================
来源：http://hq.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://re.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qc.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vt.shtwfgs.cn

JS:   await fetch(url)
来源：http://rr.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://jw.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xf.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://so.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fa.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://av.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ns.hnjuh.cn


<!-- 参考信息 -->