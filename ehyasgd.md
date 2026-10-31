代发 wailian999

Py:   value = d.get("k") or default
来源：http://wl.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zg.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gl.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ba.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://as.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://po.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ic.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://ko.szxytkj.cn

[H07] 断言
来源：http://rk.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://bu.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://hf.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://ez.huanxung.cn

TS:   console.assert(x > 0);
来源：http://fa.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://wh.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nl.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qd.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ju.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://rh.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://uj.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wh.hahajie.cn

JS:   e.message;  e.stack
来源：http://es.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cs.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sw.521024.cn

Go:   err.Error()
来源：http://us.521024.cn

Ruby: e.message;  e.backtrace
来源：http://wy.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://eq.nicolike.cn

[H09] 带错误码的异常
来源：http://mr.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qq.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fs.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gk.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mp.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ni.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iq.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qk.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://br.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://fb.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ex.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ca.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sv.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://re.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ih.nicolike.cn

Go:   defer f.Close()
来源：http://rk.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ox.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zi.jctech888.com.cn

================================================================================
来源：http://fv.newstarts.cn

I. 正则表达式
来源：http://ch.jctech888.com.cn

================================================================================
来源：http://tx.szsharing.cn

[I01] 判断是否匹配
来源：http://pq.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://er.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pg.huanxung.cn

JS:   /\d+/.test(s)
来源：http://bf.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://ra.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tz.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yb.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://mp.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pe.jctech888.com.cn

[I02] 提取所有匹配
来源：http://pc.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://fo.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sq.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cx.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://jb.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oq.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pd.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qe.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://op.muxihuayi.cn

[I03] 提取捕获分组
来源：http://pk.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vm.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zk.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://db.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qp.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hf.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nm.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ic.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jb.newstarts.cn

[I04] 正则替换
来源：http://xi.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://le.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uc.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hj.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vc.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iz.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xp.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jy.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mf.asd995.cn

[I05] 按正则拆分
来源：http://he.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://px.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ah.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://vt.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://dm.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://bh.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lf.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fa.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pf.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pf.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fk.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pi.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ki.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pk.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wd.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://va.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bw.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fm.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://uu.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hr.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pq.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dt.asd995.cn

TS:   /error/gim
来源：http://qi.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ko.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kc.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://wv.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lx.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://fv.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://di.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://td.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://us.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xx.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lq.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mz.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hw.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uc.haigaiapp.cn

================================================================================
来源：http://rn.haigaiapp.cn

J. 日期与时间
来源：http://ro.szxytkj.cn

================================================================================
来源：http://vv.wgjwhj.cn

[J01] 获取当前时间
来源：http://rm.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nv.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ru.521024.cn

JS:   new Date();  Date.now()
来源：http://ha.9csxet.cn

TS:   new Date();  Date.now()
来源：http://nm.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ie.hnjuh.cn

Go:   time.Now()
来源：http://zs.yuexingan06.cn

Ruby: Time.now
来源：http://wg.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yi.newstarts.cn

[J02] 格式化输出
来源：http://bs.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ez.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qd.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ou.hahajie.cn

TS:   d.toISOString()
来源：http://hm.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fp.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zu.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gr.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://me.huanxung.cn

[J03] 字符串解析为日期
来源：http://qb.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jb.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qf.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://qt.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://an.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ts.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ge.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ys.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bk.nszjky.cn

[J04] 时间戳与日期互转
来源：http://ko.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kc.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ih.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ad.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nj.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gx.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yq.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dc.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rg.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://bc.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://xq.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://da.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kn.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xw.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://qe.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aa.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://zv.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gh.nicolike.cn

[J06] 计算两时间之差
来源：http://rv.521024.cn

Py:   (end - start).total_seconds()
来源：http://jo.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ko.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gh.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bh.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bj.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://ql.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://rn.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://sb.shxzskj.cn

[J07] 比较两个日期
来源：http://qb.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://wi.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cn.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ln.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gr.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cy.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ig.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bh.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://mx.nszjky.cn

[J08] 提取年月日与星期
来源：http://tz.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mw.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nw.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gq.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cx.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://go.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yg.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://up.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ga.9csxet.cn

[J09] 时区处理
来源：http://ln.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yv.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ow.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mp.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eg.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ba.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aa.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gk.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://hx.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sz.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uo.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ms.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ir.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://at.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hy.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ur.szsharing.cn

================================================================================
来源：http://gx.newstarts.cn

K. JSON 与序列化
来源：http://zs.huixiangedu.cn

================================================================================
来源：http://is.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://ej.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ei.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zq.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://bq.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://pw.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rk.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://zn.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gf.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hg.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://lw.shxzukj.cn

Py:   json.loads(s)
来源：http://gi.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fm.lnxyls.cn

JS:   JSON.parse(s)
来源：http://bw.asd995.cn

TS:   JSON.parse(s)
来源：http://mr.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lu.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://qu.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://xo.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://so.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://nx.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nv.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ie.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://up.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ek.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kq.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dy.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xn.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ou.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pe.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zw.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ss.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gl.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dy.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ao.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://du.hnjuh.cn

[K05] 深拷贝对象
来源：http://lj.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://id.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://um.szsharing.cn

JS:   structuredClone(obj)
来源：http://jb.panjiajie.cn

TS:   structuredClone(obj)
来源：http://nl.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jd.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xf.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tb.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lw.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://qx.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nx.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xl.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ud.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wc.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gu.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aw.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://na.bookmarksfly.cn

[K07] 进制转换
来源：http://gw.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ek.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kq.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pg.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mv.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://va.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fm.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cl.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qd.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://cd.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://ms.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qu.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://sr.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://zk.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ny.wgjwhj.cn

Go:   encoding/gob
来源：http://xy.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://xy.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dr.9csxet.cn

================================================================================
来源：http://qe.bookmarksfly.cn

L. 网络请求
来源：http://hv.nicolike.cn

================================================================================
来源：http://yq.panjiajie.cn

[L01] 发送 GET 请求
来源：http://jk.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vd.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bi.jctech888.com.cn

JS:   await fetch(url)
来源：http://lb.szsharing.cn

TS:   await fetch(url)
来源：http://kd.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yb.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://am.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fd.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rq.521024.cn

[L02] 发送 POST JSON
来源：http://so.asd995.cn


<!-- 参考信息 -->