代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uy.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://bp.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://bb.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://zp.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://an.521024.cn

Ruby: rescue ArgumentError => e
来源：http://lm.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cy.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://ks.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://it.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ah.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://un.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sa.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ww.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pe.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://is.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://uu.panjiajie.cn

[H07] 断言
来源：http://ob.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://vz.szsharing.cn

PHP:  assert($x > 0);
来源：http://pl.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://ao.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://we.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://yz.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cm.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hk.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://fe.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://kq.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ps.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gv.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://jr.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xp.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ds.szsharing.cn

Go:   err.Error()
来源：http://qh.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ir.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://hw.bjjhwx.cn

[H09] 带错误码的异常
来源：http://oe.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vl.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fz.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cq.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sx.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mu.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gw.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ha.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jv.asd995.cn

[H10] 资源自动释放
来源：http://et.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pq.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gw.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xj.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nd.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ne.bookmarksfly.cn

Go:   defer f.Close()
来源：http://md.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pz.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qd.521024.cn

================================================================================
来源：http://qx.bookmarksfly.cn

I. 正则表达式
来源：http://hx.hnjuh.cn

================================================================================
来源：http://ma.newstarts.cn

[I01] 判断是否匹配
来源：http://yp.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cf.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xb.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://wj.newstarts.cn

TS:   /\d+/.test(s)
来源：http://oc.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ss.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://fp.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://es.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://fo.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://ni.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bq.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ap.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://qg.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gu.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fx.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://bh.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kl.9csxet.cn

[I03] 提取捕获分组
来源：http://ff.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kz.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wa.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kq.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nl.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zs.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wa.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ie.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tu.shxzskj.cn

[I04] 正则替换
来源：http://fk.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vd.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nw.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ly.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qs.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://og.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sx.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lc.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lq.szsharing.cn

[I05] 按正则拆分
来源：http://qm.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wv.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bc.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://nu.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://og.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://uq.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ld.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sc.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gm.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xd.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lq.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://to.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hd.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://io.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://te.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mj.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fu.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oe.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://bq.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://og.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ne.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mw.bookmarksfly.cn

TS:   /error/gim
来源：http://ef.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rw.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ug.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://fg.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ta.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://vo.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cw.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qm.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ks.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vt.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://al.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://he.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tu.colortex.cn

================================================================================
来源：http://gf.gzmigu.cn

J. 日期与时间
来源：http://ms.nicolike.cn

================================================================================
来源：http://ho.shxzukj.cn

[J01] 获取当前时间
来源：http://nc.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bb.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ts.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://uj.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://cb.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pl.szsharing.cn

Go:   time.Now()
来源：http://sl.huixiangedu.cn

Ruby: Time.now
来源：http://pf.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ft.yuexingan06.cn

[J02] 格式化输出
来源：http://iy.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rs.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fl.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wc.muxihuayi.cn

TS:   d.toISOString()
来源：http://js.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ns.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://si.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xc.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rb.colortex.cn

[J03] 字符串解析为日期
来源：http://aa.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lr.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rt.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://kz.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://fj.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ok.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ly.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://sb.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zt.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://co.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uf.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://us.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mj.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mw.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yz.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ia.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rx.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cy.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://og.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://zl.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cr.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nk.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://ap.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ei.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://gw.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rq.huanxung.cn

[J06] 计算两时间之差
来源：http://br.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://mn.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://mx.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mq.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yp.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ol.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://he.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://hd.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://in.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://ck.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://xh.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tb.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gr.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lc.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://me.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hh.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fl.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://tr.lnxyls.cn

[J08] 提取年月日与星期
来源：http://et.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xg.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zb.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://za.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lm.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fn.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mp.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fv.bjjhwx.cn

[J09] 时区处理
来源：http://jo.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pd.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lp.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xo.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cd.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jz.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tg.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ne.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://lx.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xv.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ed.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lt.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mi.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rb.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ts.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://so.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ia.lnxyls.cn

================================================================================
来源：http://uh.9csxet.cn

K. JSON 与序列化
来源：http://lq.bjjhwx.cn

================================================================================
来源：http://rm.521024.cn

[K01] 对象转 JSON 字符串
来源：http://xv.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://si.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://su.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://io.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://lv.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cq.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://mq.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ce.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gz.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://yf.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://rq.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bm.hnjuh.cn

JS:   JSON.parse(s)
来源：http://yv.gzmigu.cn

TS:   JSON.parse(s)
来源：http://po.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uf.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://xj.521024.cn

Ruby: JSON.parse(s)
来源：http://ql.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ht.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://it.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hn.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mz.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ik.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tt.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pr.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://je.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lm.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eu.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://hx.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ac.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bz.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zx.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gp.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fi.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uf.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lk.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://to.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://zv.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://cj.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://jn.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ow.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ly.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fo.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ox.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fi.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fs.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ad.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sd.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pi.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xe.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cu.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aw.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yf.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lu.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yb.hnjuh.cn

[K07] 进制转换
来源：http://lh.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uj.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fu.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xt.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bc.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hw.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cp.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ja.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://os.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://pb.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://dz.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fc.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://ah.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://pm.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bv.wgjwhj.cn

Go:   encoding/gob
来源：http://da.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://wa.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rc.jianghongdianzi.cn

================================================================================
来源：http://sz.yuntaijiaju.cn

L. 网络请求
来源：http://fa.shxzukj.cn

================================================================================
来源：http://es.szsharing.cn

[L01] 发送 GET 请求
来源：http://nf.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gm.huixiangedu.cn


<!-- 参考信息 -->