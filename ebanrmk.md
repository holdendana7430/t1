代发 wailian999

Py:   value = d.get("k") or default
来源：http://cb.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sx.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lt.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://by.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kq.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pa.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://bd.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://ys.gzmigu.cn

[H07] 断言
来源：http://hq.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://lu.szxytkj.cn

PHP:  assert($x > 0);
来源：http://fl.521024.cn

JS:   console.assert(x > 0);
来源：http://wm.colortex.cn

TS:   console.assert(x > 0);
来源：http://vx.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://dp.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xb.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ge.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://pc.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://kc.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://zq.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dz.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://lz.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ke.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zm.yuexingan06.cn

Go:   err.Error()
来源：http://fp.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://qc.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://gu.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://rj.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://be.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bx.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xp.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bj.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ju.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qt.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ml.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jg.shxzukj.cn

[H10] 资源自动释放
来源：http://zn.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pu.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dw.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zv.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xj.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vm.haigaiapp.cn

Go:   defer f.Close()
来源：http://tx.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zh.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://su.gzmigu.cn

I. 正则表达式
来源：http://bh.wgjwhj.cn

================================================================================
来源：http://od.jctech888.com.cn

[I01] 判断是否匹配
来源：http://er.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://la.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xo.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://ee.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://oi.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ao.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jh.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://hr.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zy.asd995.cn

[I02] 提取所有匹配
来源：http://am.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://uv.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gv.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://or.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://bg.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dc.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ty.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://lf.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dy.521024.cn

[I03] 提取捕获分组
来源：http://nz.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://px.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vq.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qt.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oz.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ua.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qj.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://es.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vu.hnjuh.cn

[I04] 正则替换
来源：http://zh.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qh.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bd.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://er.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fr.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://te.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hr.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hd.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pq.nszjky.cn

[I05] 按正则拆分
来源：http://vu.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sk.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pb.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ig.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yj.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ok.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yj.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kl.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zo.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ar.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ou.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qj.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vm.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mr.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ho.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ra.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mp.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gg.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://jr.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ed.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kd.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wp.nszjky.cn

TS:   /error/gim
来源：http://tf.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iu.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vo.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://du.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vg.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://dh.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ec.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qx.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jn.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xd.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jg.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eo.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ph.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://py.haigaiapp.cn

================================================================================
来源：http://uf.shxzskj.cn

J. 日期与时间
来源：http://mu.haigaiapp.cn

================================================================================
来源：http://wm.szxytkj.cn

[J01] 获取当前时间
来源：http://sa.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://li.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fo.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ue.colortex.cn

TS:   new Date();  Date.now()
来源：http://vq.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wj.bjjhwx.cn

Go:   time.Now()
来源：http://yb.shxzskj.cn

Ruby: Time.now
来源：http://cr.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kf.521024.cn

[J02] 格式化输出
来源：http://pv.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gz.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ht.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://po.shxzukj.cn

TS:   d.toISOString()
来源：http://yr.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kc.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eh.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sa.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vl.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://me.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xn.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xw.521024.cn

JS:   new Date("2024-01-02")
来源：http://yz.colortex.cn

TS:   new Date("2024-01-02")
来源：http://un.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lq.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iu.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://jw.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://in.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://ib.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eo.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nd.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kv.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mr.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cu.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://un.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://er.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://os.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://vj.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ik.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mu.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pq.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mh.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xz.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eq.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://qm.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://px.hnjuh.cn

[J06] 计算两时间之差
来源：http://an.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://tb.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://if.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zl.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mb.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jq.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://ui.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://xf.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://of.nszjky.cn

[J07] 比较两个日期
来源：http://ub.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://qd.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mm.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qb.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ab.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jy.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ij.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ru.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://uy.shxzukj.cn

[J08] 提取年月日与星期
来源：http://lm.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://op.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ph.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yo.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://os.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uz.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dl.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ge.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yh.521024.cn

[J09] 时区处理
来源：http://pi.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ma.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zf.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://or.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xs.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tw.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dq.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zb.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ye.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://oi.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fz.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mz.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oa.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tn.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gm.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vb.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rb.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wg.nicolike.cn

================================================================================
来源：http://qv.colortex.cn

K. JSON 与序列化
来源：http://fz.nicolike.cn

================================================================================
来源：http://jk.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ek.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cd.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xm.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://uu.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://jd.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bn.hahajie.cn

Go:   json.Marshal(obj)
来源：http://om.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ll.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ln.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://vi.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://dh.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ti.panjiajie.cn

JS:   JSON.parse(s)
来源：http://zn.lnxyls.cn

TS:   JSON.parse(s)
来源：http://gi.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xc.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://hh.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://di.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pk.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://ki.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ke.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vw.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lq.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sc.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kf.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bu.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sr.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eg.huanxung.cn

[K04] 读取 JSON 文件
来源：http://ss.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kr.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rp.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fl.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ux.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fw.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ko.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sl.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://to.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://gu.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://di.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://dm.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://lv.gzmigu.cn

TS:   structuredClone(obj)
来源：http://yt.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://or.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zp.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bq.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ha.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://gg.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gk.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://he.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sc.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yr.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uy.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://av.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ap.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yl.haigaiapp.cn

[K07] 进制转换
来源：http://hv.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://me.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://om.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zd.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dm.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xa.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uu.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qe.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xc.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gj.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://zy.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ak.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://gl.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ly.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yp.newstarts.cn

Go:   encoding/gob
来源：http://bg.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://wu.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lf.shxzukj.cn

================================================================================
来源：http://st.haigaiapp.cn

L. 网络请求
来源：http://bl.hnjuh.cn

================================================================================
来源：http://lg.szsharing.cn

[L01] 发送 GET 请求
来源：http://ka.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uq.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hb.hahajie.cn

JS:   await fetch(url)
来源：http://td.asd995.cn

TS:   await fetch(url)
来源：http://zp.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://on.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://vo.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vj.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ho.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://im.colortex.cn


<!-- 参考信息 -->