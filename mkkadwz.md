代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://og.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ss.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://sv.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://iq.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tq.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://li.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bt.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ds.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://bk.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vr.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ht.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://es.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://va.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ip.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://vu.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://ms.szxytkj.cn

[H07] 断言
来源：http://ds.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://oc.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://uw.hahajie.cn

JS:   console.assert(x > 0);
来源：http://pn.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://md.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://bw.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xf.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jx.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://io.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://az.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://af.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ax.newstarts.cn

JS:   e.message;  e.stack
来源：http://tm.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://or.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nh.yuexingan06.cn

Go:   err.Error()
来源：http://yb.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://bs.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://sy.wgjwhj.cn

[H09] 带错误码的异常
来源：http://do.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kg.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zc.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fh.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iq.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ti.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ti.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bo.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://pe.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wg.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ha.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fh.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nj.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xy.gzmigu.cn

Go:   defer f.Close()
来源：http://bh.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rk.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ia.chemitech.net.cn

================================================================================
来源：http://gr.panjiajie.cn

I. 正则表达式
来源：http://ow.hnjuh.cn

================================================================================
来源：http://xq.yuexingan06.cn

[I01] 判断是否匹配
来源：http://ed.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gt.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gy.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://mz.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://pk.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mk.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xr.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://pw.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ak.9csxet.cn

[I02] 提取所有匹配
来源：http://ks.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://vv.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sy.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bv.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://ar.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mv.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://je.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ng.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ms.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ip.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cm.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kc.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://px.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oy.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lv.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gl.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ps.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xi.huanxung.cn

[I04] 正则替换
来源：http://ph.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bv.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fl.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mg.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qg.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wp.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kw.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ye.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ke.hnjuh.cn

[I05] 按正则拆分
来源：http://jt.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ba.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iy.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://ya.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://jg.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://yx.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mn.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://up.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ws.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hd.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bl.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tq.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jr.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ll.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lw.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://be.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pg.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cd.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://ce.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ua.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oa.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dg.newstarts.cn

TS:   /error/gim
来源：http://jn.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://za.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ku.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://aj.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sg.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://on.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xr.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sa.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ue.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bp.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tl.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vk.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aj.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gd.nicolike.cn

================================================================================
来源：http://wm.yuexingan06.cn

J. 日期与时间
来源：http://ys.asd995.cn

================================================================================
来源：http://wp.yuexingan06.cn

[J01] 获取当前时间
来源：http://wv.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rn.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://en.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://fv.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://gu.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kh.huanxung.cn

Go:   time.Now()
来源：http://hy.yuntaijiaju.cn

Ruby: Time.now
来源：http://ii.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://by.lnxyls.cn

[J02] 格式化输出
来源：http://ys.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ba.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ir.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dn.bjjhwx.cn

TS:   d.toISOString()
来源：http://bm.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bp.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wr.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ze.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cj.asd995.cn

[J03] 字符串解析为日期
来源：http://zl.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oc.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ta.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://mi.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://im.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://my.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xw.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://xp.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pt.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://dd.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yt.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ql.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fk.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cg.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ys.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pj.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://em.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://um.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://wk.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://fr.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ne.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jf.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://di.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ws.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tg.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://xt.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ub.lnxyls.cn

[J06] 计算两时间之差
来源：http://rg.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ur.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://os.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yh.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ta.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fy.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://rh.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://px.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://eu.muxihuayi.cn

[J07] 比较两个日期
来源：http://ia.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://vm.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pg.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://za.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://si.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lt.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rh.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ia.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://wq.nszjky.cn

[J08] 提取年月日与星期
来源：http://gr.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://py.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sf.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ss.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mt.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://km.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mr.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ur.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pi.haigaiapp.cn

[J09] 时区处理
来源：http://iv.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ty.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nd.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://em.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://se.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xo.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vs.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uo.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bh.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://oi.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vw.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mo.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://em.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gz.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yn.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://su.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fm.lnxyls.cn

================================================================================
来源：http://wj.9csxet.cn

K. JSON 与序列化
来源：http://li.bookmarksfly.cn

================================================================================
来源：http://qp.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://oj.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qk.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wt.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://tz.521024.cn

TS:   JSON.stringify(obj)
来源：http://ou.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fx.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://ot.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nl.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yk.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://rp.huanxung.cn

Py:   json.loads(s)
来源：http://fx.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pk.gzmigu.cn

JS:   JSON.parse(s)
来源：http://uu.newstarts.cn

TS:   JSON.parse(s)
来源：http://mi.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rh.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://lk.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://xd.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oy.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://cn.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ja.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cf.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://br.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dw.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eh.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dx.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://op.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ii.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ve.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qa.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qs.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fj.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xy.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bu.gzmigu.cn

[K05] 深拷贝对象
来源：http://lm.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://mh.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ay.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ia.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://hu.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lq.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ed.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bx.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://my.nszjky.cn

[K06] 解析 URL 查询串
来源：http://sf.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ub.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zw.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cd.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bx.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yn.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mc.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ph.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ll.newstarts.cn

[K07] 进制转换
来源：http://vd.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lm.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eo.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mm.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fc.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yd.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nk.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sp.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pm.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://wa.asd995.cn

Py:   pickle.dumps(obj)
来源：http://vn.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zv.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://fe.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://br.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tb.jctech888.com.cn

Go:   encoding/gob
来源：http://sl.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://jq.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zc.colortex.cn

================================================================================
来源：http://lz.haigaiapp.cn

L. 网络请求
来源：http://nr.yuexingan06.cn

================================================================================
来源：http://lq.lnxyls.cn

[L01] 发送 GET 请求
来源：http://vn.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jl.szxytkj.cn


<!-- 参考信息 -->