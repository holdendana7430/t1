代发 wailian999

JS:   class MyError extends Error {}
来源：http://lg.szsharing.cn

TS:   class MyError extends Error {}
来源：http://wv.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://kt.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ei.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ng.newstarts.cn

C#:   class MyException : Exception {}
来源：http://nw.huanxung.cn

[H05] 捕获特定类型
来源：http://zd.lnxyls.cn

Py:   except ValueError as e:
来源：http://up.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mn.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://os.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://bw.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://sl.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://om.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://wu.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wy.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://ka.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://fv.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mo.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://et.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nx.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ml.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dl.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://vb.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://iy.jctech888.com.cn

[H07] 断言
来源：http://ho.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://qa.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://ph.hahajie.cn

JS:   console.assert(x > 0);
来源：http://ok.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://zv.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://ck.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vv.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://la.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://id.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://oy.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://kp.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mw.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://we.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ym.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qv.jctech888.com.cn

Go:   err.Error()
来源：http://vp.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ng.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://li.nszjky.cn

[H09] 带错误码的异常
来源：http://qy.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ap.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ps.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mv.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vq.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kp.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://la.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fi.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zu.521024.cn

[H10] 资源自动释放
来源：http://sf.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rt.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kf.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lv.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tl.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wd.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://og.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iq.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kv.shxzskj.cn

================================================================================
来源：http://my.shtwfgs.cn

I. 正则表达式
来源：http://nk.panjiajie.cn

================================================================================
来源：http://ha.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://rl.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ok.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jj.newstarts.cn

JS:   /\d+/.test(s)
来源：http://vf.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://oo.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vl.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yx.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://sb.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aq.chemitech.net.cn

[I02] 提取所有匹配
来源：http://um.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://er.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bx.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oo.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://dj.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://je.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rh.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://of.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aj.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ur.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://da.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iz.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sg.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gw.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wx.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zs.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vl.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mg.newstarts.cn

[I04] 正则替换
来源：http://sb.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ra.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kk.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eq.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://by.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rd.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ve.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pd.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tb.colortex.cn

[I05] 按正则拆分
来源：http://jp.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wp.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bt.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://qy.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ww.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://mo.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gs.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wo.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bn.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vr.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xe.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yq.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rf.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jw.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://il.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lr.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ly.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ba.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://iw.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zz.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ar.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tc.huixinmuqiang.cn

TS:   /error/gim
来源：http://lu.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ds.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jz.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://rj.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xe.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://id.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pn.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jv.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://br.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://om.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sg.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vc.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sg.jctech888.com.cn

================================================================================
来源：http://ds.szxytkj.cn

J. 日期与时间
来源：http://kf.haigaiapp.cn

================================================================================
来源：http://ho.bjjhwx.cn

[J01] 获取当前时间
来源：http://jl.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bx.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fo.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://hg.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://or.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ue.newstarts.cn

Go:   time.Now()
来源：http://re.hnjuh.cn

Ruby: Time.now
来源：http://ol.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mk.yuntaijiaju.cn

[J02] 格式化输出
来源：http://jd.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pz.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wa.gzmigu.cn

TS:   d.toISOString()
来源：http://rp.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ld.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vh.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pw.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://br.9csxet.cn

[J03] 字符串解析为日期
来源：http://lg.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://or.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sm.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://ya.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://tv.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pl.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ut.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://vt.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://np.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://xj.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sc.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oa.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tf.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xk.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bn.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ue.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ag.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gw.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://zs.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://za.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zx.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xb.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nk.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://bm.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xj.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://rh.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vi.gzmigu.cn

[J06] 计算两时间之差
来源：http://ih.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://tq.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://ch.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pn.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kf.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wb.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://hc.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ld.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://az.szsharing.cn

[J07] 比较两个日期
来源：http://ry.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://iq.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dx.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ri.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://na.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zj.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sl.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vb.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://ai.colortex.cn

[J08] 提取年月日与星期
来源：http://pl.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lk.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aa.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vw.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cu.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jz.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gh.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oa.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vf.shtwfgs.cn

[J09] 时区处理
来源：http://si.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ck.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yo.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ox.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cb.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ok.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dj.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rs.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mn.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://df.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wi.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ie.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ks.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tn.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wj.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sq.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://us.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qt.newstarts.cn

================================================================================
来源：http://ei.gzmigu.cn

K. JSON 与序列化
来源：http://ye.panjiajie.cn

================================================================================
来源：http://ea.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://es.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gj.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zl.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://hl.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://kj.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ju.nicolike.cn

Go:   json.Marshal(obj)
来源：http://jt.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rw.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rs.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://uv.huanxung.cn

Py:   json.loads(s)
来源：http://kg.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hu.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://mr.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://wv.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kz.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://qp.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://us.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lz.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://mj.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rp.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wv.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nu.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ix.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hk.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kk.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pq.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tp.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://df.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xj.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vj.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cz.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sj.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xs.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ht.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ii.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.muxihuayi.cn

[K05] 深拷贝对象
来源：http://ii.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://iv.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://tu.newstarts.cn

JS:   structuredClone(obj)
来源：http://pb.shxzskj.cn

TS:   structuredClone(obj)
来源：http://by.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iv.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rc.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://az.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rl.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://bq.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rk.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://os.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bo.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wj.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dt.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rw.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zg.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hx.asd995.cn

[K07] 进制转换
来源：http://ja.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pl.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qk.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bf.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jx.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mn.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://px.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kw.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sg.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://pn.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://kk.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qu.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nz.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://qd.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://br.shxzskj.cn


<!-- 参考信息 -->