代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://pl.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://aw.nicolike.cn

[H05] 捕获特定类型
来源：http://rd.haigaiapp.cn

Py:   except ValueError as e:
来源：http://qw.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pj.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://wk.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://tk.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://qg.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://az.521024.cn

Ruby: rescue ArgumentError => e
来源：http://kz.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vh.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://sw.newstarts.cn

Py:   value = d.get("k") or default
来源：http://mh.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mk.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ph.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pm.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bi.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nk.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://nd.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://jh.colortex.cn

[H07] 断言
来源：http://dt.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://gw.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://mj.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://aj.nszjky.cn

TS:   console.assert(x > 0);
来源：http://db.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://um.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yu.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://os.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://jl.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://kv.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://qy.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vx.shxzukj.cn

JS:   e.message;  e.stack
来源：http://vg.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qu.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dg.muxihuayi.cn

Go:   err.Error()
来源：http://zq.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://xp.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://nk.yuexingan06.cn

[H09] 带错误码的异常
来源：http://te.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ic.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tw.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ve.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qq.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yp.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xn.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bw.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iu.newstarts.cn

[H10] 资源自动释放
来源：http://ho.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ch.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qe.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pq.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hv.szsharing.cn

Go:   defer f.Close()
来源：http://ni.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ab.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://no.jctech888.com.cn

================================================================================
来源：http://qu.szsharing.cn

I. 正则表达式
来源：http://ig.bookmarksfly.cn

================================================================================
来源：http://fu.wgjwhj.cn

[I01] 判断是否匹配
来源：http://vh.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cn.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qv.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://fj.szsharing.cn

TS:   /\d+/.test(s)
来源：http://nq.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sp.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lz.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://xb.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lk.panjiajie.cn

[I02] 提取所有匹配
来源：http://fe.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://nm.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hg.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pj.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://mm.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jf.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mt.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://qz.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://db.szxytkj.cn

[I03] 提取捕获分组
来源：http://vm.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xv.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hf.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vg.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zl.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jp.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kt.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hq.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cv.muxihuayi.cn

[I04] 正则替换
来源：http://qw.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jx.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ky.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mp.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://us.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yy.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ga.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zx.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cs.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://qz.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wj.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zo.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://yp.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://ue.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://vw.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ak.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kh.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://om.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qm.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://br.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qn.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bb.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dq.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lv.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sr.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lp.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gb.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://xz.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gc.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fh.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://il.huixiangedu.cn

TS:   /error/gim
来源：http://mn.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jm.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vf.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://bt.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vh.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://zo.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ud.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gq.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ye.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ad.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cy.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ms.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ld.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fo.szsharing.cn

================================================================================
来源：http://yu.shtwfgs.cn

J. 日期与时间
来源：http://av.colortex.cn

================================================================================
来源：http://bo.shxzukj.cn

[J01] 获取当前时间
来源：http://lh.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uy.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zf.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://nn.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://ff.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vs.hnjuh.cn

Go:   time.Now()
来源：http://yz.jianghongdianzi.cn

Ruby: Time.now
来源：http://fr.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xn.muxihuayi.cn

[J02] 格式化输出
来源：http://yt.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ue.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iz.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jr.nszjky.cn

TS:   d.toISOString()
来源：http://ok.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ic.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mu.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vx.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jm.hnjuh.cn

[J03] 字符串解析为日期
来源：http://os.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dd.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://go.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://jj.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://ue.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://np.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://md.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://qo.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dm.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://vj.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nh.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gn.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gj.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jh.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hp.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ej.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pl.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ji.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://ke.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://eu.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lz.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://is.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://os.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://wy.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sm.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://bm.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nj.asd995.cn

[J06] 计算两时间之差
来源：http://oe.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://zv.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://lr.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cx.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ej.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gu.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://yp.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ed.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://dp.panjiajie.cn

[J07] 比较两个日期
来源：http://sd.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://gp.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ez.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ok.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ax.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jr.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pf.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lo.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://yj.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dw.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mk.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jk.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fc.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kn.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gz.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zi.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xs.bjjhwx.cn

[J09] 时区处理
来源：http://qu.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zk.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rt.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cb.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ni.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ci.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oc.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://po.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oj.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://be.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xk.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jx.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fe.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bo.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sh.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lu.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ua.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nj.yuexingan06.cn

================================================================================
来源：http://ip.nszjky.cn

K. JSON 与序列化
来源：http://cz.nszjky.cn

================================================================================
来源：http://fl.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://bz.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vq.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sv.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://xa.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://xu.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://do.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ts.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fv.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oq.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://df.huixiangedu.cn

Py:   json.loads(s)
来源：http://ke.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://iw.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://qc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sm.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://tg.nicolike.cn

Ruby: JSON.parse(s)
来源：http://cv.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zr.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://qk.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xr.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cy.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kb.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uv.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ih.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nq.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gk.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yn.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://el.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ov.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wn.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rg.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ok.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rs.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fg.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mb.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pq.haigaiapp.cn

[K05] 深拷贝对象
来源：http://fd.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://gw.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ro.szsharing.cn

JS:   structuredClone(obj)
来源：http://du.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ky.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nu.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oj.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fy.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nh.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://wy.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hm.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tj.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rr.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ey.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pz.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kk.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gr.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vp.521024.cn

[K07] 进制转换
来源：http://bk.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cv.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://po.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gj.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fb.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lv.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ri.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yb.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vv.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://oy.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://xp.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wn.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://xg.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://zq.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vq.gzmigu.cn

Go:   encoding/gob
来源：http://dm.521024.cn

Ruby: Marshal.dump(obj)
来源：http://xd.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ij.huanxung.cn

================================================================================
来源：http://th.jctech888.com.cn


<!-- 参考信息 -->