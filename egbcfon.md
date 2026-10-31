代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://la.colortex.cn

C#:   class MyException : Exception {}
来源：http://zp.lnxyls.cn

[H05] 捕获特定类型
来源：http://my.9csxet.cn

Py:   except ValueError as e:
来源：http://fe.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://al.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://jc.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://xn.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://pl.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://he.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://pn.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pg.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://mv.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://yj.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ft.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zk.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://il.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wd.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oj.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://an.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://yw.huixiangedu.cn

[H07] 断言
来源：http://uz.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://ux.szxytkj.cn

PHP:  assert($x > 0);
来源：http://lb.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://gb.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://lh.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ob.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uq.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yp.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://go.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://wx.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://yu.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sb.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://vb.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eu.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cn.shxzskj.cn

Go:   err.Error()
来源：http://rh.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ba.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://ln.lnxyls.cn

[H09] 带错误码的异常
来源：http://ub.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wk.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rn.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oy.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ht.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://su.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fa.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kq.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jp.shxzukj.cn

[H10] 资源自动释放
来源：http://mg.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sc.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oi.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lo.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://og.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aj.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://kz.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fv.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lq.hnjuh.cn

================================================================================
来源：http://aw.huixiangedu.cn

I. 正则表达式
来源：http://sz.nszjky.cn

================================================================================
来源：http://ep.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://wj.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qb.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ct.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://sc.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://wb.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pw.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lo.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://sf.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qe.nicolike.cn

[I02] 提取所有匹配
来源：http://cg.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://pd.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zh.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tq.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://ku.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lg.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gm.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://zg.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bq.asd995.cn

[I03] 提取捕获分组
来源：http://fx.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ml.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uq.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xb.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uu.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://av.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gx.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gz.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tx.muxihuayi.cn

[I04] 正则替换
来源：http://tw.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pd.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mq.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hg.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://az.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sy.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cv.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yo.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ni.hnjuh.cn

[I05] 按正则拆分
来源：http://im.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://re.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ts.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://ps.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ml.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://cf.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qo.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://po.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mz.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fz.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nn.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vn.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://th.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cu.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xu.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sr.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tm.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ci.521024.cn

[I07] 忽略大小写与多行模式
来源：http://dk.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wv.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ew.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qp.wgjwhj.cn

TS:   /error/gim
来源：http://pz.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wt.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://be.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://wc.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jj.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://zo.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wo.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gq.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vq.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://my.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jh.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://du.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tt.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dr.yuexingan06.cn

================================================================================
来源：http://lr.shxzukj.cn

J. 日期与时间
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://sf.shtwfgs.cn

[J01] 获取当前时间
来源：http://ux.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ek.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ry.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://hk.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://oj.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cs.panjiajie.cn

Go:   time.Now()
来源：http://fa.szsharing.cn

Ruby: Time.now
来源：http://zh.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jp.huanxung.cn

[J02] 格式化输出
来源：http://rr.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ck.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ha.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pb.wgjwhj.cn

TS:   d.toISOString()
来源：http://qi.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gh.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://px.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qm.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sn.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://ha.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ov.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cp.521024.cn

JS:   new Date("2024-01-02")
来源：http://lx.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://hg.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mr.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hc.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://sx.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dj.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://lm.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://su.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tu.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kq.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xt.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oa.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xn.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wm.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nu.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://jt.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://qq.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://us.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rj.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dt.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://yr.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://du.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://yu.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jy.huixiangedu.cn

[J06] 计算两时间之差
来源：http://zi.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://de.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ws.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ns.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xa.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hd.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://vv.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://nr.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://cz.asd995.cn

[J07] 比较两个日期
来源：http://ux.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://rn.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ml.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ew.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pb.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zf.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qn.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qc.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://bs.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ta.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zi.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fa.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ek.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xy.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ly.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ji.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bi.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rq.yuntaijiaju.cn

[J09] 时区处理
来源：http://np.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ls.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iy.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ez.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kj.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ro.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fr.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zl.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://nc.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zs.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ge.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ys.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pw.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lz.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jw.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vb.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yo.521024.cn

================================================================================
来源：http://zw.gzmigu.cn

K. JSON 与序列化
来源：http://lr.gzmigu.cn

================================================================================
来源：http://kz.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://yk.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dt.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://by.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://xw.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://oc.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qm.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://uh.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yj.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mp.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://qx.shtwfgs.cn

Py:   json.loads(s)
来源：http://vi.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gx.panjiajie.cn

JS:   JSON.parse(s)
来源：http://iu.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://hb.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cx.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://dd.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://im.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bk.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://wz.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jn.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wl.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://te.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wq.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hd.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zs.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pd.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kc.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://fd.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ts.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hv.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lw.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dw.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hv.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kg.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eo.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nm.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://bh.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://xw.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ac.521024.cn

JS:   structuredClone(obj)
来源：http://ze.521024.cn

TS:   structuredClone(obj)
来源：http://do.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://au.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ic.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pi.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qj.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://tu.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jx.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bv.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sy.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://md.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kh.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qg.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bp.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wj.shxzskj.cn

[K07] 进制转换
来源：http://xj.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vl.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fn.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mf.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pc.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ke.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zc.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kz.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://oh.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://be.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ly.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://xs.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://cp.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vy.bookmarksfly.cn

Go:   encoding/gob
来源：http://bq.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://tk.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sl.shxzukj.cn

================================================================================
来源：http://ud.bjjhwx.cn


<!-- 参考信息 -->