代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://zq.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://on.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mu.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wn.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://je.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nc.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mq.yuexingan06.cn

[H10] 资源自动释放
来源：http://fa.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yz.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zw.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jo.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gx.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xf.chemitech.net.cn

Go:   defer f.Close()
来源：http://ov.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mc.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://st.lnxyls.cn

================================================================================
来源：http://it.gzmigu.cn

I. 正则表达式
来源：http://ki.huanxung.cn

================================================================================
来源：http://lh.521024.cn

[I01] 判断是否匹配
来源：http://ci.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nx.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ln.521024.cn

JS:   /\d+/.test(s)
来源：http://pj.huanxung.cn

TS:   /\d+/.test(s)
来源：http://fv.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pv.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qy.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://cf.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rj.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://ig.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://ah.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lv.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gg.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://jm.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sk.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ar.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://qf.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ga.haigaiapp.cn

[I03] 提取捕获分组
来源：http://gl.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cs.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pr.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nz.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cp.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qw.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://po.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dy.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wgjwhj.cn

[I04] 正则替换
来源：http://fx.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yh.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://af.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ga.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sl.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ht.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kt.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dy.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ag.newstarts.cn

[I05] 按正则拆分
来源：http://gi.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://al.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ta.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://sm.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://le.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://da.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pg.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://is.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zf.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gt.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jd.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xo.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ok.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oh.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qx.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bp.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zs.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kk.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://gr.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://id.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iv.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xy.muxihuayi.cn

TS:   /error/gim
来源：http://bp.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://di.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ut.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://nc.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pk.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ft.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nc.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eb.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zh.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://up.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ji.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nt.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lb.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wf.gzmigu.cn

================================================================================
来源：http://rk.shtwfgs.cn

J. 日期与时间
来源：http://ax.jctech888.com.cn

================================================================================
来源：http://ts.wgjwhj.cn

[J01] 获取当前时间
来源：http://xl.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xl.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kb.hahajie.cn

JS:   new Date();  Date.now()
来源：http://gw.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://hk.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gp.hahajie.cn

Go:   time.Now()
来源：http://ny.bjjhwx.cn

Ruby: Time.now
来源：http://sx.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xd.bjjhwx.cn

[J02] 格式化输出
来源：http://sg.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://py.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hl.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://il.huanxung.cn

TS:   d.toISOString()
来源：http://rd.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pz.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ji.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rb.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ky.newstarts.cn

[J03] 字符串解析为日期
来源：http://uw.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dn.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xn.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://us.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://oy.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lf.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oi.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://me.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ui.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://vw.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://so.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pk.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gk.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ls.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nm.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://er.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://em.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uu.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://ee.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://ke.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bj.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mf.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://is.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://hj.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xj.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://qz.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tz.chemitech.net.cn

[J06] 计算两时间之差
来源：http://qh.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://kg.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://kq.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iq.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://df.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xi.521024.cn

Go:   end.Sub(start).Hours()
来源：http://mi.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://er.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://jd.gzmigu.cn

[J07] 比较两个日期
来源：http://ep.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://nl.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ks.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mo.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kw.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uf.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ji.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://du.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://zd.gzmigu.cn

[J08] 提取年月日与星期
来源：http://vh.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bq.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ua.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ip.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://an.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qi.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fe.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jr.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mg.gzmigu.cn

[J09] 时区处理
来源：http://ut.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://je.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zt.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mu.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qq.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nz.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ez.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iw.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://bg.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uh.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sy.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dx.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ms.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hy.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://to.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fp.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://db.shtwfgs.cn

================================================================================
来源：http://ir.nicolike.cn

K. JSON 与序列化
来源：http://ot.szsharing.cn

================================================================================
来源：http://zz.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://fz.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ly.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nc.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://cq.asd995.cn

TS:   JSON.stringify(obj)
来源：http://sg.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ro.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://bf.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ef.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pu.nicolike.cn

[K02] JSON 字符串转对象
来源：http://pc.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://qj.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pr.521024.cn

JS:   JSON.parse(s)
来源：http://jp.szxytkj.cn

TS:   JSON.parse(s)
来源：http://ep.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://co.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://ld.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://tw.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ws.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dk.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ks.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kc.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://no.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aa.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nr.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qy.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gi.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ns.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ug.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://io.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qe.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hy.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wj.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ly.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tc.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ya.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zt.9csxet.cn

[K05] 深拷贝对象
来源：http://dw.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://wo.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://lp.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://in.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://lb.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ay.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tg.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nv.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vy.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://za.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ik.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dv.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ed.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mc.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ob.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ic.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yv.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vo.9csxet.cn

[K07] 进制转换
来源：http://xg.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://au.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qa.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ug.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xf.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lz.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cd.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gt.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cp.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qo.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://vd.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xs.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ln.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://yy.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.bjjhwx.cn

Go:   encoding/gob
来源：http://rk.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://hn.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uc.521024.cn

================================================================================
来源：http://jk.hnjuh.cn

L. 网络请求
来源：http://eh.muxihuayi.cn

================================================================================
来源：http://ax.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://hp.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ly.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jn.wgjwhj.cn

JS:   await fetch(url)
来源：http://ke.shxzskj.cn

TS:   await fetch(url)
来源：http://kh.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fo.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://uj.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ej.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sv.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://rc.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pm.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nq.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ng.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xh.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hv.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qu.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mc.nszjky.cn

[L03] 设置自定义请求头
来源：http://gq.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aa.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lm.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xa.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://is.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uc.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oc.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lx.szxytkj.cn

[L04] 设置超时
来源：http://xo.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://ot.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zp.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://al.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oa.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jh.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ya.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gb.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qp.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://bz.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mr.huixiangedu.cn


<!-- 参考信息 -->