代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bj.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://fm.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://fe.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://sv.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ev.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://qf.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hk.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://jz.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://pu.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cv.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tf.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xi.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yy.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nj.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://cj.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://es.asd995.cn

[H07] 断言
来源：http://lb.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://tv.panjiajie.cn

PHP:  assert($x > 0);
来源：http://lf.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://ge.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://fz.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://xl.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nx.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://js.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://gr.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://rh.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://fo.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jl.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://pw.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ix.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bg.huixinmuqiang.cn

Go:   err.Error()
来源：http://lk.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://fx.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://az.huanxung.cn

[H09] 带错误码的异常
来源：http://uf.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iv.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vh.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xs.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jz.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ip.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fx.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://az.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xf.shxzskj.cn

[H10] 资源自动释放
来源：http://og.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://on.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zj.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hm.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mh.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mt.haigaiapp.cn

Go:   defer f.Close()
来源：http://il.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://da.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ih.nszjky.cn

================================================================================
来源：http://gt.asd995.cn

I. 正则表达式
来源：http://jl.colortex.cn

================================================================================
来源：http://ik.shxzukj.cn

[I01] 判断是否匹配
来源：http://qj.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jt.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ic.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ex.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://lz.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rs.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xp.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://bq.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://to.lnxyls.cn

[I02] 提取所有匹配
来源：http://fi.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ut.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jf.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wf.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://vt.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jb.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://li.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://vl.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ze.shxzukj.cn

[I03] 提取捕获分组
来源：http://bg.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ys.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rs.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sj.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sl.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tu.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ie.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hj.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qo.shtwfgs.cn

[I04] 正则替换
来源：http://ej.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lz.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://is.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gj.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yo.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ez.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zb.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xv.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bt.muxihuayi.cn

[I05] 按正则拆分
来源：http://hl.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yb.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ma.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://bh.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://xj.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://vc.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oq.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rk.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fj.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dg.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bo.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pb.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cu.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qb.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://st.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oi.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uo.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://am.521024.cn

[I07] 忽略大小写与多行模式
来源：http://oc.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lm.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ns.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ib.yuntaijiaju.cn

TS:   /error/gim
来源：http://bs.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zb.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nw.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://np.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fe.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://sn.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mw.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cu.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jf.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cu.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dy.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ru.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://us.newstarts.cn

================================================================================
来源：http://ul.newstarts.cn

J. 日期与时间
来源：http://dr.bookmarksfly.cn

================================================================================
来源：http://lv.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://hg.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://li.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ms.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://xm.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://fb.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tu.shxzskj.cn

Go:   time.Now()
来源：http://bs.gzmigu.cn

Ruby: Time.now
来源：http://rb.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lk.jianghongdianzi.cn

[J02] 格式化输出
来源：http://sb.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gp.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://es.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.bjjhwx.cn

TS:   d.toISOString()
来源：http://ld.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nz.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oi.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xg.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://by.hnjuh.cn

[J03] 字符串解析为日期
来源：http://cz.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ss.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ie.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://pi.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ix.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fn.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jf.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://hy.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zd.nicolike.cn

[J04] 时间戳与日期互转
来源：http://gd.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ad.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hg.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wp.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pj.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ys.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fu.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fd.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ck.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://oz.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://xk.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gp.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fp.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hc.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://pl.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pb.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://cw.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wv.521024.cn

[J06] 计算两时间之差
来源：http://xf.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://yw.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://tb.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pr.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xx.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nf.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://iw.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://ej.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://za.haigaiapp.cn

[J07] 比较两个日期
来源：http://pa.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://bd.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://np.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kc.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uk.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wa.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ac.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jp.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ze.asd995.cn

[J08] 提取年月日与星期
来源：http://qb.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zv.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://py.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xh.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ew.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gt.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qw.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pr.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gv.wgjwhj.cn

[J09] 时区处理
来源：http://lb.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qc.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sy.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kf.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vs.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nh.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mf.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oc.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yf.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://kv.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ga.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lg.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vq.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cj.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gt.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zb.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hf.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dd.muxihuayi.cn

================================================================================
来源：http://qm.9csxet.cn

K. JSON 与序列化
来源：http://ie.hnjuh.cn

================================================================================
来源：http://iy.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://nv.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mc.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://if.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://pw.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://zz.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://og.9csxet.cn

Go:   json.Marshal(obj)
来源：http://gk.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zq.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nu.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ww.asd995.cn

Py:   json.loads(s)
来源：http://vk.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mw.panjiajie.cn

JS:   JSON.parse(s)
来源：http://sj.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://gz.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nv.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://xj.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://wd.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://al.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://iq.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kq.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vv.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://su.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xe.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yj.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iy.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sg.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mq.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://vl.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fe.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hb.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ym.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lt.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gt.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ex.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jo.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wa.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://su.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://cl.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://wb.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://yf.9csxet.cn

TS:   structuredClone(obj)
来源：http://cb.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vl.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dm.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kr.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cg.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://qt.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qf.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rf.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bh.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://do.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jm.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://af.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aq.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ik.hahajie.cn

[K07] 进制转换
来源：http://vd.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mw.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://px.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yk.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iv.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bk.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://si.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dj.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wp.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://zi.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://lf.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://un.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://bg.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://uo.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gj.hnjuh.cn

Go:   encoding/gob
来源：http://ym.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://ih.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jb.shxzskj.cn

================================================================================
来源：http://yr.colortex.cn

L. 网络请求
来源：http://th.newstarts.cn

================================================================================
来源：http://ky.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://gp.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ph.muxihuayi.cn


<!-- 参考信息 -->