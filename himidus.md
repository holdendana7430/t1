代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://vg.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://ep.asd995.cn

[H05] 捕获特定类型
来源：http://fr.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://jj.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bu.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://ee.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ck.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://nh.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yi.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://mp.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ua.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://ud.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://xs.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gq.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wh.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ra.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rz.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sh.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://io.muxihuayi.cn

[H07] 断言
来源：http://ry.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://qk.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://vu.nszjky.cn

JS:   console.assert(x > 0);
来源：http://cy.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://bf.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://wj.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oz.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ef.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://gt.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://pc.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://yg.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jt.panjiajie.cn

JS:   e.message;  e.stack
来源：http://nx.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zg.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sz.muxihuayi.cn

Go:   err.Error()
来源：http://lz.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://ut.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://va.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://tg.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qe.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cx.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cv.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rd.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://et.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ir.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jy.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ld.shxzskj.cn

[H10] 资源自动释放
来源：http://bz.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tw.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wk.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wo.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ca.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sq.nszjky.cn

Go:   defer f.Close()
来源：http://po.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qf.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tz.haigaiapp.cn

================================================================================
来源：http://my.colortex.cn

I. 正则表达式
来源：http://fr.shtwfgs.cn

================================================================================
来源：http://er.shxzukj.cn

[I01] 判断是否匹配
来源：http://iq.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dv.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dl.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://vg.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://sa.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xm.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sb.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ta.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yg.szsharing.cn

[I02] 提取所有匹配
来源：http://nf.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://kx.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fy.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fg.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://lr.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wp.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qv.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://rx.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ue.bjjhwx.cn

[I03] 提取捕获分组
来源：http://mg.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://im.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tw.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cx.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zd.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kh.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cv.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://az.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://da.yuntaijiaju.cn

[I04] 正则替换
来源：http://st.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://io.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mw.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gy.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pb.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fj.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://os.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xm.nicolike.cn

[I05] 按正则拆分
来源：http://su.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tg.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kb.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ga.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://zz.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ls.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nw.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bl.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zn.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yk.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vn.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ql.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pr.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xl.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iq.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kh.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tq.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wx.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://hk.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ja.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mm.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nc.yuexingan06.cn

TS:   /error/gim
来源：http://hs.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lc.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fa.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://hy.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qq.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://zm.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jn.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tz.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xv.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iq.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pi.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pl.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tm.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ze.asd995.cn

================================================================================
来源：http://ij.panjiajie.cn

J. 日期与时间
来源：http://po.shxzskj.cn

================================================================================
来源：http://yo.haigaiapp.cn

[J01] 获取当前时间
来源：http://fk.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://li.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nl.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://zg.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://mn.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zd.haigaiapp.cn

Go:   time.Now()
来源：http://dn.521024.cn

Ruby: Time.now
来源：http://dl.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kc.hahajie.cn

[J02] 格式化输出
来源：http://oq.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ep.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://du.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ga.szsharing.cn

TS:   d.toISOString()
来源：http://wk.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sl.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qs.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kw.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://so.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://wz.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fe.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qa.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://na.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://lu.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yl.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ia.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://tk.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rx.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://sl.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wz.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dy.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oj.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://at.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ap.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ge.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aq.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yk.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ip.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ok.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vg.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ky.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gc.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://rb.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ar.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://em.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ve.huixiangedu.cn

[J06] 计算两时间之差
来源：http://xx.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://zd.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://zr.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rs.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://em.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ld.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ru.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://cw.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://aq.colortex.cn

[J07] 比较两个日期
来源：http://pi.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://sy.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ms.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sz.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sj.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xb.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kq.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://og.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://pt.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://am.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ya.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qt.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hg.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aa.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ba.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ti.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gr.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qv.jianghongdianzi.cn

[J09] 时区处理
来源：http://lp.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ql.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qb.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ok.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fb.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jg.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://an.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://co.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://nw.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yc.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jb.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ys.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vj.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://op.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vc.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ey.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uj.lnxyls.cn

================================================================================
来源：http://gq.yuntaijiaju.cn

K. JSON 与序列化
来源：http://zz.haigaiapp.cn

================================================================================
来源：http://uz.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://fm.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ft.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pu.asd995.cn

JS:   JSON.stringify(obj)
来源：http://bk.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://fh.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fw.huanxung.cn

Go:   json.Marshal(obj)
来源：http://zt.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yt.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wz.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://bn.jctech888.com.cn

Py:   json.loads(s)
来源：http://ke.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ew.9csxet.cn

JS:   JSON.parse(s)
来源：http://ux.colortex.cn

TS:   JSON.parse(s)
来源：http://gh.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wm.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://vl.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://xe.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tt.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://tq.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ne.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fo.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fh.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qy.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ea.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xk.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ic.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://af.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://pb.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bz.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sf.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ma.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ba.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pi.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fl.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rp.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://uy.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://dy.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://mq.szsharing.cn

JS:   structuredClone(obj)
来源：http://pa.shxzukj.cn

TS:   structuredClone(obj)
来源：http://bk.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ye.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gj.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://de.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yg.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://cw.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ok.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mm.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jb.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jt.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://te.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kc.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://df.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zi.wgjwhj.cn

[K07] 进制转换
来源：http://ij.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sn.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jp.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mo.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cl.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cy.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pf.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ga.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pe.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://fq.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://sv.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uy.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://lm.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://no.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sz.colortex.cn

Go:   encoding/gob
来源：http://qh.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://qf.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://co.521024.cn

================================================================================
来源：http://cu.colortex.cn


<!-- 参考信息 -->