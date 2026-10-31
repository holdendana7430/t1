代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qz.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://yi.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ky.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://ao.hahajie.cn

Py:   value = d.get("k") or default
来源：http://ih.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bq.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mq.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eu.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qg.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vc.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://xe.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://di.lnxyls.cn

[H07] 断言
来源：http://if.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://cp.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://rl.nszjky.cn

JS:   console.assert(x > 0);
来源：http://zs.nicolike.cn

TS:   console.assert(x > 0);
来源：http://ct.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://kt.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dx.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yq.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://bn.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ef.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://ms.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ax.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://eq.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cv.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tu.panjiajie.cn

Go:   err.Error()
来源：http://ok.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://kh.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://wv.huanxung.cn

[H09] 带错误码的异常
来源：http://za.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zv.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rh.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cu.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dc.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lt.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xj.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vn.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uj.huixiangedu.cn

[H10] 资源自动释放
来源：http://yc.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pv.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wp.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cw.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cs.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ip.newstarts.cn

Go:   defer f.Close()
来源：http://ua.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dq.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eb.szsharing.cn

================================================================================
来源：http://iq.bookmarksfly.cn

I. 正则表达式
来源：http://ka.huixinmuqiang.cn

================================================================================
来源：http://ge.nicolike.cn

[I01] 判断是否匹配
来源：http://le.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pt.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yk.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://st.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://sd.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lk.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ja.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://pi.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nt.yuexingan06.cn

[I02] 提取所有匹配
来源：http://dm.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://bs.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nm.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rt.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://rf.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pn.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tu.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://sq.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hn.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ty.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zp.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qp.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yy.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mn.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ti.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rl.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lz.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tz.haigaiapp.cn

[I04] 正则替换
来源：http://dx.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://po.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uc.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bi.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ak.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ax.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yt.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pl.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hq.muxihuayi.cn

[I05] 按正则拆分
来源：http://qf.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vo.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wb.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://mu.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://vg.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ef.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://az.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dt.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nq.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://et.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xh.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://it.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mo.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vh.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lx.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lg.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://px.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uh.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://jf.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wi.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cv.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mn.szxytkj.cn

TS:   /error/gim
来源：http://ep.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fy.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dj.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://eo.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vu.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://mt.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ib.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xe.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nm.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fd.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lz.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://et.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ug.lnxyls.cn

================================================================================
来源：http://ns.jianghongdianzi.cn

J. 日期与时间
来源：http://bo.shxzukj.cn

================================================================================
来源：http://et.haigaiapp.cn

[J01] 获取当前时间
来源：http://vd.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ln.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iy.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://uz.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://ig.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fi.gzmigu.cn

Go:   time.Now()
来源：http://pt.muxihuayi.cn

Ruby: Time.now
来源：http://yr.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nh.yuntaijiaju.cn

[J02] 格式化输出
来源：http://si.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yf.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ol.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ph.jctech888.com.cn

TS:   d.toISOString()
来源：http://tg.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://by.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fi.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mi.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hp.shxzukj.cn

[J03] 字符串解析为日期
来源：http://ky.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fx.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pj.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://oj.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://qx.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rw.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rj.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://za.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pr.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ml.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://il.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ip.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://up.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hw.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fh.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ve.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bp.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://en.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://kx.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://sy.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kl.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nj.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://sr.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vp.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ju.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dh.nicolike.cn

[J06] 计算两时间之差
来源：http://bj.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://cv.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://kk.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zi.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wc.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vu.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://fg.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://kc.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://su.nszjky.cn

[J07] 比较两个日期
来源：http://of.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://sv.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://en.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pj.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ep.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ef.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://of.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eb.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ue.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://kq.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nh.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lh.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lm.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yt.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uj.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xc.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://np.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pd.gzmigu.cn

[J09] 时区处理
来源：http://aw.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cc.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hk.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qo.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rz.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dt.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dz.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wp.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bt.521024.cn

[J10] 取今天 / 本月第一天
来源：http://hq.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ka.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kb.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pz.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xs.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gd.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hu.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mk.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://of.jctech888.com.cn

================================================================================
来源：http://fm.newstarts.cn

K. JSON 与序列化
来源：http://hc.jianghongdianzi.cn

================================================================================
来源：http://zk.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://zg.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ir.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uw.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ce.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://cx.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ai.asd995.cn

Go:   json.Marshal(obj)
来源：http://yj.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zp.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sc.huanxung.cn

[K02] JSON 字符串转对象
来源：http://tt.nicolike.cn

Py:   json.loads(s)
来源：http://ux.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dh.521024.cn

JS:   JSON.parse(s)
来源：http://yd.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://oo.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iv.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://qi.szsharing.cn

Ruby: JSON.parse(s)
来源：http://fy.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bu.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://mj.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://of.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wu.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nh.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zf.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bo.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yl.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ay.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yg.9csxet.cn

[K04] 读取 JSON 文件
来源：http://ju.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ek.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ve.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ow.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://li.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fd.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qi.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ps.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zw.shxzskj.cn

[K05] 深拷贝对象
来源：http://se.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://zv.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://xb.szsharing.cn

JS:   structuredClone(obj)
来源：http://kf.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://pn.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jr.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kl.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ht.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tv.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://wd.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tq.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vt.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cq.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yf.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dz.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uf.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ud.huixinmuqiang.cn

[K07] 进制转换
来源：http://qt.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nx.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fx.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uw.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sg.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sm.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bu.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eu.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jb.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://cz.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://he.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hf.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://ih.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://qx.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yh.bookmarksfly.cn

Go:   encoding/gob
来源：http://pq.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://vb.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jv.chemitech.net.cn

================================================================================
来源：http://zk.nszjky.cn

L. 网络请求
来源：http://nu.huanxung.cn

================================================================================
来源：http://qw.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://el.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://go.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mr.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://bj.szxytkj.cn

TS:   await fetch(url)
来源：http://th.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ic.panjiajie.cn


<!-- 参考信息 -->