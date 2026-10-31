代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://zt.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mh.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cn.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nb.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wp.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pv.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tz.huixiangedu.cn

[H10] 资源自动释放
来源：http://up.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jv.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fz.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dq.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mr.asd995.cn

Go:   defer f.Close()
来源：http://ir.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://er.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xz.nszjky.cn

================================================================================
来源：http://nl.haigaiapp.cn

I. 正则表达式
来源：http://gd.jctech888.com.cn

================================================================================
来源：http://lv.szsharing.cn

[I01] 判断是否匹配
来源：http://tt.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jh.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pl.nicolike.cn

JS:   /\d+/.test(s)
来源：http://ga.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://qb.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qp.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://am.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://yl.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://na.szsharing.cn

[I02] 提取所有匹配
来源：http://lq.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://nz.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qq.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ef.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ok.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ju.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zf.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://dd.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mx.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://hg.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cb.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vi.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://on.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yz.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://py.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sv.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wn.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://un.szxytkj.cn

[I04] 正则替换
来源：http://zw.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uw.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qh.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iq.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ux.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dj.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mx.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vd.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sc.szxytkj.cn

[I05] 按正则拆分
来源：http://eb.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oq.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pr.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://uc.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wo.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://ke.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ly.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bh.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vd.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://st.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ud.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cx.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fy.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rg.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://da.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xs.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://la.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nj.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://be.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://il.shxzskj.cn

TS:   /error/gim
来源：http://ud.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dd.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hg.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://zm.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ew.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://cf.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yd.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rd.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://io.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qp.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://md.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cj.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ns.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rs.jctech888.com.cn

================================================================================
来源：http://mj.hnjuh.cn

J. 日期与时间
来源：http://ai.asd995.cn

================================================================================
来源：http://ou.wgjwhj.cn

[J01] 获取当前时间
来源：http://sc.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://do.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lt.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://zq.szsharing.cn

TS:   new Date();  Date.now()
来源：http://vy.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://re.yuexingan06.cn

Go:   time.Now()
来源：http://yb.huixinmuqiang.cn

Ruby: Time.now
来源：http://eh.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yf.lnxyls.cn

[J02] 格式化输出
来源：http://ku.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ah.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wi.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iz.521024.cn

TS:   d.toISOString()
来源：http://dc.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ke.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vz.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vs.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://on.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ss.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nb.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://wg.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://sh.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hh.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rh.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://tr.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sf.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://nz.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kv.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xx.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://su.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nq.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mp.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lo.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cg.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yo.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://wn.521024.cn

Py:   now + timedelta(days=7)
来源：http://zi.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rn.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kp.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nt.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://hd.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://et.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://xm.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zr.muxihuayi.cn

[J06] 计算两时间之差
来源：http://tt.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ot.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://jn.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zh.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dm.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ay.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://kb.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://rn.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://eq.asd995.cn

[J07] 比较两个日期
来源：http://js.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://pu.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ib.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cf.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ox.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ku.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iw.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qv.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://cb.asd995.cn

[J08] 提取年月日与星期
来源：http://ym.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://os.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dx.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://or.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fn.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ov.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qk.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xe.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ga.bookmarksfly.cn

[J09] 时区处理
来源：http://vu.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gu.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qz.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ju.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hd.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lr.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xs.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yy.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hn.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://un.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yp.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lv.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vl.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pa.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jf.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pf.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://og.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://ly.9csxet.cn

K. JSON 与序列化
来源：http://um.yuntaijiaju.cn

================================================================================
来源：http://ac.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://nm.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oy.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vc.colortex.cn

JS:   JSON.stringify(obj)
来源：http://zi.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://cb.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lm.hahajie.cn

Go:   json.Marshal(obj)
来源：http://rt.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zo.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zg.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://lv.huixiangedu.cn

Py:   json.loads(s)
来源：http://qc.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jt.nszjky.cn

JS:   JSON.parse(s)
来源：http://hl.huanxung.cn

TS:   JSON.parse(s)
来源：http://qy.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://at.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://df.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://lp.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xu.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://mz.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dk.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kg.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gu.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mq.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://la.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ur.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tf.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mt.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://id.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bm.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mt.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nk.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xp.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uv.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://va.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tw.bjjhwx.cn

[K05] 深拷贝对象
来源：http://jw.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://zh.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ee.newstarts.cn

JS:   structuredClone(obj)
来源：http://vn.hnjuh.cn

TS:   structuredClone(obj)
来源：http://to.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dl.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nc.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tv.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gq.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://rj.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jk.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tx.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xj.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cz.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://im.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ju.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ac.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nv.gzmigu.cn

[K07] 进制转换
来源：http://mo.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vj.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yf.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ip.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qg.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://io.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xt.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qc.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vu.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://re.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://xt.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rc.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cg.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://xo.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hh.yuntaijiaju.cn

Go:   encoding/gob
来源：http://mv.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://fl.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sv.jianghongdianzi.cn

================================================================================
来源：http://gh.panjiajie.cn

L. 网络请求
来源：http://hk.szxytkj.cn

================================================================================
来源：http://oz.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://hg.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://au.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dd.521024.cn

JS:   await fetch(url)
来源：http://yy.asd995.cn

TS:   await fetch(url)
来源：http://ll.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bb.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://uj.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bt.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ri.newstarts.cn

[L02] 发送 POST JSON
来源：http://fv.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xs.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gm.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iz.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ct.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://es.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iu.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tf.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nh.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://tn.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ql.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tc.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lq.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ei.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ri.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bm.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xu.shtwfgs.cn

[L04] 设置超时
来源：http://jx.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://wy.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jn.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fl.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rp.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yn.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rd.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pn.newstarts.cn

[L05] 上传文件（multipart）
来源：http://cb.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ca.panjiajie.cn


<!-- 参考信息 -->