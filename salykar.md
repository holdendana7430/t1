代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yo.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://gk.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xf.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://mj.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://zq.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://li.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xm.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lk.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://km.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qi.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://fc.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://zy.colortex.cn

[H07] 断言
来源：http://gl.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://yu.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://cw.huanxung.cn

JS:   console.assert(x > 0);
来源：http://jv.huanxung.cn

TS:   console.assert(x > 0);
来源：http://vj.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://ot.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://es.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fk.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://eb.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://du.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://wr.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ic.shxzskj.cn

JS:   e.message;  e.stack
来源：http://en.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hm.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vm.bjjhwx.cn

Go:   err.Error()
来源：http://up.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://me.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://mp.hnjuh.cn

[H09] 带错误码的异常
来源：http://yh.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wd.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kw.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vu.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yh.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qu.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lk.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ra.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rf.hahajie.cn

[H10] 资源自动释放
来源：http://da.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vp.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://md.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bf.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://et.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://sl.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ip.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://er.huanxung.cn

================================================================================
来源：http://qu.yuexingan06.cn

I. 正则表达式
来源：http://hj.yuntaijiaju.cn

================================================================================
来源：http://kd.panjiajie.cn

[I01] 判断是否匹配
来源：http://bp.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ex.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://su.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://rz.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://kk.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wa.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dd.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://oz.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.haigaiapp.cn

[I02] 提取所有匹配
来源：http://yh.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://ie.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hy.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qj.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://fn.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wq.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://id.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://uv.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://as.huixiangedu.cn

[I03] 提取捕获分组
来源：http://eo.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://af.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://db.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lv.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hd.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yq.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sc.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ma.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qg.shxzskj.cn

[I04] 正则替换
来源：http://hl.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xk.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lj.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ao.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fp.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qk.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kf.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fu.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nf.gzmigu.cn

[I05] 按正则拆分
来源：http://nd.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cc.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ur.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qf.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ur.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://mr.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rr.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://df.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ud.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oh.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lj.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ta.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wn.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jl.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bn.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ku.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yc.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kq.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://al.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bj.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oj.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mz.yuexingan06.cn

TS:   /error/gim
来源：http://ym.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jc.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vn.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://cw.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tn.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://kb.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uh.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://os.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hl.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ie.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ks.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ia.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rh.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://me.shxzukj.cn

================================================================================
来源：http://gh.jctech888.com.cn

J. 日期与时间
来源：http://hg.newstarts.cn

================================================================================
来源：http://mr.szxytkj.cn

[J01] 获取当前时间
来源：http://bd.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ii.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zg.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://oz.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://tf.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tl.wgjwhj.cn

Go:   time.Now()
来源：http://lj.yuntaijiaju.cn

Ruby: Time.now
来源：http://pb.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fj.huixiangedu.cn

[J02] 格式化输出
来源：http://lw.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qg.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tm.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fc.huanxung.cn

TS:   d.toISOString()
来源：http://zl.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ry.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hc.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sk.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zu.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ei.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ov.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sr.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://qr.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://mw.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tn.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fz.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://aw.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ym.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://vn.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rw.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kh.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qp.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zq.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://al.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eo.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sy.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vg.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://lm.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://wb.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vg.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ol.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://ts.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ij.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ij.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iq.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://zz.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://kd.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://cd.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ge.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ox.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mj.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://iu.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://rj.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://xa.szxytkj.cn

[J07] 比较两个日期
来源：http://gp.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://oy.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gw.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xl.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kx.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mr.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gx.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://up.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://kb.hnjuh.cn

[J08] 提取年月日与星期
来源：http://fi.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sa.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yu.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vp.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zg.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://th.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://me.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rl.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ko.wgjwhj.cn

[J09] 时区处理
来源：http://fh.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pv.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qr.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pt.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jg.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sn.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zw.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dl.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bt.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://wc.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jc.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cd.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jg.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pu.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dq.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mn.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mz.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vw.gzmigu.cn

================================================================================
来源：http://tf.shtwfgs.cn

K. JSON 与序列化
来源：http://ho.huanxung.cn

================================================================================
来源：http://fy.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://ag.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://it.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ih.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://lr.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://rr.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vj.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://em.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://he.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jm.nicolike.cn

[K02] JSON 字符串转对象
来源：http://pw.yuexingan06.cn

Py:   json.loads(s)
来源：http://de.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://op.colortex.cn

JS:   JSON.parse(s)
来源：http://yt.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://iq.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rz.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://xx.9csxet.cn

Ruby: JSON.parse(s)
来源：http://hi.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kl.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zj.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bi.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ne.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qz.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tw.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xn.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://op.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ln.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gw.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://ju.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zg.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vl.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ky.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sq.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://al.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ai.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://av.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rx.hnjuh.cn

[K05] 深拷贝对象
来源：http://oy.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://hi.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://nc.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://po.9csxet.cn

TS:   structuredClone(obj)
来源：http://ml.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hx.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yo.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ke.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wj.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://xs.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dp.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uh.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cy.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jo.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ho.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gk.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fs.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dh.szxytkj.cn

[K07] 进制转换
来源：http://ww.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nj.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gu.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qd.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yv.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mz.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ed.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ds.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kz.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://pc.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zy.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://jv.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://uj.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qv.nszjky.cn

Go:   encoding/gob
来源：http://kf.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ll.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zj.szsharing.cn

================================================================================
来源：http://fs.panjiajie.cn

L. 网络请求
来源：http://da.hnjuh.cn

================================================================================
来源：http://pn.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://ht.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xr.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nq.jctech888.com.cn

JS:   await fetch(url)
来源：http://qe.newstarts.cn

TS:   await fetch(url)
来源：http://kq.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://di.lnxyls.cn


<!-- 参考信息 -->