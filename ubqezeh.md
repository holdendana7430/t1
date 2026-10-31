代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://dq.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hq.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ly.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ra.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zb.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fy.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ty.521024.cn

[H10] 资源自动释放
来源：http://cy.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ki.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qk.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ih.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cr.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sj.nszjky.cn

Go:   defer f.Close()
来源：http://oi.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qj.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bv.nicolike.cn

================================================================================
来源：http://kw.yuexingan06.cn

I. 正则表达式
来源：http://zd.panjiajie.cn

================================================================================
来源：http://yc.muxihuayi.cn

[I01] 判断是否匹配
来源：http://kn.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qj.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ie.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://bp.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://qt.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://by.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hd.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ww.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ug.9csxet.cn

[I02] 提取所有匹配
来源：http://eo.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://iz.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yq.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nn.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://qg.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mu.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cn.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://qo.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ph.yuexingan06.cn

[I03] 提取捕获分组
来源：http://gh.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sb.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mx.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yk.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ok.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bd.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hr.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ev.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dk.jctech888.com.cn

[I04] 正则替换
来源：http://aw.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nu.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yf.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eo.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uj.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://th.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://am.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mt.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cv.nicolike.cn

[I05] 按正则拆分
来源：http://ic.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dl.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://er.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://sd.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gk.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://by.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qa.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://is.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xm.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hy.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ll.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oa.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rm.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ow.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oj.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dx.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dl.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hr.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://qp.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vt.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xa.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://df.shtwfgs.cn

TS:   /error/gim
来源：http://hg.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xj.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zp.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://jt.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ny.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sf.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ea.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bg.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sd.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ze.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://na.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mc.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sc.9csxet.cn

================================================================================
来源：http://fe.huixinmuqiang.cn

J. 日期与时间
来源：http://kj.szsharing.cn

================================================================================
来源：http://cg.nszjky.cn

[J01] 获取当前时间
来源：http://tf.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ut.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lw.hahajie.cn

JS:   new Date();  Date.now()
来源：http://uq.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://kr.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nw.jctech888.com.cn

Go:   time.Now()
来源：http://go.haigaiapp.cn

Ruby: Time.now
来源：http://nu.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mi.521024.cn

[J02] 格式化输出
来源：http://ve.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jp.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://py.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xo.bjjhwx.cn

TS:   d.toISOString()
来源：http://rn.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zx.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ps.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wt.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://af.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ch.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ib.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mw.521024.cn

JS:   new Date("2024-01-02")
来源：http://pz.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://df.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kt.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fi.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://wf.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bg.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://vg.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lv.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wl.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yy.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rc.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dc.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ah.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qy.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://im.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://vc.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://nz.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://as.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ue.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sl.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://jm.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xb.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://tz.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hh.nszjky.cn

[J06] 计算两时间之差
来源：http://hw.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://hp.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://mb.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hj.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zf.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ds.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://qc.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://wh.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://lz.jctech888.com.cn

[J07] 比较两个日期
来源：http://ao.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ya.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lp.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iy.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fz.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pn.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hb.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nr.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://uk.szsharing.cn

[J08] 提取年月日与星期
来源：http://px.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ml.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jc.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cq.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vs.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ql.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gz.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://it.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jh.newstarts.cn

[J09] 时区处理
来源：http://jg.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tj.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yj.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sz.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qt.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sm.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sk.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qj.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hy.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://gj.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ch.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lo.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://es.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xs.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dp.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uc.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xy.gzmigu.cn

================================================================================
来源：http://jh.huixinmuqiang.cn

K. JSON 与序列化
来源：http://wk.521024.cn

================================================================================
来源：http://gl.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://fa.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qs.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wr.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://au.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://yy.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sc.hahajie.cn

Go:   json.Marshal(obj)
来源：http://hw.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yi.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vg.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://ie.nicolike.cn

Py:   json.loads(s)
来源：http://ic.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ln.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ek.colortex.cn

TS:   JSON.parse(s)
来源：http://fq.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://te.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://hd.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://iu.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qw.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://tw.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kz.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sw.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ly.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ja.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ag.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sn.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iu.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zc.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ug.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ks.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mv.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tn.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vr.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iv.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://re.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wq.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fz.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://yr.521024.cn

Py:   copy.deepcopy(obj)
来源：http://jy.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ut.gzmigu.cn

JS:   structuredClone(obj)
来源：http://dh.shxzskj.cn

TS:   structuredClone(obj)
来源：http://ab.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jj.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cq.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rg.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://by.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://yy.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pg.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pk.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ho.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ex.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ru.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zl.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ul.huixinmuqiang.cn

[K07] 进制转换
来源：http://az.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://di.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ul.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zl.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ug.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://to.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dz.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wp.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ww.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://xw.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://ce.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cm.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qt.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ww.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zh.hahajie.cn

Go:   encoding/gob
来源：http://uu.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ue.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sh.nszjky.cn

================================================================================
来源：http://td.panjiajie.cn

L. 网络请求
来源：http://yn.521024.cn

================================================================================
来源：http://pi.panjiajie.cn

[L01] 发送 GET 请求
来源：http://sa.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ro.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haigaiapp.cn

JS:   await fetch(url)
来源：http://ma.shxzskj.cn

TS:   await fetch(url)
来源：http://kp.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lz.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://ve.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dn.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jp.hnjuh.cn

[L02] 发送 POST JSON
来源：http://zz.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ul.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dw.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ok.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sa.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mn.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qv.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mn.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bo.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://fm.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pe.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yu.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yu.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lj.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vh.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rw.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lz.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://si.521024.cn

[L04] 设置超时
来源：http://oj.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://mp.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bb.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://le.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ej.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vp.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qz.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vo.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ic.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://pm.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rm.colortex.cn


<!-- 参考信息 -->