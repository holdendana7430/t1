代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xx.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://uu.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://zn.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://cs.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://se.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://ni.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pk.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://vg.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://cw.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rf.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bh.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jc.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://db.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xn.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://rq.521024.cn

C#:   obj?.A?.B ?? default
来源：http://yy.shxzukj.cn

[H07] 断言
来源：http://jr.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://xq.521024.cn

PHP:  assert($x > 0);
来源：http://gn.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://qm.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://qf.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://dr.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ip.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iw.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://br.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://vh.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://ui.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pu.hahajie.cn

JS:   e.message;  e.stack
来源：http://bx.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://po.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jx.newstarts.cn

Go:   err.Error()
来源：http://hn.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://gq.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ya.shxzskj.cn

[H09] 带错误码的异常
来源：http://ns.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xa.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uq.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iv.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kw.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yg.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eb.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fm.wgjwhj.cn

[H10] 资源自动释放
来源：http://et.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yk.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ce.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ph.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kx.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ir.huixiangedu.cn

Go:   defer f.Close()
来源：http://kd.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ex.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dm.szxytkj.cn

================================================================================
来源：http://bt.shtwfgs.cn

I. 正则表达式
来源：http://il.jctech888.com.cn

================================================================================
来源：http://rx.chemitech.net.cn

[I01] 判断是否匹配
来源：http://tj.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ae.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wm.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://fp.521024.cn

TS:   /\d+/.test(s)
来源：http://fr.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://az.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qq.521024.cn

Ruby: s.match?(/\d+/)
来源：http://ey.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oz.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://xu.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://gy.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gh.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ml.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://fg.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ht.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ni.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://zz.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mb.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://df.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xx.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://la.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jf.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ky.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gg.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ju.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mc.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hu.newstarts.cn

[I04] 正则替换
来源：http://sn.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kg.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kf.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://my.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xe.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cm.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ej.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://le.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yg.haigaiapp.cn

[I05] 按正则拆分
来源：http://wq.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ca.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oq.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://bk.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xk.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://iu.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://du.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vk.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pe.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vr.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xf.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hk.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kz.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eo.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nt.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ps.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nm.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://vd.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://he.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ib.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lg.hahajie.cn

TS:   /error/gim
来源：http://ej.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ul.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ft.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://ft.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hu.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qb.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ef.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xe.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jd.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zw.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dx.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zh.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://te.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://op.szxytkj.cn

================================================================================
来源：http://hx.szsharing.cn

J. 日期与时间
来源：http://uz.gzmigu.cn

================================================================================
来源：http://pr.jctech888.com.cn

[J01] 获取当前时间
来源：http://ml.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://af.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nt.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://cy.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://mt.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cj.nszjky.cn

Go:   time.Now()
来源：http://kn.gzmigu.cn

Ruby: Time.now
来源：http://cx.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rd.huixiangedu.cn

[J02] 格式化输出
来源：http://po.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fu.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dk.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://da.gzmigu.cn

TS:   d.toISOString()
来源：http://xc.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cl.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xd.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eg.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ps.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ma.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lm.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://xt.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://wj.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://na.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ei.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wi.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://yx.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tw.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://go.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ph.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fu.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jz.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://db.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ex.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ik.521024.cn

[J05] 时间加减（加 7 天）
来源：http://hn.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://ej.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xi.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ci.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://vd.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wb.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://ob.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ff.shtwfgs.cn

[J06] 计算两时间之差
来源：http://wu.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://sz.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://em.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yi.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jg.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nw.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://hf.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://qh.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://va.gzmigu.cn

[J07] 比较两个日期
来源：http://qa.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://vx.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ev.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://di.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vf.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qy.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ag.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vc.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://kc.asd995.cn

[J08] 提取年月日与星期
来源：http://ym.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rk.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hs.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gz.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mp.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vj.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pt.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cm.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.haigaiapp.cn

[J09] 时区处理
来源：http://bm.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vy.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qb.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gx.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nq.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wg.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uc.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oi.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xi.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://lg.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ck.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xt.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tf.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://go.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nk.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hn.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ok.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xw.jianghongdianzi.cn

================================================================================
来源：http://fc.gzmigu.cn

K. JSON 与序列化
来源：http://gm.lnxyls.cn

================================================================================
来源：http://jn.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://xp.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rq.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fx.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://jr.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://aa.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vi.huanxung.cn

Go:   json.Marshal(obj)
来源：http://hr.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pt.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cs.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://qi.haigaiapp.cn

Py:   json.loads(s)
来源：http://md.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gt.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://du.asd995.cn

TS:   JSON.parse(s)
来源：http://wc.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rd.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://to.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://bv.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lf.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://vb.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pf.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://by.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://it.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tq.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://at.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aa.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zq.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://ff.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://st.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kp.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://il.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fg.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://de.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ee.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lt.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xe.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://dz.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://yy.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://il.gzmigu.cn

JS:   structuredClone(obj)
来源：http://jf.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://xs.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hk.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://it.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dv.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rj.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ss.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jv.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aa.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gy.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bd.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hw.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tp.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yl.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://og.newstarts.cn

[K07] 进制转换
来源：http://sv.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kg.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zz.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://am.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vw.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ya.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oa.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mx.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qz.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://pj.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://cv.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mv.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://im.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ha.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pm.hnjuh.cn

Go:   encoding/gob
来源：http://hp.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://xd.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jg.newstarts.cn

================================================================================
来源：http://qs.huixiangedu.cn

L. 网络请求
来源：http://ri.szxytkj.cn

================================================================================
来源：http://it.gzmigu.cn

[L01] 发送 GET 请求
来源：http://vy.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ao.asd995.cn


<!-- 参考信息 -->