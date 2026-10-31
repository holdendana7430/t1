代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oh.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vr.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cd.huixiangedu.cn

[H10] 资源自动释放
来源：http://gs.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kw.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jt.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mw.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nt.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bo.szxytkj.cn

Go:   defer f.Close()
来源：http://kl.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sn.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ch.szsharing.cn

================================================================================
来源：http://vi.szxytkj.cn

I. 正则表达式
来源：http://rd.newstarts.cn

================================================================================
来源：http://js.hahajie.cn

[I01] 判断是否匹配
来源：http://jm.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gh.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yu.szsharing.cn

JS:   /\d+/.test(s)
来源：http://dv.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://dh.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kr.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bx.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://eb.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://po.9csxet.cn

[I02] 提取所有匹配
来源：http://ob.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://xw.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lz.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gr.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://iz.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ye.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xt.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://pw.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uz.haigaiapp.cn

[I03] 提取捕获分组
来源：http://rv.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zr.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ia.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ub.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zh.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sm.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://py.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jo.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nt.haigaiapp.cn

[I04] 正则替换
来源：http://yl.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cf.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lp.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ri.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sx.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eu.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ya.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bi.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pt.521024.cn

[I05] 按正则拆分
来源：http://lf.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jp.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qa.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://xz.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://pw.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://bh.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bn.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://em.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ka.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xm.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tv.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kf.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ix.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lv.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mn.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bt.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://et.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dl.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://sv.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lp.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fq.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sb.hnjuh.cn

TS:   /error/gim
来源：http://ux.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ii.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nk.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://bl.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://we.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ae.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qw.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yd.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xb.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ma.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dc.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://le.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ar.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sz.bookmarksfly.cn

================================================================================
来源：http://ty.panjiajie.cn

J. 日期与时间
来源：http://tj.hahajie.cn

================================================================================
来源：http://ma.szxytkj.cn

[J01] 获取当前时间
来源：http://bo.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dy.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://og.9csxet.cn

JS:   new Date();  Date.now()
来源：http://kw.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://cf.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wx.asd995.cn

Go:   time.Now()
来源：http://kw.huixiangedu.cn

Ruby: Time.now
来源：http://tb.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jy.bjjhwx.cn

[J02] 格式化输出
来源：http://ck.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ft.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qi.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gk.yuexingan06.cn

TS:   d.toISOString()
来源：http://pq.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iy.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ia.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qq.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ot.hahajie.cn

[J03] 字符串解析为日期
来源：http://gk.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rj.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ee.521024.cn

JS:   new Date("2024-01-02")
来源：http://zm.asd995.cn

TS:   new Date("2024-01-02")
来源：http://tk.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ut.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yo.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://lg.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jv.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://nv.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ly.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ej.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zj.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tu.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mj.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vt.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://br.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://el.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://bb.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://gx.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://as.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nl.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sf.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ai.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://df.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://qx.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ry.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://yx.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://ll.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://hi.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ys.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jg.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gb.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://li.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://dd.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ql.asd995.cn

[J07] 比较两个日期
来源：http://gh.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://or.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ns.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lb.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dh.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lf.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://re.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cs.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ch.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://lf.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bz.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gn.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bg.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://du.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ql.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kg.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qm.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vq.huixinmuqiang.cn

[J09] 时区处理
来源：http://tr.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iz.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tc.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://co.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yz.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ka.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fi.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lg.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fx.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://rv.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zz.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ns.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mx.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://or.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pu.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kp.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kd.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cp.nicolike.cn

================================================================================
来源：http://rl.jianghongdianzi.cn

K. JSON 与序列化
来源：http://dj.hnjuh.cn

================================================================================
来源：http://xh.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ik.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yv.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cb.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ft.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ol.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pv.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://fa.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ic.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://re.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://sp.gzmigu.cn

Py:   json.loads(s)
来源：http://wv.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jl.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://lt.shxzskj.cn

TS:   JSON.parse(s)
来源：http://lh.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qw.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://gb.nszjky.cn

Ruby: JSON.parse(s)
来源：http://qs.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yh.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ev.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ni.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gz.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rg.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dl.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hs.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://po.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qy.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ai.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://qs.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://az.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iy.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jq.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://da.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hr.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zk.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ol.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://em.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://il.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://am.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://jy.shxzukj.cn

JS:   structuredClone(obj)
来源：http://qt.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://xh.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ek.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lu.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ql.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lv.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://re.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sv.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://be.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yq.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hn.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bk.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aw.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sw.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bi.chemitech.net.cn

[K07] 进制转换
来源：http://fs.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lp.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://du.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xq.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://us.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gi.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rq.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lp.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tl.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qj.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://go.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ya.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ea.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://pv.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ke.shxzukj.cn

Go:   encoding/gob
来源：http://aw.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://yb.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qc.newstarts.cn

================================================================================
来源：http://ji.wgjwhj.cn

L. 网络请求
来源：http://xn.muxihuayi.cn

================================================================================
来源：http://os.colortex.cn

[L01] 发送 GET 请求
来源：http://bk.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bn.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kt.521024.cn

JS:   await fetch(url)
来源：http://xc.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://qw.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gy.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://jh.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tn.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cr.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://yz.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pu.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://is.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sb.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uk.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lk.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dh.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://na.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://co.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://ir.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zq.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vl.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uk.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wu.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hj.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ov.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://po.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jm.panjiajie.cn

[L04] 设置超时
来源：http://yd.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ob.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aw.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qp.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cn.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://au.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ko.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jb.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rx.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://wc.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cs.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cl.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vj.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yq.9csxet.cn


<!-- 参考信息 -->