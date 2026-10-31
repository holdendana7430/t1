代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://zb.nicolike.cn

C#:   class MyException : Exception {}
来源：http://bo.newstarts.cn

[H05] 捕获特定类型
来源：http://oa.bjjhwx.cn

Py:   except ValueError as e:
来源：http://at.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gg.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://fx.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://su.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://bj.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kj.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://fs.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uy.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://dz.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://ym.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vj.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mm.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sy.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ut.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ct.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://gz.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://dm.shtwfgs.cn

[H07] 断言
来源：http://yn.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://qf.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://dx.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://mk.9csxet.cn

TS:   console.assert(x > 0);
来源：http://dt.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://hk.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wn.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ua.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://gl.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://hb.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://mb.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sq.newstarts.cn

JS:   e.message;  e.stack
来源：http://xu.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nh.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mi.lnxyls.cn

Go:   err.Error()
来源：http://vp.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://kz.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://xd.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://hq.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nn.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jk.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ai.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pk.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vo.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fw.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tu.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ch.bookmarksfly.cn

[H10] 资源自动释放
来源：http://gs.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tr.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://js.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lm.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://we.panjiajie.cn

Go:   defer f.Close()
来源：http://yy.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qx.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wr.wgjwhj.cn

================================================================================
来源：http://zl.jctech888.com.cn

I. 正则表达式
来源：http://jz.yuexingan06.cn

================================================================================
来源：http://jw.hnjuh.cn

[I01] 判断是否匹配
来源：http://yc.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ez.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cv.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://pr.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://oz.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ku.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://if.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://ei.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rq.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://yx.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://ij.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://og.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oz.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://lu.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gp.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gw.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://ni.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://da.jctech888.com.cn

[I03] 提取捕获分组
来源：http://ve.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://at.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kf.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kz.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ul.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pb.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vl.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://km.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kx.521024.cn

[I04] 正则替换
来源：http://xc.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xo.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ct.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://za.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cg.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vm.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vv.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cf.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://az.nicolike.cn

[I05] 按正则拆分
来源：http://mb.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gu.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wx.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://si.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://bs.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://gv.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ds.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qd.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xz.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oa.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mx.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ec.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pb.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hx.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cn.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ls.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gg.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://oi.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cu.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vl.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ry.jianghongdianzi.cn

TS:   /error/gim
来源：http://dz.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nb.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lh.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://iy.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xb.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yc.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ez.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xi.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gk.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xx.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kl.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uu.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cb.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xi.wgjwhj.cn

================================================================================
来源：http://vy.521024.cn

J. 日期与时间
来源：http://zp.asd995.cn

================================================================================
来源：http://du.szsharing.cn

[J01] 获取当前时间
来源：http://gr.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jy.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jv.hahajie.cn

JS:   new Date();  Date.now()
来源：http://ne.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://kj.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uc.521024.cn

Go:   time.Now()
来源：http://hz.lnxyls.cn

Ruby: Time.now
来源：http://nc.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zq.nszjky.cn

[J02] 格式化输出
来源：http://os.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wc.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xt.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nl.asd995.cn

TS:   d.toISOString()
来源：http://vh.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://po.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lr.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uk.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ct.hnjuh.cn

[J03] 字符串解析为日期
来源：http://ib.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zb.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rn.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://of.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://yg.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qs.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wc.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ii.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cl.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://zm.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vg.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zd.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zh.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pi.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ya.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jd.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rh.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zb.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://cl.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://fn.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ew.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xz.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://er.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ih.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wl.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ct.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ra.colortex.cn

[J06] 计算两时间之差
来源：http://ne.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://tz.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://aq.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nm.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nz.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sl.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://sm.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://vv.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://qf.yuexingan06.cn

[J07] 比较两个日期
来源：http://iv.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://my.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zx.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fg.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cw.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pp.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wb.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yf.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://gg.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://hd.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fq.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sz.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pb.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xp.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vk.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nl.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zy.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lm.haigaiapp.cn

[J09] 时区处理
来源：http://ye.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ah.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uz.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fc.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://id.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ua.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vk.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://it.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://rz.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://is.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wx.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fw.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ok.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pr.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cf.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ki.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://og.huixinmuqiang.cn

================================================================================
来源：http://ea.shxzskj.cn

K. JSON 与序列化
来源：http://ib.yuntaijiaju.cn

================================================================================
来源：http://za.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://dq.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eu.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ys.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ue.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://rc.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mo.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://xp.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pf.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ju.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://qv.panjiajie.cn

Py:   json.loads(s)
来源：http://xf.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qh.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://qo.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://gs.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ac.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://oe.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://tx.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nk.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://ig.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oo.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bv.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vn.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wa.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qp.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://df.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hm.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://al.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ra.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zc.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vb.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wh.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://si.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eh.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://es.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gy.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qe.yuexingan06.cn

[K05] 深拷贝对象
来源：http://bs.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://ar.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://fj.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://tu.colortex.cn

TS:   structuredClone(obj)
来源：http://lw.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kk.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ar.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uo.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oz.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://vm.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lr.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ul.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jc.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iu.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://et.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jt.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://um.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://or.yuntaijiaju.cn

[K07] 进制转换
来源：http://dj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xz.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://an.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ob.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ux.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mb.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cr.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eu.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zo.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ic.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://qn.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aq.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://aq.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://bw.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ka.yuntaijiaju.cn

Go:   encoding/gob
来源：http://ev.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ed.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hd.muxihuayi.cn

================================================================================
来源：http://bm.9csxet.cn


<!-- 参考信息 -->