代发 wailian999

Py:   value = d.get("k") or default
来源：http://tm.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kn.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yk.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ny.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://us.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hd.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://qo.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://mc.hnjuh.cn

[H07] 断言
来源：http://lj.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://bc.shxzukj.cn

PHP:  assert($x > 0);
来源：http://uh.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://vi.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://ua.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://qj.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hr.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ow.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://xe.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://we.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://yt.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mh.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://yb.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xl.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cr.huixinmuqiang.cn

Go:   err.Error()
来源：http://fo.521024.cn

Ruby: e.message;  e.backtrace
来源：http://qs.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://uu.huixiangedu.cn

[H09] 带错误码的异常
来源：http://gw.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ko.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nf.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qa.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zg.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gf.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rh.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://go.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rq.szsharing.cn

[H10] 资源自动释放
来源：http://mr.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gb.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qz.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://th.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hn.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zd.huixiangedu.cn

Go:   defer f.Close()
来源：http://cw.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qs.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://he.szsharing.cn

================================================================================
来源：http://ot.szxytkj.cn

I. 正则表达式
来源：http://bx.huanxung.cn

================================================================================
来源：http://un.nicolike.cn

[I01] 判断是否匹配
来源：http://vj.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dt.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rf.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://kr.nszjky.cn

TS:   /\d+/.test(s)
来源：http://sh.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nx.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://km.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://hj.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uw.chemitech.net.cn

[I02] 提取所有匹配
来源：http://sp.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://it.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fa.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lq.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://px.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mi.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cn.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://ne.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mv.nszjky.cn

[I03] 提取捕获分组
来源：http://sq.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ay.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bp.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wc.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hk.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://by.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://br.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hp.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wl.haigaiapp.cn

[I04] 正则替换
来源：http://dn.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ma.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uw.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fd.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xa.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jx.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mj.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vt.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ab.shxzskj.cn

[I05] 按正则拆分
来源：http://ts.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ov.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vh.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://zn.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://cr.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ef.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bf.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sa.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hj.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cn.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pi.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bg.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kb.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gf.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://un.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nd.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://we.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ns.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://qg.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uf.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tz.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lp.muxihuayi.cn

TS:   /error/gim
来源：http://ic.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ve.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ve.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://tl.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://em.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://jm.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ii.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ev.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cu.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ru.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://re.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nc.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zb.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qz.shxzskj.cn

================================================================================
来源：http://rq.gzmigu.cn

J. 日期与时间
来源：http://pz.szxytkj.cn

================================================================================
来源：http://gf.szxytkj.cn

[J01] 获取当前时间
来源：http://yg.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jk.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lw.nszjky.cn

JS:   new Date();  Date.now()
来源：http://yr.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://hv.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uj.bjjhwx.cn

Go:   time.Now()
来源：http://jk.hnjuh.cn

Ruby: Time.now
来源：http://zb.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ai.shxzukj.cn

[J02] 格式化输出
来源：http://zy.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jj.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qe.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ze.newstarts.cn

TS:   d.toISOString()
来源：http://nv.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pu.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ue.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jg.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uz.nicolike.cn

[J03] 字符串解析为日期
来源：http://ix.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ft.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tu.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://kc.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://vh.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ux.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vi.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://hk.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://pr.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fu.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lh.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fk.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zz.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://io.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cp.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sv.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://qk.521024.cn

Py:   now + timedelta(days=7)
来源：http://fx.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://la.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kk.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ts.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://qi.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oz.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://qe.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://na.lnxyls.cn

[J06] 计算两时间之差
来源：http://rj.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://or.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://ei.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hq.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://et.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fu.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ur.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://pn.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://qp.bookmarksfly.cn

[J07] 比较两个日期
来源：http://ic.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ze.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rb.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://te.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ft.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ae.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pr.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ff.hahajie.cn

[J08] 提取年月日与星期
来源：http://ev.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ds.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ev.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ed.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bx.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ec.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://py.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gx.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ok.haigaiapp.cn

[J09] 时区处理
来源：http://ks.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ps.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hm.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://po.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ih.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yu.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ka.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ln.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://os.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xh.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://su.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bp.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fh.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uy.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rm.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tq.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fb.colortex.cn

================================================================================
来源：http://qb.szxytkj.cn

K. JSON 与序列化
来源：http://in.nszjky.cn

================================================================================
来源：http://zi.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://jl.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tq.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wg.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://tj.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://cb.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rr.colortex.cn

Go:   json.Marshal(obj)
来源：http://mf.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fz.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://un.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://pr.wgjwhj.cn

Py:   json.loads(s)
来源：http://cz.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dh.panjiajie.cn

JS:   JSON.parse(s)
来源：http://zi.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://jj.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ou.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://gk.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://zs.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yd.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://kb.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ob.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gh.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://py.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fv.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://du.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gc.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cg.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uk.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://oi.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yj.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ck.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://no.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gj.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://um.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hq.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ub.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gg.colortex.cn

[K05] 深拷贝对象
来源：http://ny.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://iz.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ut.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://xh.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://hh.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tj.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eu.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nm.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zg.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ty.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jx.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ff.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jg.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bi.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uc.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sm.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eh.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rn.hahajie.cn

[K07] 进制转换
来源：http://ae.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://db.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ax.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vf.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zq.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ou.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gm.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fu.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nn.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://dl.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://la.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dq.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ul.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://zb.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uu.shxzukj.cn

Go:   encoding/gob
来源：http://mg.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://dw.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sq.yuexingan06.cn

================================================================================
来源：http://gv.szxytkj.cn

L. 网络请求
来源：http://tw.asd995.cn

================================================================================
来源：http://ku.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://xq.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sk.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ll.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://rv.lnxyls.cn

TS:   await fetch(url)
来源：http://cg.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ze.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://zt.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://om.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xd.lnxyls.cn

[L02] 发送 POST JSON
来源：http://jk.bookmarksfly.cn


<!-- 参考信息 -->