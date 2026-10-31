代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ju.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ha.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nw.haigaiapp.cn

[H10] 资源自动释放
来源：http://ye.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xi.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hw.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://la.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ne.szsharing.cn

Go:   defer f.Close()
来源：http://vz.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mm.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://si.shtwfgs.cn

================================================================================
来源：http://dq.hnjuh.cn

I. 正则表达式
来源：http://ff.521024.cn

================================================================================
来源：http://qw.newstarts.cn

[I01] 判断是否匹配
来源：http://se.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pp.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nc.9csxet.cn

JS:   /\d+/.test(s)
来源：http://dm.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://tx.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fw.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gy.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://sc.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vp.chemitech.net.cn

[I02] 提取所有匹配
来源：http://mz.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://wz.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gs.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ck.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://sy.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ql.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mj.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://cr.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kr.huixiangedu.cn

[I03] 提取捕获分组
来源：http://tv.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ap.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://du.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nl.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bd.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xg.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cr.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ll.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xa.huixiangedu.cn

[I04] 正则替换
来源：http://ev.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vy.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://we.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rg.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vs.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://av.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ue.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://km.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fv.yuexingan06.cn

[I05] 按正则拆分
来源：http://gd.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://he.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://av.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://ly.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://mr.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://jx.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bq.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nr.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pf.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ro.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ow.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nq.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sm.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tk.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wk.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qt.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ve.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ug.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://md.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dj.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ax.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hb.colortex.cn

TS:   /error/gim
来源：http://xm.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oz.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sy.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://cp.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gn.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://qd.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mq.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ej.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hd.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ks.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ov.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yk.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vb.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ff.hahajie.cn

================================================================================
来源：http://es.chemitech.net.cn

J. 日期与时间
来源：http://ps.jianghongdianzi.cn

================================================================================
来源：http://ko.newstarts.cn

[J01] 获取当前时间
来源：http://rh.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://da.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xr.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://og.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://wj.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dt.jctech888.com.cn

Go:   time.Now()
来源：http://dv.nicolike.cn

Ruby: Time.now
来源：http://yc.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xw.shxzukj.cn

[J02] 格式化输出
来源：http://bm.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sb.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wd.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sa.yuexingan06.cn

TS:   d.toISOString()
来源：http://co.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sy.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ax.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://le.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cs.lnxyls.cn

[J03] 字符串解析为日期
来源：http://cj.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bi.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ih.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://vd.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://uj.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://de.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ay.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://iu.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fr.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://kn.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gx.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://js.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xn.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vx.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://li.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zl.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hs.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ys.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://mj.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://zz.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zv.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hn.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nh.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://we.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vy.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://hy.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ua.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://mz.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://kd.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://kf.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vw.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://za.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qt.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://bk.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://kt.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://uk.jctech888.com.cn

[J07] 比较两个日期
来源：http://jw.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://cj.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hy.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pg.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lc.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jm.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rd.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dd.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://no.szsharing.cn

[J08] 提取年月日与星期
来源：http://cc.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vy.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://li.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xw.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ho.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vp.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gh.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ot.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ib.haigaiapp.cn

[J09] 时区处理
来源：http://hw.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lk.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ka.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://et.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cc.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ih.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sp.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wq.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://ea.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bh.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ae.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rg.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yh.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mw.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zl.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tv.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://az.huixiangedu.cn

================================================================================
来源：http://ed.shxzskj.cn

K. JSON 与序列化
来源：http://mv.huanxung.cn

================================================================================
来源：http://jb.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://kr.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pb.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rj.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://tr.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://am.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xc.hahajie.cn

Go:   json.Marshal(obj)
来源：http://qe.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cd.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uj.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://di.newstarts.cn

Py:   json.loads(s)
来源：http://by.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lg.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://go.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://nx.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://az.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://qs.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://qy.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qf.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://uv.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sa.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rl.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xa.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tt.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://an.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fo.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bu.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jc.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://th.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yh.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iu.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hb.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ec.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fq.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ae.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nv.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dg.chemitech.net.cn

[K05] 深拷贝对象
来源：http://zg.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://js.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://ju.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://on.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://yd.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rr.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qz.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kg.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dg.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://rv.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uc.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xa.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ek.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ux.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qe.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dh.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xw.yuntaijiaju.cn

[K07] 进制转换
来源：http://we.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nz.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ld.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nn.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sh.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://th.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mh.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cz.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ba.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://pb.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://qg.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xv.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://bw.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://wl.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cj.asd995.cn

Go:   encoding/gob
来源：http://zq.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ra.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zg.nszjky.cn

================================================================================
来源：http://pt.shtwfgs.cn

L. 网络请求
来源：http://yz.shxzskj.cn

================================================================================
来源：http://uz.huanxung.cn

[L01] 发送 GET 请求
来源：http://pi.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pd.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fs.shxzskj.cn

JS:   await fetch(url)
来源：http://su.muxihuayi.cn

TS:   await fetch(url)
来源：http://wg.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jf.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://vr.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ta.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://gh.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eo.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mm.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cd.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xu.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lm.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ti.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yf.szsharing.cn

[L03] 设置自定义请求头
来源：http://li.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gp.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zp.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kt.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sj.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sv.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lz.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sn.haigaiapp.cn

[L04] 设置超时
来源：http://wm.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://fd.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://em.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xd.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dq.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qr.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eu.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wa.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ka.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://vo.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rl.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://br.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mi.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lz.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wx.muxihuayi.cn


<!-- 参考信息 -->