代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://pt.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://jn.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://pp.shxzskj.cn

Py:   except ValueError as e:
来源：http://yo.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gy.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ne.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://px.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://wm.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nk.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://dv.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ho.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://jg.huanxung.cn

Py:   value = d.get("k") or default
来源：http://fq.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qn.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mq.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tz.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dq.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rv.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://di.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://xb.hnjuh.cn

[H07] 断言
来源：http://op.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://sy.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://be.huanxung.cn

JS:   console.assert(x > 0);
来源：http://sw.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://wy.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://yz.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qk.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ct.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://rh.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://dd.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://cm.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tz.panjiajie.cn

JS:   e.message;  e.stack
来源：http://kk.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fm.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ov.nszjky.cn

Go:   err.Error()
来源：http://qx.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://yr.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ar.colortex.cn

[H09] 带错误码的异常
来源：http://yt.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://by.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mu.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rf.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zq.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uy.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kd.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tg.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yw.yuexingan06.cn

[H10] 资源自动释放
来源：http://oh.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ql.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ps.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://el.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dn.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zo.shxzskj.cn

Go:   defer f.Close()
来源：http://cu.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jp.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uh.chemitech.net.cn

================================================================================
来源：http://td.jianghongdianzi.cn

I. 正则表达式
来源：http://ql.muxihuayi.cn

================================================================================
来源：http://hn.521024.cn

[I01] 判断是否匹配
来源：http://it.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vw.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sx.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://tx.szsharing.cn

TS:   /\d+/.test(s)
来源：http://vz.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kv.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://og.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://cl.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fg.lnxyls.cn

[I02] 提取所有匹配
来源：http://pt.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://he.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jb.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bx.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://sa.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ns.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ab.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://sy.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://es.yuexingan06.cn

[I03] 提取捕获分组
来源：http://ap.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mf.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ft.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cs.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kf.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oq.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wp.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jr.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nc.shxzskj.cn

[I04] 正则替换
来源：http://if.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ly.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://at.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wg.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rb.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cp.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ex.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ge.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vt.wgjwhj.cn

[I05] 按正则拆分
来源：http://xy.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lv.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cj.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://sp.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://vt.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://bg.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zg.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jl.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uj.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ys.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yc.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sz.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gd.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zx.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rm.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qs.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mv.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cc.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://yz.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ht.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zf.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mr.9csxet.cn

TS:   /error/gim
来源：http://ks.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ew.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zv.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://um.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eo.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://io.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gd.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qi.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mr.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ma.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ku.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://he.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pd.jianghongdianzi.cn

================================================================================
来源：http://tc.9csxet.cn

J. 日期与时间
来源：http://jz.yuexingan06.cn

================================================================================
来源：http://nl.bjjhwx.cn

[J01] 获取当前时间
来源：http://ep.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vk.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://km.9csxet.cn

JS:   new Date();  Date.now()
来源：http://vj.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://hg.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wr.lnxyls.cn

Go:   time.Now()
来源：http://ho.bjjhwx.cn

Ruby: Time.now
来源：http://xg.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vw.panjiajie.cn

[J02] 格式化输出
来源：http://cj.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zl.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ey.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ep.hahajie.cn

TS:   d.toISOString()
来源：http://sz.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ix.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ss.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ca.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lt.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://mv.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pc.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://or.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://wq.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://pv.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rg.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sa.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://kk.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ov.521024.cn

[J04] 时间戳与日期互转
来源：http://ai.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kr.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xw.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://co.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gp.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kw.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ef.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ck.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://at.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://iu.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://ki.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uh.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fw.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://mo.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fm.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ni.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tm.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://uv.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://wc.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://ed.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pc.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dr.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ql.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://qn.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vb.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://xq.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://dt.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gf.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sc.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hd.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rv.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ap.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kh.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://oj.hahajie.cn

[J08] 提取年月日与星期
来源：http://pk.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ea.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://os.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ny.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vt.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hy.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xo.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vj.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hq.chemitech.net.cn

[J09] 时区处理
来源：http://vt.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ym.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lq.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ij.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jn.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dd.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eo.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uv.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lo.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://af.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cp.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sz.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ai.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://em.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rd.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ja.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://to.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iq.bookmarksfly.cn

================================================================================
来源：http://sg.yuexingan06.cn

K. JSON 与序列化
来源：http://rn.gzmigu.cn

================================================================================
来源：http://ee.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://eq.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bm.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wu.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://gb.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://vl.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yt.szsharing.cn

Go:   json.Marshal(obj)
来源：http://vj.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eh.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qn.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://fg.nicolike.cn

Py:   json.loads(s)
来源：http://sk.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bz.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://lr.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://ln.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xg.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://oa.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://tl.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vo.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ds.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lo.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qb.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://op.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://id.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qe.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ue.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xt.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sy.colortex.cn

[K04] 读取 JSON 文件
来源：http://pc.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sg.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ji.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rp.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xw.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fi.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kf.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uq.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sm.9csxet.cn

[K05] 深拷贝对象
来源：http://ow.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://bv.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://wf.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ol.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://dm.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kj.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fp.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bi.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gt.nicolike.cn

[K06] 解析 URL 查询串
来源：http://cq.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kf.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://en.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://of.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tp.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nc.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ts.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ae.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zx.gzmigu.cn

[K07] 进制转换
来源：http://on.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vq.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ad.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jb.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ft.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ll.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://he.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hy.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yr.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sd.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://dw.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fm.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://fs.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://vb.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jz.hnjuh.cn

Go:   encoding/gob
来源：http://il.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://jh.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rg.bookmarksfly.cn

================================================================================
来源：http://gl.szxytkj.cn


<!-- 参考信息 -->