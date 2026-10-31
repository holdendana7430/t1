代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bu.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://lm.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lc.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://pn.nicolike.cn

Py:   value = d.get("k") or default
来源：http://dk.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bu.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ol.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bs.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dr.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dz.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://vo.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://mb.asd995.cn

[H07] 断言
来源：http://ww.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ks.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://bu.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://dp.asd995.cn

TS:   console.assert(x > 0);
来源：http://ku.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://ax.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iv.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ow.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://bi.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://mz.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://xi.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pi.gzmigu.cn

JS:   e.message;  e.stack
来源：http://zn.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ct.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gq.nicolike.cn

Go:   err.Error()
来源：http://ts.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://jf.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://rd.gzmigu.cn

[H09] 带错误码的异常
来源：http://gp.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fl.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fw.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oi.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ju.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://an.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fh.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wj.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://el.shxzukj.cn

[H10] 资源自动释放
来源：http://hw.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ip.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bt.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ei.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kb.bjjhwx.cn

Go:   defer f.Close()
来源：http://sx.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zv.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mw.yuntaijiaju.cn

================================================================================
来源：http://ut.colortex.cn

I. 正则表达式
来源：http://jr.haigaiapp.cn

================================================================================
来源：http://tc.shtwfgs.cn

[I01] 判断是否匹配
来源：http://tw.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://im.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gw.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://xv.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://ha.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://di.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wu.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://gr.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://az.yuexingan06.cn

[I02] 提取所有匹配
来源：http://yu.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://na.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ym.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ax.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://lg.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kr.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wu.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://al.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rf.huixiangedu.cn

[I03] 提取捕获分组
来源：http://rt.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nq.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vq.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iz.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xc.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ez.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vr.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ls.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ht.jianghongdianzi.cn

[I04] 正则替换
来源：http://ef.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sv.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nl.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tt.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pl.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xl.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cy.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://be.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://id.lnxyls.cn

[I05] 按正则拆分
来源：http://sw.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sc.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vz.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://es.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://ak.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://jm.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rh.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cc.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jf.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mg.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sm.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yo.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aq.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fc.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qv.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vd.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nj.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gm.521024.cn

[I07] 忽略大小写与多行模式
来源：http://uk.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ra.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qz.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mn.szsharing.cn

TS:   /error/gim
来源：http://nl.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ix.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uu.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://pv.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vx.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://df.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bw.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vq.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ic.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ly.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pv.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kg.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://km.newstarts.cn

================================================================================
来源：http://rm.szxytkj.cn

J. 日期与时间
来源：http://qn.hahajie.cn

================================================================================
来源：http://lf.lnxyls.cn

[J01] 获取当前时间
来源：http://qm.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ck.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bz.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://pn.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ot.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ux.jctech888.com.cn

Go:   time.Now()
来源：http://rx.lnxyls.cn

Ruby: Time.now
来源：http://gn.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cs.shtwfgs.cn

[J02] 格式化输出
来源：http://ya.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yu.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://us.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gx.jctech888.com.cn

TS:   d.toISOString()
来源：http://oy.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hp.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ai.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cb.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mx.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://lk.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eu.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xq.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://ks.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://es.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xb.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pr.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://fc.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vo.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://qy.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jh.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ra.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://py.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gw.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://is.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lc.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mx.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://es.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ra.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://od.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://es.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qr.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zk.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ey.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oe.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://oh.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://my.panjiajie.cn

[J06] 计算两时间之差
来源：http://td.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://jx.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://sy.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wf.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hg.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zb.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://hv.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://qd.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://nv.nszjky.cn

[J07] 比较两个日期
来源：http://xn.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://pv.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bm.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ah.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tj.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ho.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://np.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://je.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ua.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://hz.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mc.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nt.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mt.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tx.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mm.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://az.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tu.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ew.yuntaijiaju.cn

[J09] 时区处理
来源：http://lh.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ta.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://to.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tb.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ef.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vx.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rm.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://js.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bx.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nq.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oa.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nq.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sg.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xz.panjiajie.cn

================================================================================
来源：http://af.colortex.cn

K. JSON 与序列化
来源：http://nj.huixiangedu.cn

================================================================================
来源：http://ig.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://mf.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nk.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dp.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://xk.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://rn.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ce.nszjky.cn

Go:   json.Marshal(obj)
来源：http://zy.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oo.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ca.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://xt.jctech888.com.cn

Py:   json.loads(s)
来源：http://kp.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kl.lnxyls.cn

JS:   JSON.parse(s)
来源：http://hz.gzmigu.cn

TS:   JSON.parse(s)
来源：http://lm.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://go.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://it.asd995.cn

Ruby: JSON.parse(s)
来源：http://ci.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qy.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://gq.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uf.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tb.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wl.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ei.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ft.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wf.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xd.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qf.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://mi.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xs.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dn.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hs.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bn.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qp.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bv.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vn.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ss.wgjwhj.cn

[K05] 深拷贝对象
来源：http://og.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://vc.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ub.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://zo.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://td.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ig.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nr.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://du.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://js.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://qh.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://np.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wu.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://np.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zi.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vs.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://om.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kn.asd995.cn

[K07] 进制转换
来源：http://nv.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sn.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yk.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yl.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ae.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xr.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sp.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zn.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cn.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://xe.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://qm.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ib.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://gg.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://qs.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pz.nicolike.cn

Go:   encoding/gob
来源：http://bt.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://fx.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jt.9csxet.cn

================================================================================
来源：http://vt.bookmarksfly.cn

L. 网络请求
来源：http://ti.huanxung.cn

================================================================================
来源：http://ei.szsharing.cn

[L01] 发送 GET 请求
来源：http://tl.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xp.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ea.nicolike.cn

JS:   await fetch(url)
来源：http://hs.asd995.cn

TS:   await fetch(url)
来源：http://qc.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oq.colortex.cn


<!-- 参考信息 -->