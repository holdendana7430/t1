代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://vn.newstarts.cn

C#:   class MyException : Exception {}
来源：http://ae.lnxyls.cn

[H05] 捕获特定类型
来源：http://es.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://gz.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ns.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://as.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pz.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://xf.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ea.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://zc.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vx.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ew.nszjky.cn

Py:   value = d.get("k") or default
来源：http://cu.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dq.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://om.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ch.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wk.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vh.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://tc.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://ks.huixinmuqiang.cn

[H07] 断言
来源：http://vt.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://vm.521024.cn

PHP:  assert($x > 0);
来源：http://bs.nicolike.cn

JS:   console.assert(x > 0);
来源：http://nx.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://to.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://hx.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://th.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dx.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://vl.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://zx.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://la.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qh.panjiajie.cn

JS:   e.message;  e.stack
来源：http://id.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uu.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jc.nicolike.cn

Go:   err.Error()
来源：http://xm.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://jh.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://tw.haigaiapp.cn

[H09] 带错误码的异常
来源：http://ep.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eq.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kf.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hn.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kx.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://td.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ix.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://et.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mt.lnxyls.cn

[H10] 资源自动释放
来源：http://cd.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cy.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cj.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nc.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wt.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ge.shxzukj.cn

Go:   defer f.Close()
来源：http://kn.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vk.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xg.hnjuh.cn

================================================================================
来源：http://lb.shxzukj.cn

I. 正则表达式
来源：http://ty.huanxung.cn

================================================================================
来源：http://ag.shxzskj.cn

[I01] 判断是否匹配
来源：http://lo.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gj.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ic.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://pk.szsharing.cn

TS:   /\d+/.test(s)
来源：http://sw.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sb.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eu.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://dk.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mn.9csxet.cn

[I02] 提取所有匹配
来源：http://qu.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://ms.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vn.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ay.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://ip.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hd.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ur.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://am.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ib.hahajie.cn

[I03] 提取捕获分组
来源：http://se.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://va.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://of.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://po.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ay.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kg.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zf.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lu.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sh.bookmarksfly.cn

[I04] 正则替换
来源：http://xr.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gg.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fd.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pc.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bs.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dp.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qo.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mn.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xg.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://ok.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dm.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sc.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://xh.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://tg.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://fv.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ku.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iw.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vq.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tr.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fv.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ji.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zk.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ze.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ty.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://et.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rq.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://bz.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ma.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kp.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ab.huixinmuqiang.cn

TS:   /error/gim
来源：http://xi.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qh.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lw.colortex.cn

Ruby: s.scan(/error/i)
来源：http://gk.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bi.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://xs.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://az.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://es.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yy.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ct.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vu.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zm.hnjuh.cn

================================================================================
来源：http://hc.nszjky.cn

J. 日期与时间
来源：http://gu.chemitech.net.cn

================================================================================
来源：http://nt.szsharing.cn

[J01] 获取当前时间
来源：http://rm.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wt.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lp.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://as.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://mn.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://le.panjiajie.cn

Go:   time.Now()
来源：http://cv.huixiangedu.cn

Ruby: Time.now
来源：http://bb.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mn.colortex.cn

[J02] 格式化输出
来源：http://le.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://av.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gu.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.szsharing.cn

TS:   d.toISOString()
来源：http://ng.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hg.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nx.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mw.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zf.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ny.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bp.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jr.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://hw.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://za.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ad.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xt.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://ib.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wh.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://rm.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yj.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gu.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ne.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://le.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nv.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ur.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://id.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bt.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://vu.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://cp.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xw.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://en.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dm.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://is.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tz.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://va.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fy.jctech888.com.cn

[J06] 计算两时间之差
来源：http://qw.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://pe.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://cv.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://if.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bo.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ga.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://is.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://lh.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://hq.nszjky.cn

[J07] 比较两个日期
来源：http://ys.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://uu.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mv.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jo.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xw.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mc.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qk.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://hy.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://fn.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nv.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ua.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://be.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cv.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cn.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ao.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oj.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xr.shxzukj.cn

[J09] 时区处理
来源：http://bd.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sj.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://af.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sl.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://om.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://os.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mg.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jl.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kz.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://tx.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qy.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fc.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://po.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ht.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bi.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gw.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ta.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dn.huixiangedu.cn

================================================================================
来源：http://wa.521024.cn

K. JSON 与序列化
来源：http://eh.chemitech.net.cn

================================================================================
来源：http://az.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://fo.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gx.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vu.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://qg.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://st.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mw.521024.cn

Go:   json.Marshal(obj)
来源：http://ex.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ti.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ye.nszjky.cn

[K02] JSON 字符串转对象
来源：http://rp.panjiajie.cn

Py:   json.loads(s)
来源：http://ng.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iu.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://kw.panjiajie.cn

TS:   JSON.parse(s)
来源：http://bo.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qw.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://in.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://mk.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yu.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wx.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rs.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://io.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wf.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dt.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pg.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kz.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fg.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://dq.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zl.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://br.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://do.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://by.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://on.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dp.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yw.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nm.hahajie.cn

[K05] 深拷贝对象
来源：http://wm.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://ad.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://hq.huanxung.cn

JS:   structuredClone(obj)
来源：http://ef.nszjky.cn

TS:   structuredClone(obj)
来源：http://id.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ht.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ea.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eg.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fo.szsharing.cn

[K06] 解析 URL 查询串
来源：http://rr.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://am.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://of.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://us.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mn.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oj.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ko.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bg.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hc.bjjhwx.cn

[K07] 进制转换
来源：http://zc.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tw.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ly.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aq.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vw.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gk.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kk.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vp.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://am.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://aq.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://sa.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yd.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mz.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://sn.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rs.jianghongdianzi.cn

Go:   encoding/gob
来源：http://gm.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://mq.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://st.muxihuayi.cn

================================================================================
来源：http://ek.lnxyls.cn


<!-- 参考信息 -->