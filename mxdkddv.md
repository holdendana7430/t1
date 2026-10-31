代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://ex.newstarts.cn

C#:   class MyException : Exception {}
来源：http://gv.chemitech.net.cn

[H05] 捕获特定类型
来源：http://rf.wgjwhj.cn

Py:   except ValueError as e:
来源：http://da.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hw.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://aq.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://jx.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ks.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://lh.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mf.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://yk.asd995.cn

Py:   value = d.get("k") or default
来源：http://aw.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jf.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pn.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ss.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://je.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fz.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://xb.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://ky.muxihuayi.cn

[H07] 断言
来源：http://wa.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://fj.hnjuh.cn

PHP:  assert($x > 0);
来源：http://wu.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://ee.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://km.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://uq.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cw.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zv.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://oz.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://og.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://hs.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://me.nszjky.cn

JS:   e.message;  e.stack
来源：http://ld.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jy.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hs.shtwfgs.cn

Go:   err.Error()
来源：http://aj.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://fn.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://nd.colortex.cn

[H09] 带错误码的异常
来源：http://yd.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pz.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uc.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xw.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ys.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://au.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gl.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ej.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gi.panjiajie.cn

[H10] 资源自动释放
来源：http://vu.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://um.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ef.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cw.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jx.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nn.nicolike.cn

Go:   defer f.Close()
来源：http://nk.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ii.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wt.huixinmuqiang.cn

================================================================================
来源：http://zl.szxytkj.cn

I. 正则表达式
来源：http://nf.szsharing.cn

================================================================================
来源：http://nh.shxzskj.cn

[I01] 判断是否匹配
来源：http://tz.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ua.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hk.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://ic.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://ka.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ny.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ke.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ej.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rk.huanxung.cn

[I02] 提取所有匹配
来源：http://ub.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://qb.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kv.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ru.asd995.cn

TS:   s.match(/\d+/g)
来源：http://af.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ud.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jp.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://yz.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jd.gzmigu.cn

[I03] 提取捕获分组
来源：http://pf.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eg.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ji.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rf.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lw.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fh.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ux.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dw.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kt.newstarts.cn

[I04] 正则替换
来源：http://ox.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://br.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rz.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yc.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://as.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nj.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fh.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://am.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ca.hahajie.cn

[I05] 按正则拆分
来源：http://bm.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rt.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mv.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ht.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://lx.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://au.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tl.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nv.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jp.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ak.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cm.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ii.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sb.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hd.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kf.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://af.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zw.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cw.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://ss.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ei.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://op.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qm.shxzskj.cn

TS:   /error/gim
来源：http://bf.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nh.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bu.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://pg.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://te.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://kx.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vb.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ud.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qf.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cq.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cg.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nm.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bq.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ca.gzmigu.cn

================================================================================
来源：http://lg.shxzskj.cn

J. 日期与时间
来源：http://hc.szsharing.cn

================================================================================
来源：http://ct.jctech888.com.cn

[J01] 获取当前时间
来源：http://xo.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hj.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ey.nicolike.cn

JS:   new Date();  Date.now()
来源：http://ae.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://fg.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://si.hnjuh.cn

Go:   time.Now()
来源：http://oc.newstarts.cn

Ruby: Time.now
来源：http://tf.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fe.shxzskj.cn

[J02] 格式化输出
来源：http://qw.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://os.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xk.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xx.szxytkj.cn

TS:   d.toISOString()
来源：http://gq.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kt.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://he.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ym.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://li.szsharing.cn

[J03] 字符串解析为日期
来源：http://up.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nm.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kn.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://zt.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://sx.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xy.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://og.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://mh.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hn.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://bj.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gq.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ft.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ed.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://se.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qa.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xr.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dd.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://pa.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://cp.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rd.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yk.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rc.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://li.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wj.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://nl.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ll.bjjhwx.cn

[J06] 计算两时间之差
来源：http://xm.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://qk.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://oy.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ve.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zb.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fn.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://li.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://wa.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://kn.chemitech.net.cn

[J07] 比较两个日期
来源：http://nb.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://zu.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jg.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nn.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ab.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zw.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nb.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lm.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://we.hahajie.cn

[J08] 提取年月日与星期
来源：http://fk.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uh.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://br.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://my.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cq.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uo.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hl.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qv.chemitech.net.cn

[J09] 时区处理
来源：http://ss.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xi.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://af.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zx.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rl.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mk.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wh.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://le.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vx.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://ne.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pl.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jx.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fo.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mc.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xr.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rh.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://so.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gw.lnxyls.cn

================================================================================
来源：http://fh.asd995.cn

K. JSON 与序列化
来源：http://xg.huixinmuqiang.cn

================================================================================
来源：http://wg.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://zk.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://il.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nn.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://wj.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://tq.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aj.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://ox.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fq.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aq.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ey.shxzskj.cn

Py:   json.loads(s)
来源：http://xm.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zk.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://sv.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://mq.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qo.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://wg.colortex.cn

Ruby: JSON.parse(s)
来源：http://zn.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fh.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xk.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cw.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gj.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xa.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tk.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://an.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uz.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tc.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hl.521024.cn

[K04] 读取 JSON 文件
来源：http://bd.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qw.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yb.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pb.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eu.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nn.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://no.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pg.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hf.hahajie.cn

[K05] 深拷贝对象
来源：http://fi.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://dc.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://dz.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://vw.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://wt.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fq.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://go.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://va.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fj.szsharing.cn

[K06] 解析 URL 查询串
来源：http://gs.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ys.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jl.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pm.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wm.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sz.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fq.hahajie.cn

[K07] 进制转换
来源：http://me.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yo.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qh.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zr.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lz.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ex.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jf.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ye.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://fn.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://ee.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lo.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://jy.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://yg.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oq.hnjuh.cn

Go:   encoding/gob
来源：http://aw.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://bi.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gl.jianghongdianzi.cn

================================================================================
来源：http://zq.521024.cn


<!-- 参考信息 -->