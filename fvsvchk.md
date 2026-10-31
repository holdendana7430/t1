代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ru.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sp.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gv.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mw.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://da.shtwfgs.cn

Go:   defer f.Close()
来源：http://hg.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dm.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vo.huixinmuqiang.cn

================================================================================
来源：http://wh.huanxung.cn

I. 正则表达式
来源：http://cd.asd995.cn

================================================================================
来源：http://fs.wgjwhj.cn

[I01] 判断是否匹配
来源：http://jx.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://du.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qm.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://dh.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://tw.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rs.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jh.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://vd.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uu.nszjky.cn

[I02] 提取所有匹配
来源：http://uo.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://fl.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wb.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sd.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://jv.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://li.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bb.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://wo.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xh.jctech888.com.cn

[I03] 提取捕获分组
来源：http://mw.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wj.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://at.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ft.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ej.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hl.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lb.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ff.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ze.shxzukj.cn

[I04] 正则替换
来源：http://wf.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gc.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xu.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ju.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cp.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xu.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rj.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dw.yuexingan06.cn

[I05] 按正则拆分
来源：http://py.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ec.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vt.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://pc.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://gn.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://jn.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://az.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://am.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zv.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gx.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oa.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xp.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ak.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hi.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://om.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zf.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xd.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://br.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://pn.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bu.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wj.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ac.huixinmuqiang.cn

TS:   /error/gim
来源：http://mw.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zb.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ky.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://ri.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bm.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://jd.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kg.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fg.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pd.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rv.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zo.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ho.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tu.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://we.panjiajie.cn

================================================================================
来源：http://mk.huixinmuqiang.cn

J. 日期与时间
来源：http://bp.bjjhwx.cn

================================================================================
来源：http://ar.szsharing.cn

[J01] 获取当前时间
来源：http://jh.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fa.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mu.hahajie.cn

JS:   new Date();  Date.now()
来源：http://kv.huanxung.cn

TS:   new Date();  Date.now()
来源：http://ne.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ne.bjjhwx.cn

Go:   time.Now()
来源：http://aw.muxihuayi.cn

Ruby: Time.now
来源：http://pg.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wp.hahajie.cn

[J02] 格式化输出
来源：http://mz.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sz.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lw.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wz.panjiajie.cn

TS:   d.toISOString()
来源：http://fw.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sy.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rm.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fj.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vf.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://by.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://za.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dm.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://rr.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ma.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uk.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rt.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://sp.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vs.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://va.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yn.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fq.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hn.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gf.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xk.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kf.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dg.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zn.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://ux.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://qt.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pt.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bg.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xi.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ya.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ks.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ur.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gx.haigaiapp.cn

[J06] 计算两时间之差
来源：http://zz.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://xs.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://in.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mt.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://og.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://wt.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://tb.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://uo.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://cw.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://pv.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jc.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ix.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bh.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://br.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lj.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://bu.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://ff.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ia.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tw.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tf.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ef.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sh.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ax.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dc.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uu.bjjhwx.cn

[J09] 时区处理
来源：http://si.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iq.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nl.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mk.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tl.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rp.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pi.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pa.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ql.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://rt.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gq.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lx.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ny.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cu.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cl.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rz.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gr.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ho.jianghongdianzi.cn

================================================================================
来源：http://ol.szxytkj.cn

K. JSON 与序列化
来源：http://wo.huanxung.cn

================================================================================
来源：http://hg.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://vu.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dc.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oa.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ue.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://nq.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gi.521024.cn

Go:   json.Marshal(obj)
来源：http://xs.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qk.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nf.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://pd.nicolike.cn

Py:   json.loads(s)
来源：http://mf.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kp.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://kq.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ic.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bg.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://kf.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://hm.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rp.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://th.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://es.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zi.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kl.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ci.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://io.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ln.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sy.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mi.nicolike.cn

[K04] 读取 JSON 文件
来源：http://el.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gr.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tk.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xg.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ku.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kv.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ng.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vz.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xn.shxzukj.cn

[K05] 深拷贝对象
来源：http://wc.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://oq.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://zj.shxzskj.cn

JS:   structuredClone(obj)
来源：http://cd.nicolike.cn

TS:   structuredClone(obj)
来源：http://st.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hh.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://te.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gj.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cb.colortex.cn

[K06] 解析 URL 查询串
来源：http://rb.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hx.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gn.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://st.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bm.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oj.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qv.bookmarksfly.cn

[K07] 进制转换
来源：http://fu.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gc.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uo.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ay.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zm.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ht.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ib.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hj.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://vf.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://xh.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ve.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://jn.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://fl.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eb.asd995.cn

Go:   encoding/gob
来源：http://wi.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://ko.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rt.shxzskj.cn

================================================================================
来源：http://zx.bookmarksfly.cn

L. 网络请求
来源：http://vl.colortex.cn

================================================================================
来源：http://nm.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://ku.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zr.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kv.huanxung.cn

JS:   await fetch(url)
来源：http://uk.haigaiapp.cn

TS:   await fetch(url)
来源：http://qr.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://si.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://re.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bo.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://et.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://se.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vu.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wd.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cc.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oe.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tj.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ch.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hh.newstarts.cn

[L03] 设置自定义请求头
来源：http://yi.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yx.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://es.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ge.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://su.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ik.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cy.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pk.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ln.shtwfgs.cn

[L04] 设置超时
来源：http://hk.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://uk.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ow.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vm.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oj.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vw.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pq.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wx.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bd.hahajie.cn

[L05] 上传文件（multipart）
来源：http://pq.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wu.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fu.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vb.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vf.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tr.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pt.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xt.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ai.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://wx.yuntaijiaju.cn


<!-- 参考信息 -->