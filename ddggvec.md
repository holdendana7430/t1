代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://su.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://so.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mt.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gt.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jk.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qg.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hk.muxihuayi.cn

[H10] 资源自动释放
来源：http://xu.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ob.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ww.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://as.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yn.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vd.colortex.cn

Go:   defer f.Close()
来源：http://kt.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sl.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dp.huixinmuqiang.cn

================================================================================
来源：http://il.wgjwhj.cn

I. 正则表达式
来源：http://jb.yuntaijiaju.cn

================================================================================
来源：http://yh.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://fv.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fn.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zy.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://rb.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ln.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://et.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hq.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://um.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fm.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ja.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://kw.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ba.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kv.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://id.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vb.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ua.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://yj.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xh.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://ck.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ti.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ye.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qd.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bb.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gl.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mh.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mf.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mr.newstarts.cn

[I04] 正则替换
来源：http://fq.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gb.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zk.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dq.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wi.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xl.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eb.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://li.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dw.lnxyls.cn

[I05] 按正则拆分
来源：http://sw.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wo.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lh.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://jm.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://jd.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://kz.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fl.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sx.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tl.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ub.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yt.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rf.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mo.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hn.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bu.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yx.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uq.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xw.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ej.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oi.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ym.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://er.yuexingan06.cn

TS:   /error/gim
来源：http://kc.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pa.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jf.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://jr.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zo.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://gw.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rg.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://id.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xo.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lx.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zt.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lk.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wx.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://be.chemitech.net.cn

================================================================================
来源：http://uh.shxzskj.cn

J. 日期与时间
来源：http://mu.lnxyls.cn

================================================================================
来源：http://gc.asd995.cn

[J01] 获取当前时间
来源：http://pk.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dh.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ku.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://dl.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://qk.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jz.hnjuh.cn

Go:   time.Now()
来源：http://il.bjjhwx.cn

Ruby: Time.now
来源：http://uy.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nk.yuntaijiaju.cn

[J02] 格式化输出
来源：http://wr.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tj.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bx.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dt.huixiangedu.cn

TS:   d.toISOString()
来源：http://cz.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qd.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ru.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ut.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kh.hnjuh.cn

[J03] 字符串解析为日期
来源：http://nh.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sb.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rf.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://zo.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://vg.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ru.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vv.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://cj.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://js.szsharing.cn

[J04] 时间戳与日期互转
来源：http://kt.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zo.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vb.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jc.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wv.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://za.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ca.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rs.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ir.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://re.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ut.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://la.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pi.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://dt.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qc.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://jd.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jx.colortex.cn

[J06] 计算两时间之差
来源：http://te.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ut.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://zi.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ff.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nr.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ad.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://uw.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://en.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://lc.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://jp.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://dl.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qd.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qu.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dz.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ol.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mx.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kk.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://lo.panjiajie.cn

[J08] 提取年月日与星期
来源：http://xw.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zi.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rq.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zv.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kr.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xv.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iq.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nc.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cn.colortex.cn

[J09] 时区处理
来源：http://yb.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ab.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://db.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yy.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ia.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ko.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://el.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ec.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vk.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://ha.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yv.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eu.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gf.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fq.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://si.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ww.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ar.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kd.huixiangedu.cn

================================================================================
来源：http://mn.yuntaijiaju.cn

K. JSON 与序列化
来源：http://zw.huixinmuqiang.cn

================================================================================
来源：http://lb.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://qw.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://if.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vg.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://rj.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://dk.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dv.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://as.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sd.521024.cn

[K02] JSON 字符串转对象
来源：http://do.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://qr.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zk.shxzukj.cn

JS:   JSON.parse(s)
来源：http://cx.szxytkj.cn

TS:   JSON.parse(s)
来源：http://cq.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uu.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://zs.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://mn.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://je.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://qp.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://os.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hn.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ju.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tj.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wa.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ko.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dh.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://na.asd995.cn

[K04] 读取 JSON 文件
来源：http://mt.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qy.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zz.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oq.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nc.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bz.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uk.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mf.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bf.chemitech.net.cn

[K05] 深拷贝对象
来源：http://gu.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://qe.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://cv.lnxyls.cn

JS:   structuredClone(obj)
来源：http://ck.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://sd.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ih.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rw.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qy.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ly.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://sl.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fp.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jn.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eh.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zk.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gc.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vq.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zi.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yd.9csxet.cn

[K07] 进制转换
来源：http://tl.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zo.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pd.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nl.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://in.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hh.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ko.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bx.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ni.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://de.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://rm.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lr.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ey.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://go.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oq.9csxet.cn

Go:   encoding/gob
来源：http://as.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ql.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hq.huixiangedu.cn

================================================================================
来源：http://yv.shtwfgs.cn

L. 网络请求
来源：http://ar.wgjwhj.cn

================================================================================
来源：http://hw.shxzskj.cn

[L01] 发送 GET 请求
来源：http://pi.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tu.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zy.asd995.cn

JS:   await fetch(url)
来源：http://ol.szsharing.cn

TS:   await fetch(url)
来源：http://de.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nj.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://mp.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://va.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ea.shxzskj.cn

[L02] 发送 POST JSON
来源：http://zq.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pd.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mb.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://he.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jz.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://os.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zo.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://re.hnjuh.cn

[L03] 设置自定义请求头
来源：http://dr.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sm.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gi.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://st.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zf.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ba.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ku.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kx.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xg.521024.cn

[L04] 设置超时
来源：http://ii.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://wn.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ij.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jx.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zd.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pq.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hx.newstarts.cn

[L05] 上传文件（multipart）
来源：http://es.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ha.szxytkj.cn


<!-- 参考信息 -->