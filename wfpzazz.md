代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ze.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://cz.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xy.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://vl.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ke.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://oc.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pp.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://rb.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://ip.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mm.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hi.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nb.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oo.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ym.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://ye.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://sh.szsharing.cn

[H07] 断言
来源：http://ob.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://qz.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://ho.hahajie.cn

JS:   console.assert(x > 0);
来源：http://wa.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://ok.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://dd.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vq.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fw.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://me.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://jq.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://sq.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bv.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://ll.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vd.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xo.hahajie.cn

Go:   err.Error()
来源：http://nz.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://ob.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://bm.hnjuh.cn

[H09] 带错误码的异常
来源：http://cl.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ce.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qv.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mh.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zt.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yl.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wq.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://er.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bi.szsharing.cn

[H10] 资源自动释放
来源：http://iu.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yf.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cv.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gr.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fm.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://at.newstarts.cn

Go:   defer f.Close()
来源：http://wp.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xw.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ub.szxytkj.cn

================================================================================
来源：http://wa.shxzukj.cn

I. 正则表达式
来源：http://jp.asd995.cn

================================================================================
来源：http://hc.521024.cn

[I01] 判断是否匹配
来源：http://jc.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dh.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vq.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://aa.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://an.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gv.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kp.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://jy.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wy.huixiangedu.cn

[I02] 提取所有匹配
来源：http://wu.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://xy.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gh.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pb.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://xx.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ab.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fw.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://fk.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tj.szxytkj.cn

[I03] 提取捕获分组
来源：http://ua.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gp.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zb.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://af.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zh.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gp.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mk.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ln.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://al.colortex.cn

[I04] 正则替换
来源：http://qi.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://at.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vq.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ut.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ug.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nn.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ny.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jr.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ij.panjiajie.cn

[I05] 按正则拆分
来源：http://an.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://je.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gw.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://un.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://oz.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://ss.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mj.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xx.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://td.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://im.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ac.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wd.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ev.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gg.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dx.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ea.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yt.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://jz.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jz.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hq.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zr.newstarts.cn

TS:   /error/gim
来源：http://bm.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xs.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://na.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://sc.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fs.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://zd.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mw.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://na.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ml.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ba.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wl.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vw.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qy.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ei.jianghongdianzi.cn

================================================================================
来源：http://lo.panjiajie.cn

J. 日期与时间
来源：http://cj.nicolike.cn

================================================================================
来源：http://gu.colortex.cn

[J01] 获取当前时间
来源：http://er.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rn.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ty.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://fo.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://ko.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vw.szxytkj.cn

Go:   time.Now()
来源：http://yq.shxzskj.cn

Ruby: Time.now
来源：http://zl.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xm.shxzukj.cn

[J02] 格式化输出
来源：http://fv.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fp.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ad.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ez.panjiajie.cn

TS:   d.toISOString()
来源：http://hm.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bx.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pa.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ej.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lm.hahajie.cn

[J03] 字符串解析为日期
来源：http://fh.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fl.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://di.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://gs.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://vd.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jz.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dn.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://pf.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gf.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ex.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ps.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vi.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://se.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dr.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pm.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ii.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ti.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sz.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://by.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://cq.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jj.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oa.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jw.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://iw.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vk.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://bp.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kl.shxzskj.cn

[J06] 计算两时间之差
来源：http://xx.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://lj.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://dp.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jz.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nx.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pl.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://fe.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://jj.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://po.nszjky.cn

[J07] 比较两个日期
来源：http://xq.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://wf.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wt.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sp.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xa.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oz.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pe.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mv.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://cb.colortex.cn

[J08] 提取年月日与星期
来源：http://cm.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kv.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wo.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vr.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vp.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mk.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mu.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vy.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iy.asd995.cn

[J09] 时区处理
来源：http://kf.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lx.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dq.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sw.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ds.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jm.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://df.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ao.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fq.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://jb.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pg.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qf.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ik.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ii.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mz.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mg.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qy.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gd.jianghongdianzi.cn

================================================================================
来源：http://ue.huixinmuqiang.cn

K. JSON 与序列化
来源：http://tp.chemitech.net.cn

================================================================================
来源：http://vc.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://le.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nk.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xe.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://uf.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://fr.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://si.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ya.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ei.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kp.9csxet.cn

[K02] JSON 字符串转对象
来源：http://od.huanxung.cn

Py:   json.loads(s)
来源：http://oi.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hl.szsharing.cn

JS:   JSON.parse(s)
来源：http://pf.panjiajie.cn

TS:   JSON.parse(s)
来源：http://rm.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ux.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ta.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://fq.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xj.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://yf.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zu.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dv.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rr.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fo.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dk.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rm.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uy.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://kk.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wm.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rr.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cl.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lg.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ua.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://le.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vd.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qz.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://jq.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://pe.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://se.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://tx.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://nf.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sg.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mx.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eq.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mk.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://yl.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xx.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dc.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cb.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oo.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uc.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uz.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://on.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mz.panjiajie.cn

[K07] 进制转换
来源：http://qt.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pp.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sk.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rj.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pe.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gl.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xt.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vs.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fz.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://og.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://rs.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dz.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ku.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tp.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jg.yuexingan06.cn

Go:   encoding/gob
来源：http://hk.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://fc.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jn.szxytkj.cn

================================================================================
来源：http://tk.muxihuayi.cn

L. 网络请求
来源：http://wt.huanxung.cn

================================================================================
来源：http://ja.521024.cn

[L01] 发送 GET 请求
来源：http://ts.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://om.jctech888.com.cn


<!-- 参考信息 -->