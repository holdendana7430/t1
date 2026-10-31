代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://us.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vf.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kx.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ne.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rv.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qs.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lh.szxytkj.cn

[H10] 资源自动释放
来源：http://hj.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ah.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vm.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rs.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zn.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bk.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://gn.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bf.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jt.shxzskj.cn

================================================================================
来源：http://jx.bjjhwx.cn

I. 正则表达式
来源：http://bj.muxihuayi.cn

================================================================================
来源：http://by.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://jq.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tl.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sm.hahajie.cn

JS:   /\d+/.test(s)
来源：http://yl.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://do.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bh.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gu.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://me.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qx.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://ea.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://qf.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ta.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wa.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://qd.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ab.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mf.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://qq.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oh.wgjwhj.cn

[I03] 提取捕获分组
来源：http://sz.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kc.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pb.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fx.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ea.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hj.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gk.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://um.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pb.hahajie.cn

[I04] 正则替换
来源：http://mf.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qe.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nb.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xk.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://co.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nq.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xu.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mg.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mp.huixiangedu.cn

[I05] 按正则拆分
来源：http://mk.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vg.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ad.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://if.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://vg.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://ki.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://js.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zy.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lz.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gz.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oe.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://us.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qe.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nw.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fd.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mw.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eq.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tr.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://kn.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lr.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dl.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ay.yuexingan06.cn

TS:   /error/gim
来源：http://gr.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qk.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fv.521024.cn

Ruby: s.scan(/error/i)
来源：http://pt.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://st.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://pi.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ej.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qh.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oi.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ki.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zz.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sc.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hp.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pu.jianghongdianzi.cn

================================================================================
来源：http://bb.shxzukj.cn

J. 日期与时间
来源：http://hs.colortex.cn

================================================================================
来源：http://ih.szxytkj.cn

[J01] 获取当前时间
来源：http://oz.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lz.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rs.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://us.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://hp.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rq.muxihuayi.cn

Go:   time.Now()
来源：http://xf.yuexingan06.cn

Ruby: Time.now
来源：http://gl.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sx.521024.cn

[J02] 格式化输出
来源：http://vc.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uq.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xp.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nw.shxzukj.cn

TS:   d.toISOString()
来源：http://wm.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ig.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bz.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oj.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wv.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://en.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vh.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://rr.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://pe.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uv.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tz.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://iv.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gs.colortex.cn

[J04] 时间戳与日期互转
来源：http://ls.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ux.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lz.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pc.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ov.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://su.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kw.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://il.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ue.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://yn.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://zj.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://is.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dj.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tv.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://uh.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://we.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://rm.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ut.hahajie.cn

[J06] 计算两时间之差
来源：http://ac.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://it.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ht.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wa.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ok.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://an.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://jp.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ra.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://cl.bookmarksfly.cn

[J07] 比较两个日期
来源：http://tb.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://of.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ez.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qg.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wq.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jq.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xy.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iw.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://vq.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://zw.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sl.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ml.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ui.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ml.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bf.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xz.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wq.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sl.haigaiapp.cn

[J09] 时区处理
来源：http://iq.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xm.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sc.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wn.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uw.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jg.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hi.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vq.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://xd.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eh.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qw.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://et.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ia.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://za.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eg.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ag.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sc.panjiajie.cn

================================================================================
来源：http://td.nszjky.cn

K. JSON 与序列化
来源：http://am.asd995.cn

================================================================================
来源：http://nm.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://ln.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pt.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ug.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://gu.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://es.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fe.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://li.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oj.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vl.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ma.shtwfgs.cn

Py:   json.loads(s)
来源：http://bz.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mk.nicolike.cn

JS:   JSON.parse(s)
来源：http://ey.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://cr.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gw.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ky.nicolike.cn

Ruby: JSON.parse(s)
来源：http://yj.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mw.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://ny.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qy.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nx.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cx.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://te.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sd.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ul.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oq.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://st.asd995.cn

[K04] 读取 JSON 文件
来源：http://qy.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wu.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xu.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xz.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vb.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xu.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gc.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ob.bjjhwx.cn

[K05] 深拷贝对象
来源：http://tr.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://fj.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://fz.hahajie.cn

JS:   structuredClone(obj)
来源：http://gp.asd995.cn

TS:   structuredClone(obj)
来源：http://fj.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cu.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://os.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dy.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cq.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://td.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nu.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wd.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bd.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fx.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ol.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vz.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nf.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qw.bjjhwx.cn

[K07] 进制转换
来源：http://bi.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://en.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yj.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zk.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://td.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ck.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zg.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yr.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mf.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://an.asd995.cn

Py:   pickle.dumps(obj)
来源：http://lj.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eq.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://lf.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://bx.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jk.haigaiapp.cn

Go:   encoding/gob
来源：http://zi.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://iy.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://el.huanxung.cn

================================================================================
来源：http://ir.9csxet.cn

L. 网络请求
来源：http://cx.shtwfgs.cn

================================================================================
来源：http://bk.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://gw.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ag.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fx.shxzukj.cn

JS:   await fetch(url)
来源：http://wc.shxzskj.cn

TS:   await fetch(url)
来源：http://ih.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zb.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://xm.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cq.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mv.9csxet.cn

[L02] 发送 POST JSON
来源：http://zj.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ij.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mo.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://il.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yo.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kp.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://om.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://px.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://zr.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://za.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fm.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yw.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ea.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://va.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yg.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vx.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cv.huixiangedu.cn

[L04] 设置超时
来源：http://py.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ji.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xt.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fs.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://st.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ed.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wc.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qn.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lx.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://si.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nt.panjiajie.cn


<!-- 参考信息 -->