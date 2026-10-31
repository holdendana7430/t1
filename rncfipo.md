代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iz.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rv.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://vg.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://sn.shxzukj.cn

[H07] 断言
来源：http://mp.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://yp.hahajie.cn

PHP:  assert($x > 0);
来源：http://ms.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://op.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://fu.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://bl.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jx.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kf.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://gt.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://mu.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://se.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dr.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://hu.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ve.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://du.lnxyls.cn

Go:   err.Error()
来源：http://ud.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://wx.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://ch.nszjky.cn

[H09] 带错误码的异常
来源：http://wl.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mg.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mp.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xz.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ij.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pu.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mw.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ha.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wb.haigaiapp.cn

[H10] 资源自动释放
来源：http://xk.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ze.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pp.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hp.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cq.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xt.yuexingan06.cn

Go:   defer f.Close()
来源：http://tg.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kx.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vq.shtwfgs.cn

================================================================================
来源：http://ok.panjiajie.cn

I. 正则表达式
来源：http://eq.wgjwhj.cn

================================================================================
来源：http://fj.nicolike.cn

[I01] 判断是否匹配
来源：http://kq.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ur.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ew.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://sh.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://to.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cc.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gc.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://oz.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://da.hnjuh.cn

[I02] 提取所有匹配
来源：http://xf.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://jh.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rd.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ow.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://rm.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qi.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xu.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ke.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pj.huanxung.cn

[I03] 提取捕获分组
来源：http://of.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oa.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qf.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xo.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wl.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rp.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jw.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ae.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ay.shxzukj.cn

[I04] 正则替换
来源：http://xy.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://go.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ym.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cl.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qf.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uw.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qk.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://th.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://og.szsharing.cn

[I05] 按正则拆分
来源：http://go.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ss.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cb.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bt.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://lz.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://vv.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ar.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ny.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fs.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gz.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jw.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xx.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eh.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://la.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bc.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cl.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zu.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://li.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://pl.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ce.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eg.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lg.wgjwhj.cn

TS:   /error/gim
来源：http://ck.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mn.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pr.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://wv.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xw.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://zp.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uc.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://of.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cm.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pv.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ke.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://di.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sn.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pd.lnxyls.cn

================================================================================
来源：http://kb.lnxyls.cn

J. 日期与时间
来源：http://zv.nicolike.cn

================================================================================
来源：http://za.huixiangedu.cn

[J01] 获取当前时间
来源：http://aw.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ml.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ul.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://lu.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://zs.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gj.chemitech.net.cn

Go:   time.Now()
来源：http://jz.bookmarksfly.cn

Ruby: Time.now
来源：http://yi.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nt.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ae.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pc.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dm.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mj.hahajie.cn

TS:   d.toISOString()
来源：http://dl.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dq.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pi.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fl.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://us.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://kw.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jp.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mb.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://ag.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://rv.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ks.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vp.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://dn.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cs.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ah.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ak.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pq.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fx.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bo.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kj.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://os.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://li.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wn.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://uq.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://hq.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://im.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wy.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vm.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://eb.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gl.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://wc.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qy.haigaiapp.cn

[J06] 计算两时间之差
来源：http://ko.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ca.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://ir.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hf.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fu.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://os.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://yr.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://vl.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://uc.shxzukj.cn

[J07] 比较两个日期
来源：http://am.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://pg.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yz.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gw.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yq.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ga.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pu.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kt.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://fi.gzmigu.cn

[J08] 提取年月日与星期
来源：http://uf.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rx.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gb.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ya.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fi.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cy.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rz.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dv.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sx.szsharing.cn

[J09] 时区处理
来源：http://lh.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oc.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ea.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xt.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fw.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fe.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ks.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://mx.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fs.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vf.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fp.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ek.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xs.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://os.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uq.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xb.szsharing.cn

================================================================================
来源：http://nn.huixiangedu.cn

K. JSON 与序列化
来源：http://fl.gzmigu.cn

================================================================================
来源：http://hk.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://zw.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ec.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nr.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://zt.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://cw.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nd.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://au.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gw.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://at.nicolike.cn

[K02] JSON 字符串转对象
来源：http://vb.shtwfgs.cn

Py:   json.loads(s)
来源：http://kj.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://me.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://px.hahajie.cn

TS:   JSON.parse(s)
来源：http://st.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ws.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://mm.colortex.cn

Ruby: JSON.parse(s)
来源：http://xo.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tx.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://av.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pl.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dw.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fi.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yi.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zz.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dp.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ko.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kj.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://ui.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qk.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kh.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ds.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oy.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tx.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gx.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ro.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ba.panjiajie.cn

[K05] 深拷贝对象
来源：http://wt.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://ic.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://ax.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://rm.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://td.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xt.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ve.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oy.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fu.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://kx.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lb.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://su.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gh.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kj.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hq.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zo.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tt.haigaiapp.cn

[K07] 进制转换
来源：http://of.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wu.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jd.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zo.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pq.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qh.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ph.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bq.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zc.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://os.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://we.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ea.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://xr.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://bl.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ue.jianghongdianzi.cn

Go:   encoding/gob
来源：http://pt.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://nw.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gi.nicolike.cn

================================================================================
来源：http://ho.wgjwhj.cn

L. 网络请求
来源：http://dh.yuntaijiaju.cn

================================================================================
来源：http://vy.huanxung.cn

[L01] 发送 GET 请求
来源：http://tz.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wc.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hl.szsharing.cn

JS:   await fetch(url)
来源：http://ig.jctech888.com.cn

TS:   await fetch(url)
来源：http://ee.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gv.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://wi.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://py.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tp.colortex.cn

[L02] 发送 POST JSON
来源：http://es.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bz.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tj.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://if.shxzukj.cn


<!-- 参考信息 -->