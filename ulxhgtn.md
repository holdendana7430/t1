代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qp.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ii.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://uj.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://sr.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rj.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://pe.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ap.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://ma.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://rk.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ia.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qe.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xb.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qf.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yu.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ju.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://nl.szxytkj.cn

[H07] 断言
来源：http://ok.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://rw.shxzskj.cn

PHP:  assert($x > 0);
来源：http://ii.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://mh.nicolike.cn

TS:   console.assert(x > 0);
来源：http://my.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://hr.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yo.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qk.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ka.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://ou.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://fj.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lj.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://ha.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pw.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lb.colortex.cn

Go:   err.Error()
来源：http://th.521024.cn

Ruby: e.message;  e.backtrace
来源：http://zt.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://hs.szsharing.cn

[H09] 带错误码的异常
来源：http://mn.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vd.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bt.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://im.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tf.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aj.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vu.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iw.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ws.521024.cn

[H10] 资源自动释放
来源：http://la.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bt.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fb.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rt.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sj.9csxet.cn

Go:   defer f.Close()
来源：http://py.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rk.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rr.haigaiapp.cn

================================================================================
来源：http://vf.shxzskj.cn

I. 正则表达式
来源：http://jz.yuexingan06.cn

================================================================================
来源：http://dt.haigaiapp.cn

[I01] 判断是否匹配
来源：http://dp.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zz.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zh.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ah.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://kf.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vy.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bk.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://ip.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nb.gzmigu.cn

[I02] 提取所有匹配
来源：http://id.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://sz.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nm.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xl.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://is.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rl.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ky.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://xu.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qi.9csxet.cn

[I03] 提取捕获分组
来源：http://vx.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pr.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bm.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bj.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wy.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pq.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dg.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://or.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pe.colortex.cn

[I04] 正则替换
来源：http://wq.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://li.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nc.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bw.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kg.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vn.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gx.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hq.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uv.nszjky.cn

[I05] 按正则拆分
来源：http://tm.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pb.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://px.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nz.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://jx.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://ci.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dt.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vq.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pv.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fn.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://de.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://os.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ik.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pp.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cv.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pm.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ej.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vr.521024.cn

[I07] 忽略大小写与多行模式
来源：http://fa.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://af.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nj.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bz.panjiajie.cn

TS:   /error/gim
来源：http://ks.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uq.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lz.521024.cn

Ruby: s.scan(/error/i)
来源：http://ym.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gq.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://gc.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nx.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hc.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sx.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ve.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tv.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aq.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ug.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gs.lnxyls.cn

================================================================================
来源：http://oh.huixinmuqiang.cn

J. 日期与时间
来源：http://vp.shxzukj.cn

================================================================================
来源：http://fa.haigaiapp.cn

[J01] 获取当前时间
来源：http://bw.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cw.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dl.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://fg.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://xg.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vw.bookmarksfly.cn

Go:   time.Now()
来源：http://ci.asd995.cn

Ruby: Time.now
来源：http://ul.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cr.jctech888.com.cn

[J02] 格式化输出
来源：http://zy.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yi.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lb.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://im.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://ke.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bb.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gd.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qa.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dg.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://zp.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kd.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vq.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://lg.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://bz.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sv.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zt.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://pm.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sc.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://vv.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://op.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gz.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ds.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oy.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cj.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uc.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dn.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lw.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://tz.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://bc.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kr.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pn.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xt.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://bt.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nh.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://dz.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://od.colortex.cn

[J06] 计算两时间之差
来源：http://kd.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://gp.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://wu.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://az.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ic.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ap.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://ex.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://co.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://du.muxihuayi.cn

[J07] 比较两个日期
来源：http://dp.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://nj.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ni.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fv.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xg.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hk.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rt.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zy.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://sf.szsharing.cn

[J08] 提取年月日与星期
来源：http://ba.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qf.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ky.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kv.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ex.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://na.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://os.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bh.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://do.bjjhwx.cn

[J09] 时区处理
来源：http://ck.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://da.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hs.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zk.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ek.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vd.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fx.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xk.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ei.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://tq.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dg.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ei.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ut.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ao.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xs.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://am.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kq.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ch.huixiangedu.cn

================================================================================
来源：http://dt.shxzskj.cn

K. JSON 与序列化
来源：http://qm.chemitech.net.cn

================================================================================
来源：http://yo.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://py.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xd.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fb.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://xv.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://xj.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pv.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://pk.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sw.nszjky.cn

[K02] JSON 字符串转对象
来源：http://jr.shxzskj.cn

Py:   json.loads(s)
来源：http://ck.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://za.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ga.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://iq.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ch.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://rc.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://il.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bh.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://in.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wr.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uf.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vh.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oz.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://op.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wr.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tr.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://hy.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tk.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bi.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wy.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vc.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jx.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jg.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tr.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cc.gzmigu.cn

[K05] 深拷贝对象
来源：http://ot.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://rp.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://wz.szsharing.cn

JS:   structuredClone(obj)
来源：http://zs.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ig.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dt.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pz.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ty.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uk.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://rh.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vb.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pg.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wu.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qu.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dd.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xc.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pv.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sk.yuexingan06.cn

[K07] 进制转换
来源：http://my.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ri.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mf.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://go.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://js.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vj.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vn.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xv.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gk.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://sk.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://hh.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ij.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://jq.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://qk.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fj.asd995.cn

Go:   encoding/gob
来源：http://hm.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://cx.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kc.colortex.cn

================================================================================
来源：http://wv.yuntaijiaju.cn

L. 网络请求
来源：http://qm.nszjky.cn

================================================================================
来源：http://ft.huanxung.cn

[L01] 发送 GET 请求
来源：http://ly.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jt.jianghongdianzi.cn


<!-- 参考信息 -->