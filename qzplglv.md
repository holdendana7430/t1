代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fr.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://jo.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qt.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://qh.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://rr.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rb.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gr.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qn.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rd.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gh.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://yl.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://mi.muxihuayi.cn

[H07] 断言
来源：http://td.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://es.szxytkj.cn

PHP:  assert($x > 0);
来源：http://zj.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://sb.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://eo.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://vu.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vu.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bw.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://af.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://rl.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://hd.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qk.panjiajie.cn

JS:   e.message;  e.stack
来源：http://wn.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gc.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qa.bookmarksfly.cn

Go:   err.Error()
来源：http://uf.521024.cn

Ruby: e.message;  e.backtrace
来源：http://ku.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://ou.lnxyls.cn

[H09] 带错误码的异常
来源：http://dc.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hi.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://np.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yj.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ue.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mx.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oq.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vk.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ot.shtwfgs.cn

[H10] 资源自动释放
来源：http://uu.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iz.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ue.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ix.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pk.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://df.yuexingan06.cn

Go:   defer f.Close()
来源：http://xq.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pm.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fe.newstarts.cn

================================================================================
来源：http://ee.wgjwhj.cn

I. 正则表达式
来源：http://xc.yuexingan06.cn

================================================================================
来源：http://dh.asd995.cn

[I01] 判断是否匹配
来源：http://zh.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vk.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pf.colortex.cn

JS:   /\d+/.test(s)
来源：http://ez.nszjky.cn

TS:   /\d+/.test(s)
来源：http://ut.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ti.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vu.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://jp.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ok.hahajie.cn

[I02] 提取所有匹配
来源：http://rj.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ku.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pg.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ty.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://ml.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yi.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://gr.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fr.huanxung.cn

[I03] 提取捕获分组
来源：http://oy.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://np.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fk.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qm.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://og.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cl.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fi.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zd.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ki.szsharing.cn

[I04] 正则替换
来源：http://tp.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sc.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jl.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oi.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ga.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dc.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xb.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zp.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://te.haigaiapp.cn

[I05] 按正则拆分
来源：http://eg.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ka.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xp.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://mp.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://lb.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://oq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ja.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bj.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yj.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zt.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hl.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://na.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bc.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yu.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fe.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mj.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uw.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tq.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://ni.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ah.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://we.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sh.colortex.cn

TS:   /error/gim
来源：http://kw.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dn.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ke.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://yl.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://er.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://hj.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fy.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mr.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lb.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lp.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://in.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zi.bjjhwx.cn

================================================================================
来源：http://zq.shxzukj.cn

J. 日期与时间
来源：http://xn.jianghongdianzi.cn

================================================================================
来源：http://mh.hnjuh.cn

[J01] 获取当前时间
来源：http://wg.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://op.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cm.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://vb.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://il.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lh.lnxyls.cn

Go:   time.Now()
来源：http://gt.shtwfgs.cn

Ruby: Time.now
来源：http://ih.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ws.yuexingan06.cn

[J02] 格式化输出
来源：http://ic.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ti.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ew.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.wgjwhj.cn

TS:   d.toISOString()
来源：http://wt.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://am.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wg.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://az.nszjky.cn

[J03] 字符串解析为日期
来源：http://zf.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://la.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qv.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://sg.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://iz.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wz.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gl.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://ls.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lv.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://kh.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jj.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hk.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ks.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zb.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fl.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tj.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ix.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ok.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://jz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://zz.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gz.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rj.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ef.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://pc.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vz.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://nm.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://on.lnxyls.cn

[J06] 计算两时间之差
来源：http://kd.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://gl.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://wm.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pu.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ri.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kv.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://ed.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://ig.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://eu.shxzukj.cn

[J07] 比较两个日期
来源：http://ck.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://ut.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lz.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pz.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ne.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vl.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hq.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sv.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ca.nszjky.cn

[J08] 提取年月日与星期
来源：http://kt.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nl.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bk.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iy.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uj.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vs.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ph.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hf.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qj.521024.cn

[J09] 时区处理
来源：http://sv.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vu.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fb.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://de.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fw.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xr.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mk.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uy.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ra.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://jw.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jp.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fp.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zx.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qs.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hi.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ws.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://do.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tv.hahajie.cn

================================================================================
来源：http://ue.bookmarksfly.cn

K. JSON 与序列化
来源：http://hs.lnxyls.cn

================================================================================
来源：http://xi.521024.cn

[K01] 对象转 JSON 字符串
来源：http://oj.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pd.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ub.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://dx.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://bl.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xq.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ej.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vu.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ro.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://fo.szxytkj.cn

Py:   json.loads(s)
来源：http://ns.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fo.lnxyls.cn

JS:   JSON.parse(s)
来源：http://kc.lnxyls.cn

TS:   JSON.parse(s)
来源：http://cj.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://by.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://cn.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://sp.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aw.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ks.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ek.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fv.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hd.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mj.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tg.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iy.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xm.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kx.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://tu.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xd.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nr.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zf.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wb.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://am.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pl.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ng.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kp.asd995.cn

[K05] 深拷贝对象
来源：http://kl.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://lf.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://um.gzmigu.cn

JS:   structuredClone(obj)
来源：http://wk.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://hm.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zl.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jz.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bk.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fy.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://xw.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wf.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ig.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qk.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lv.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uv.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ry.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bu.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://et.huanxung.cn

[K07] 进制转换
来源：http://jw.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://re.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fu.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sf.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://be.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uv.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qk.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dg.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ci.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://wl.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ti.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://go.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ci.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://oo.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ca.gzmigu.cn

Go:   encoding/gob
来源：http://mc.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://zj.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rl.jctech888.com.cn

================================================================================
来源：http://vh.lnxyls.cn

L. 网络请求
来源：http://cq.szxytkj.cn

================================================================================
来源：http://dv.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://sv.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ml.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ag.haigaiapp.cn

JS:   await fetch(url)
来源：http://sq.chemitech.net.cn

TS:   await fetch(url)
来源：http://ol.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ts.jctech888.com.cn


<!-- 参考信息 -->