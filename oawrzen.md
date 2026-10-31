代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ab.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://cs.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://gi.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://ii.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hj.521024.cn

Ruby: rescue ArgumentError => e
来源：http://pw.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cn.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://mo.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ur.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ds.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bs.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jl.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gp.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hv.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://yo.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://pf.chemitech.net.cn

[H07] 断言
来源：http://dj.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://gi.asd995.cn

PHP:  assert($x > 0);
来源：http://wh.newstarts.cn

JS:   console.assert(x > 0);
来源：http://tp.szsharing.cn

TS:   console.assert(x > 0);
来源：http://yz.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://mi.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pk.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ra.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://xt.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://cm.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://cs.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rf.szxytkj.cn

JS:   e.message;  e.stack
来源：http://wq.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://va.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kw.shtwfgs.cn

Go:   err.Error()
来源：http://am.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://ph.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://tg.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://fq.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uo.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://le.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rj.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kk.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qe.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hr.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ri.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dl.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://nj.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://be.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://es.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lr.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jf.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ut.bookmarksfly.cn

Go:   defer f.Close()
来源：http://jv.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mr.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ev.shxzskj.cn

================================================================================
来源：http://up.huanxung.cn

I. 正则表达式
来源：http://xi.hahajie.cn

================================================================================
来源：http://rj.colortex.cn

[I01] 判断是否匹配
来源：http://od.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lf.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qq.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://vq.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://kc.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rc.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fw.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://yp.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dz.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://wj.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://cd.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ay.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://je.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://dp.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://km.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ji.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://gb.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yp.muxihuayi.cn

[I03] 提取捕获分组
来源：http://qv.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://be.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fj.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ag.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ds.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sv.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hk.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ou.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ub.nszjky.cn

[I04] 正则替换
来源：http://no.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iu.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://en.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tq.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sa.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ih.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oz.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tf.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dw.lnxyls.cn

[I05] 按正则拆分
来源：http://ok.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://er.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ho.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://gy.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://xw.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://jv.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ez.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dp.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ml.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yu.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kz.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xx.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://id.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wk.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vn.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yy.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jw.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uu.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://py.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mq.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kl.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yo.gzmigu.cn

TS:   /error/gim
来源：http://xg.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ki.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://la.asd995.cn

Ruby: s.scan(/error/i)
来源：http://oi.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oi.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://wf.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kj.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qu.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ps.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gf.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yu.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qf.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uu.yuexingan06.cn

================================================================================
来源：http://hn.nicolike.cn

J. 日期与时间
来源：http://as.9csxet.cn

================================================================================
来源：http://hq.panjiajie.cn

[J01] 获取当前时间
来源：http://fn.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tj.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qc.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://if.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://ad.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zn.bookmarksfly.cn

Go:   time.Now()
来源：http://dt.shxzskj.cn

Ruby: Time.now
来源：http://zy.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ya.wgjwhj.cn

[J02] 格式化输出
来源：http://qn.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ef.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ig.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jv.wgjwhj.cn

TS:   d.toISOString()
来源：http://it.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vy.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qm.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ov.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gn.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://le.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ru.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zg.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://yg.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://he.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sr.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://et.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://si.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rf.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://gp.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nh.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bc.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cz.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xe.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lx.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://my.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fg.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ib.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://oz.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://gs.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dc.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ca.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nv.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ys.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cc.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://tw.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hu.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://fa.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ge.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://gi.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cn.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ud.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ki.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ov.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://eg.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://rx.newstarts.cn

[J07] 比较两个日期
来源：http://lo.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ie.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rx.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xt.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yk.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dc.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ko.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wz.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://yd.nszjky.cn

[J08] 提取年月日与星期
来源：http://sp.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cc.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ut.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kx.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fu.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mw.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dy.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wu.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vd.szxytkj.cn

[J09] 时区处理
来源：http://rf.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yb.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ks.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qv.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bw.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sb.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ex.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://df.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://yc.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uf.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qz.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rq.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iv.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dy.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tx.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bb.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kg.9csxet.cn

================================================================================
来源：http://ti.9csxet.cn

K. JSON 与序列化
来源：http://me.shtwfgs.cn

================================================================================
来源：http://xb.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://go.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ms.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bc.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://mp.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://vp.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gg.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://xk.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pr.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mq.newstarts.cn

[K02] JSON 字符串转对象
来源：http://kh.colortex.cn

Py:   json.loads(s)
来源：http://bn.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qs.lnxyls.cn

JS:   JSON.parse(s)
来源：http://xn.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://bj.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vb.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://yq.szsharing.cn

Ruby: JSON.parse(s)
来源：http://se.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://af.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://pu.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zd.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ka.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tz.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ps.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vb.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://in.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gm.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://is.asd995.cn

[K04] 读取 JSON 文件
来源：http://zl.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zw.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://km.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tm.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pf.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jq.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bx.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vn.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qv.bjjhwx.cn

[K05] 深拷贝对象
来源：http://fz.521024.cn

Py:   copy.deepcopy(obj)
来源：http://kt.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://lf.gzmigu.cn

JS:   structuredClone(obj)
来源：http://pa.shxzukj.cn

TS:   structuredClone(obj)
来源：http://si.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cf.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ox.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zy.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nk.9csxet.cn

[K06] 解析 URL 查询串
来源：http://tw.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://me.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://og.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ax.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tz.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rj.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pp.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pu.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wf.bookmarksfly.cn

[K07] 进制转换
来源：http://xw.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kn.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pn.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gi.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pv.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ma.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cz.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sw.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xv.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://be.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://sv.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fq.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://gp.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pe.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bd.nszjky.cn

Go:   encoding/gob
来源：http://bb.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://xn.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jz.shxzukj.cn

================================================================================
来源：http://ko.newstarts.cn

L. 网络请求
来源：http://va.panjiajie.cn

================================================================================
来源：http://fz.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://mv.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mz.huixinmuqiang.cn


<!-- 参考信息 -->