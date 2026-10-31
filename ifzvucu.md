代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wb.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://dm.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rr.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://cq.nszjky.cn

Py:   value = d.get("k") or default
来源：http://gc.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nx.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ol.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wz.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ci.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://go.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://pg.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://id.nicolike.cn

[H07] 断言
来源：http://wn.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://qx.9csxet.cn

PHP:  assert($x > 0);
来源：http://mg.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://sg.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://hl.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://bi.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hc.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eu.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://xh.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://ne.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://wv.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bw.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://ir.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sa.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://az.nicolike.cn

Go:   err.Error()
来源：http://dv.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://xx.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://xu.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://lj.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jn.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zj.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nl.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oh.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eu.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tj.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xc.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uk.wgjwhj.cn

[H10] 资源自动释放
来源：http://zc.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zs.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qa.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ik.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bx.hnjuh.cn

Go:   defer f.Close()
来源：http://ui.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jd.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fv.lnxyls.cn

================================================================================
来源：http://hh.jctech888.com.cn

I. 正则表达式
来源：http://bn.jianghongdianzi.cn

================================================================================
来源：http://lx.huanxung.cn

[I01] 判断是否匹配
来源：http://dx.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bw.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wy.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ky.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://ny.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aq.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tg.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://zu.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gw.521024.cn

[I02] 提取所有匹配
来源：http://ra.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://kj.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fj.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://be.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://bn.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kx.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lm.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://wk.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pq.9csxet.cn

[I03] 提取捕获分组
来源：http://fw.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zg.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gr.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tt.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qr.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ft.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jj.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ns.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://as.newstarts.cn

[I04] 正则替换
来源：http://yf.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lj.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ar.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uo.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ka.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jj.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zj.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wa.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mj.huixiangedu.cn

[I05] 按正则拆分
来源：http://oo.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ja.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fn.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://oi.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://bi.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ls.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fq.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tv.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tb.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cu.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ge.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mm.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jk.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dk.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qp.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pb.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cm.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ex.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://tg.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bb.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tu.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mi.9csxet.cn

TS:   /error/gim
来源：http://kl.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vm.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ch.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://fs.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://od.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://ze.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sz.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bl.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pt.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mg.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ye.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fr.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dp.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tm.jianghongdianzi.cn

================================================================================
来源：http://qp.colortex.cn

J. 日期与时间
来源：http://us.nszjky.cn

================================================================================
来源：http://wq.shxzukj.cn

[J01] 获取当前时间
来源：http://mt.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bq.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pm.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://xk.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://eu.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dh.shxzukj.cn

Go:   time.Now()
来源：http://zq.asd995.cn

Ruby: Time.now
来源：http://wn.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vj.nicolike.cn

[J02] 格式化输出
来源：http://rp.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sv.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eg.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nx.bjjhwx.cn

TS:   d.toISOString()
来源：http://qs.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yi.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zy.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bo.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tf.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://st.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ha.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uf.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://sw.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://xc.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rp.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dy.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://fp.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fq.9csxet.cn

[J04] 时间戳与日期互转
来源：http://yl.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://se.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fm.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://od.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hc.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://in.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wa.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wi.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gw.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ci.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://oh.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ga.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bh.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ux.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ga.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bi.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://qj.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uq.hahajie.cn

[J06] 计算两时间之差
来源：http://zx.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ew.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://uk.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xn.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://us.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://le.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://od.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://nr.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://bu.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://nb.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://rp.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mg.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gq.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nq.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://if.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ik.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://hf.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://wa.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qa.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gs.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ds.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ko.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dl.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lp.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ob.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ky.bookmarksfly.cn

[J09] 时区处理
来源：http://bu.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yd.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nn.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fx.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pm.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fh.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fv.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ng.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fs.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://yh.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mm.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bw.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kx.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yv.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hh.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://me.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fh.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://st.muxihuayi.cn

================================================================================
来源：http://db.huixinmuqiang.cn

K. JSON 与序列化
来源：http://qs.nicolike.cn

================================================================================
来源：http://ym.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://gd.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sk.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lh.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ic.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://cp.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qf.9csxet.cn

Go:   json.Marshal(obj)
来源：http://jc.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xq.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cj.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://sy.9csxet.cn

Py:   json.loads(s)
来源：http://po.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wn.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://lg.colortex.cn

TS:   JSON.parse(s)
来源：http://mt.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nd.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ua.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://dx.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eb.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://jx.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ui.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gm.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yr.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mh.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bl.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ib.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wt.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lo.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://oy.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fg.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wk.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bh.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yl.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bn.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qk.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wt.muxihuayi.cn

[K05] 深拷贝对象
来源：http://np.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://jo.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://bv.szsharing.cn

JS:   structuredClone(obj)
来源：http://wy.shxzskj.cn

TS:   structuredClone(obj)
来源：http://mi.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fk.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://az.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ou.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gm.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://uh.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gl.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pj.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jd.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yu.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bc.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gj.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jt.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dk.nicolike.cn

[K07] 进制转换
来源：http://pi.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yk.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gu.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jl.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uj.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ex.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cp.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qg.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ld.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://ul.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://qb.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sv.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://dc.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://kl.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ep.asd995.cn

Go:   encoding/gob
来源：http://mh.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://bg.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wj.huixinmuqiang.cn

================================================================================
来源：http://hm.huanxung.cn

L. 网络请求
来源：http://cz.yuntaijiaju.cn

================================================================================
来源：http://wg.hnjuh.cn

[L01] 发送 GET 请求
来源：http://rp.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bc.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hv.9csxet.cn

JS:   await fetch(url)
来源：http://rc.bjjhwx.cn

TS:   await fetch(url)
来源：http://zh.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dt.shxzukj.cn


<!-- 参考信息 -->