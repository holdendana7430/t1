代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://fu.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://yr.yuexingan06.cn

[H05] 捕获特定类型
来源：http://ot.9csxet.cn

Py:   except ValueError as e:
来源：http://cw.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dt.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://yn.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://uh.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://px.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://je.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://uo.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xz.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://uo.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://tz.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ia.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vz.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://is.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kf.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pb.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://ex.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ig.wgjwhj.cn

[H07] 断言
来源：http://ox.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://sx.shxzskj.cn

PHP:  assert($x > 0);
来源：http://mf.colortex.cn

JS:   console.assert(x > 0);
来源：http://wt.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://wh.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://xt.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kn.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wv.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://la.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://od.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://tk.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bu.9csxet.cn

JS:   e.message;  e.stack
来源：http://wf.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uy.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ae.huixiangedu.cn

Go:   err.Error()
来源：http://dr.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://qw.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://ie.lnxyls.cn

[H09] 带错误码的异常
来源：http://bv.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rg.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pa.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bn.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uf.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ra.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kw.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uc.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pd.bjjhwx.cn

[H10] 资源自动释放
来源：http://dw.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bh.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bs.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yo.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pq.asd995.cn

Go:   defer f.Close()
来源：http://mz.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xy.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fh.lnxyls.cn

================================================================================
来源：http://ma.bjjhwx.cn

I. 正则表达式
来源：http://wk.shxzskj.cn

================================================================================
来源：http://mk.bjjhwx.cn

[I01] 判断是否匹配
来源：http://co.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sm.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pr.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://de.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://mb.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ex.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vz.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://jr.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ki.bjjhwx.cn

[I02] 提取所有匹配
来源：http://bg.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://jg.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nw.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uo.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://jp.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xr.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mm.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ko.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cl.shtwfgs.cn

[I03] 提取捕获分组
来源：http://kr.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lk.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cj.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tx.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ha.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://od.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cn.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rh.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ki.yuexingan06.cn

[I04] 正则替换
来源：http://rj.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tf.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ay.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nq.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jn.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hy.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rj.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qe.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wc.lnxyls.cn

[I05] 按正则拆分
来源：http://nr.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ss.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pn.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://fa.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://sg.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://zc.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rp.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pm.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ce.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vo.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ah.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cz.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cm.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lj.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ig.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fm.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hn.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://id.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://pc.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vs.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gd.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aq.521024.cn

TS:   /error/gim
来源：http://uk.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zf.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yz.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://xu.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rp.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://sx.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://to.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zc.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hp.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://km.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bt.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jg.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xq.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yg.huixiangedu.cn

================================================================================
来源：http://ih.shxzskj.cn

J. 日期与时间
来源：http://qz.bjjhwx.cn

================================================================================
来源：http://em.nszjky.cn

[J01] 获取当前时间
来源：http://zr.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://he.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ks.hahajie.cn

JS:   new Date();  Date.now()
来源：http://sc.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://gw.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ap.shxzukj.cn

Go:   time.Now()
来源：http://ty.hnjuh.cn

Ruby: Time.now
来源：http://af.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lf.asd995.cn

[J02] 格式化输出
来源：http://gy.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jl.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kw.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fg.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://ch.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kb.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://il.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dg.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oe.hnjuh.cn

[J03] 字符串解析为日期
来源：http://vu.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ik.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://il.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://bn.colortex.cn

TS:   new Date("2024-01-02")
来源：http://zh.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wk.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ww.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://dt.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jh.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://sj.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ky.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gk.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://is.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://st.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qv.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mf.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yk.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://up.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://lk.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://dp.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bn.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yd.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://hm.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bu.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://nl.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lg.szxytkj.cn

[J06] 计算两时间之差
来源：http://lx.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://zw.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://xw.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fb.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pi.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mj.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ck.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://hm.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://zy.asd995.cn

[J07] 比较两个日期
来源：http://xa.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://sf.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yg.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ze.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bh.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mm.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ht.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dh.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://uc.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://zf.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nd.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://if.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ge.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bh.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qr.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yo.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://de.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sy.nszjky.cn

[J09] 时区处理
来源：http://eg.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lm.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://re.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vx.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ao.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kp.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kz.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://we.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nu.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://hk.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://in.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://si.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vo.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ge.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lx.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://au.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://th.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ni.shtwfgs.cn

================================================================================
来源：http://jg.newstarts.cn

K. JSON 与序列化
来源：http://pi.colortex.cn

================================================================================
来源：http://uw.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://vo.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lv.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ln.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://vf.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://xz.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lz.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://wv.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wt.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jp.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://cu.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://fv.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hj.nszjky.cn

JS:   JSON.parse(s)
来源：http://mm.shxzskj.cn

TS:   JSON.parse(s)
来源：http://ar.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dl.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://pv.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://nh.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dh.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://hu.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wh.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lx.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nx.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pw.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kf.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wt.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wp.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nf.521024.cn

[K04] 读取 JSON 文件
来源：http://xm.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pf.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ip.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vd.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://do.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jt.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rd.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vk.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ow.shtwfgs.cn

[K05] 深拷贝对象
来源：http://iu.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://hl.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://xf.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://wk.shxzukj.cn

TS:   structuredClone(obj)
来源：http://tb.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zo.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xr.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ur.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hs.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://gc.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zi.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lp.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gl.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kp.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ft.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://no.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mw.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bm.huixiangedu.cn

[K07] 进制转换
来源：http://si.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jv.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ln.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mw.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wv.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xm.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jn.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ul.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jq.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://zu.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://ch.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hw.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zg.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://bj.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://et.bjjhwx.cn

Go:   encoding/gob
来源：http://wp.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://dq.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nc.wgjwhj.cn

================================================================================
来源：http://ny.bjjhwx.cn


<!-- 参考信息 -->