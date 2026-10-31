代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://fs.521024.cn

C#:   class MyException : Exception {}
来源：http://ef.yuexingan06.cn

[H05] 捕获特定类型
来源：http://oq.colortex.cn

Py:   except ValueError as e:
来源：http://vj.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pd.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ch.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://ep.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://ox.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xn.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://pc.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bn.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://gd.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://dm.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xk.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ui.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cl.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oy.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ug.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://xk.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://xk.shxzskj.cn

[H07] 断言
来源：http://rb.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://ds.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ti.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://tr.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://aw.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://av.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hf.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ng.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://bk.521024.cn

[H08] 获取错误信息与堆栈
来源：http://mq.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://li.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ib.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://nr.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fs.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ek.hnjuh.cn

Go:   err.Error()
来源：http://ed.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://va.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://oh.huixiangedu.cn

[H09] 带错误码的异常
来源：http://dx.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vg.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wg.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xr.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ez.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fb.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ls.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sf.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qw.szsharing.cn

[H10] 资源自动释放
来源：http://jj.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gm.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xr.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://va.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dg.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lr.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://qc.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lw.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://go.colortex.cn

================================================================================
来源：http://qt.lnxyls.cn

I. 正则表达式
来源：http://uu.nicolike.cn

================================================================================
来源：http://cq.haigaiapp.cn

[I01] 判断是否匹配
来源：http://zn.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lx.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sb.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://vm.asd995.cn

TS:   /\d+/.test(s)
来源：http://rn.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dz.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yf.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://ry.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mc.yuexingan06.cn

[I02] 提取所有匹配
来源：http://vg.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ta.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ed.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://od.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://wk.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mw.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ak.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://vi.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xg.panjiajie.cn

[I03] 提取捕获分组
来源：http://jh.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oj.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kx.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ug.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ew.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kk.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pr.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wc.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cp.shxzskj.cn

[I04] 正则替换
来源：http://wl.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ox.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xx.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dg.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://en.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hu.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eo.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kd.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xl.521024.cn

[I05] 按正则拆分
来源：http://av.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rc.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nv.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://nh.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://uy.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://dk.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gy.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rp.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lg.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ze.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vk.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://us.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ny.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iz.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://om.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dp.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wu.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ia.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iv.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xb.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dq.muxihuayi.cn

TS:   /error/gim
来源：http://ql.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ef.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ii.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://vr.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vu.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://di.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kr.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xu.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://py.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zc.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ui.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vd.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xy.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yd.jctech888.com.cn

================================================================================
来源：http://ja.nszjky.cn

J. 日期与时间
来源：http://gf.yuexingan06.cn

================================================================================
来源：http://wg.bookmarksfly.cn

[J01] 获取当前时间
来源：http://xl.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kp.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zt.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://cm.nicolike.cn

TS:   new Date();  Date.now()
来源：http://zj.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yp.hnjuh.cn

Go:   time.Now()
来源：http://nt.colortex.cn

Ruby: Time.now
来源：http://cb.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sz.haigaiapp.cn

[J02] 格式化输出
来源：http://mq.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hk.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jp.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pe.panjiajie.cn

TS:   d.toISOString()
来源：http://bk.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ct.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ou.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fu.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://bv.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gs.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ea.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://iw.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://ms.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ah.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://al.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://bk.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ti.nszjky.cn

[J04] 时间戳与日期互转
来源：http://dd.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ca.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yr.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xl.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pr.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cd.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xp.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mu.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://gr.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://ib.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jt.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kd.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://re.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://qe.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yw.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://po.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zo.muxihuayi.cn

[J06] 计算两时间之差
来源：http://eb.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://vb.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://rt.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tp.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qz.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kg.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://xl.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://lo.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://ra.nszjky.cn

[J07] 比较两个日期
来源：http://ep.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ey.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nj.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://de.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jv.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ot.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bb.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ia.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://dr.9csxet.cn

[J08] 提取年月日与星期
来源：http://ze.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xm.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sw.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bd.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ks.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ys.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qm.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ev.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gl.panjiajie.cn

[J09] 时区处理
来源：http://ni.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rg.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oc.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mr.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ml.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oa.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://su.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://yf.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hq.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hy.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://py.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wz.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fj.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jp.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rm.newstarts.cn

================================================================================
来源：http://dc.jctech888.com.cn

K. JSON 与序列化
来源：http://tp.panjiajie.cn

================================================================================
来源：http://lv.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://it.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uh.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gn.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ge.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://pv.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ba.asd995.cn

Go:   json.Marshal(obj)
来源：http://jf.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zr.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bl.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://vj.panjiajie.cn

Py:   json.loads(s)
来源：http://st.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kq.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://fx.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://zk.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zj.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ot.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://gz.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uo.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://zb.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vy.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wu.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tn.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pr.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ek.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tg.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://au.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zl.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://fh.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ms.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vo.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ro.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qj.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cq.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xh.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vh.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://un.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://jo.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ar.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://cw.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://jg.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://sx.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jo.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fe.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ut.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dm.hahajie.cn

[K06] 解析 URL 查询串
来源：http://yl.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qe.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hm.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ua.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hb.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lf.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ij.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pj.nicolike.cn

[K07] 进制转换
来源：http://vm.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ku.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pe.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pt.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hi.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ie.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gf.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eq.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gb.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://qy.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://hw.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lj.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://vh.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://pz.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vk.521024.cn

Go:   encoding/gob
来源：http://kr.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://oc.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pj.panjiajie.cn

================================================================================
来源：http://mn.colortex.cn


<!-- 参考信息 -->