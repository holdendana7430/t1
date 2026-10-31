代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://le.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://rc.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://dt.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ed.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mm.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://pd.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ag.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://kx.nicolike.cn

Py:   value = d.get("k") or default
来源：http://nw.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qi.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fs.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vs.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ti.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bi.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://hc.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://mz.hnjuh.cn

[H07] 断言
来源：http://pz.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://gj.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://jl.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://ng.colortex.cn

TS:   console.assert(x > 0);
来源：http://xg.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ag.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fl.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ly.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://rg.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://ha.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://kh.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qf.newstarts.cn

JS:   e.message;  e.stack
来源：http://op.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zt.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ri.lnxyls.cn

Go:   err.Error()
来源：http://jx.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://hk.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://ik.hnjuh.cn

[H09] 带错误码的异常
来源：http://bc.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gt.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dt.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xt.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oc.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://un.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://be.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zy.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hi.jctech888.com.cn

[H10] 资源自动释放
来源：http://xl.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ks.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xg.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://it.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wi.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ug.hnjuh.cn

Go:   defer f.Close()
来源：http://bd.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dl.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jl.shxzskj.cn

================================================================================
来源：http://yb.nicolike.cn

I. 正则表达式
来源：http://ui.shxzukj.cn

================================================================================
来源：http://hv.szsharing.cn

[I01] 判断是否匹配
来源：http://px.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jy.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ka.521024.cn

JS:   /\d+/.test(s)
来源：http://cr.asd995.cn

TS:   /\d+/.test(s)
来源：http://vt.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tx.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sf.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://eb.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ls.huanxung.cn

[I02] 提取所有匹配
来源：http://lz.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://va.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nv.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eb.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://nn.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bh.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ac.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://vj.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oq.lnxyls.cn

[I03] 提取捕获分组
来源：http://wh.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rg.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tw.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gg.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ob.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zs.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oa.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fz.newstarts.cn

[I04] 正则替换
来源：http://mn.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fi.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zu.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hc.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lz.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xv.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zl.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://az.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nv.hahajie.cn

[I05] 按正则拆分
来源：http://ao.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qk.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jj.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qj.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://sg.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://ab.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fn.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dj.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://li.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cp.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zf.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://za.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xv.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kx.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ky.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lh.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kp.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://js.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://em.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bw.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jq.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vp.shxzukj.cn

TS:   /error/gim
来源：http://wj.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://is.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dj.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://at.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ir.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ml.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ru.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wn.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yc.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ac.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rf.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yf.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pl.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bp.panjiajie.cn

================================================================================
来源：http://mr.yuntaijiaju.cn

J. 日期与时间
来源：http://ml.chemitech.net.cn

================================================================================
来源：http://nc.hnjuh.cn

[J01] 获取当前时间
来源：http://im.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ge.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vi.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://vt.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://bb.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mw.newstarts.cn

Go:   time.Now()
来源：http://ha.nicolike.cn

Ruby: Time.now
来源：http://dc.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://te.shxzskj.cn

[J02] 格式化输出
来源：http://ci.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vc.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mu.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oj.shxzskj.cn

TS:   d.toISOString()
来源：http://fv.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://at.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://it.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nd.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xf.lnxyls.cn

[J03] 字符串解析为日期
来源：http://jt.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://au.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nn.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ks.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://eu.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ik.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uw.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ej.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dj.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://xz.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kb.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ht.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yn.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ie.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ul.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rk.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nk.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ht.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://ji.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://cu.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pl.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nr.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ui.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ip.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://uu.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fj.chemitech.net.cn

[J06] 计算两时间之差
来源：http://nk.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://um.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://pc.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uz.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://by.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hv.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://uv.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://wh.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://un.huixiangedu.cn

[J07] 比较两个日期
来源：http://um.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://en.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mm.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://if.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vl.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://av.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pf.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gu.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://jl.hnjuh.cn

[J08] 提取年月日与星期
来源：http://xl.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ro.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pu.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ah.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ve.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ql.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wb.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pd.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.yuexingan06.cn

[J09] 时区处理
来源：http://qg.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hx.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fi.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eg.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dd.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://in.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zz.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bo.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://np.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://ba.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qh.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gk.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ao.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lr.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pv.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://se.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hx.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dn.lnxyls.cn

================================================================================
来源：http://bf.muxihuayi.cn

K. JSON 与序列化
来源：http://ud.nszjky.cn

================================================================================
来源：http://sf.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://os.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lz.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tr.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ep.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://vk.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://op.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://zk.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://in.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cn.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://nd.szsharing.cn

Py:   json.loads(s)
来源：http://zb.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vb.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://zh.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://zv.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fh.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://km.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ox.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lm.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://tt.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sw.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ky.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pi.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vl.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://on.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ne.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aw.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gf.hahajie.cn

[K04] 读取 JSON 文件
来源：http://th.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yx.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vx.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mu.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://su.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://is.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jz.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pn.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://wl.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://pp.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://kz.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://vn.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://vj.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ux.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lg.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kt.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gx.szsharing.cn

[K06] 解析 URL 查询串
来源：http://gm.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ir.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pc.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ke.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rr.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zu.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xj.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xi.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://px.shxzukj.cn

[K07] 进制转换
来源：http://gb.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fd.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://je.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fs.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kg.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bh.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://br.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nc.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://px.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ky.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://bf.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cc.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ud.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://kf.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jf.9csxet.cn

Go:   encoding/gob
来源：http://aw.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://ek.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wa.panjiajie.cn

================================================================================
来源：http://jx.newstarts.cn

L. 网络请求
来源：http://ak.hahajie.cn

================================================================================
来源：http://lq.521024.cn

[L01] 发送 GET 请求
来源：http://ks.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://om.yuntaijiaju.cn


<!-- 参考信息 -->