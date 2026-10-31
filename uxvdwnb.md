代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://qy.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nb.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jr.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hb.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://li.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gl.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gd.shxzukj.cn

================================================================================
来源：http://tr.panjiajie.cn

I. 正则表达式
来源：http://iv.jctech888.com.cn

================================================================================
来源：http://tv.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://kk.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ws.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jn.nicolike.cn

JS:   /\d+/.test(s)
来源：http://tm.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://os.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ls.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ga.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://wu.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cl.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://bq.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://co.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://to.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nb.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://fa.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kx.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://am.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hf.huixiangedu.cn

[I03] 提取捕获分组
来源：http://uk.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wx.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ie.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pi.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vq.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rj.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aa.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cg.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mu.shxzskj.cn

[I04] 正则替换
来源：http://zg.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://po.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hu.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://za.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ul.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pc.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://am.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jx.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fl.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://lr.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hv.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aj.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rx.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://wu.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://no.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ij.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ls.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rk.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xt.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fq.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ak.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gj.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://el.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sj.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gu.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zc.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ne.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ko.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zv.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oj.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dm.muxihuayi.cn

TS:   /error/gim
来源：http://sv.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gl.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rp.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ph.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aq.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://cl.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://do.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ck.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lj.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://po.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jm.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ck.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jx.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zv.yuntaijiaju.cn

================================================================================
来源：http://qc.nszjky.cn

J. 日期与时间
来源：http://cg.newstarts.cn

================================================================================
来源：http://jo.szxytkj.cn

[J01] 获取当前时间
来源：http://fk.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gw.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://md.huanxung.cn

JS:   new Date();  Date.now()
来源：http://qb.9csxet.cn

TS:   new Date();  Date.now()
来源：http://eq.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pv.chemitech.net.cn

Go:   time.Now()
来源：http://md.chemitech.net.cn

Ruby: Time.now
来源：http://hb.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pa.huixiangedu.cn

[J02] 格式化输出
来源：http://fa.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://le.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ux.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ul.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://eq.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wi.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sx.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lf.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://or.9csxet.cn

[J03] 字符串解析为日期
来源：http://cc.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dq.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vu.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://zb.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://mg.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qy.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://st.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://gr.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qu.521024.cn

[J04] 时间戳与日期互转
来源：http://cw.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rr.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sw.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qs.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ob.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mg.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jt.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://on.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eu.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://ji.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://nq.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://in.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ff.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uz.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ly.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xf.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://al.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aq.szxytkj.cn

[J06] 计算两时间之差
来源：http://dc.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://us.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://xj.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bu.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://us.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sz.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://wk.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://mo.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://bm.panjiajie.cn

[J07] 比较两个日期
来源：http://in.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://xn.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://on.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vi.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xx.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yg.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hp.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ke.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://pj.shxzskj.cn

[J08] 提取年月日与星期
来源：http://wp.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nd.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wp.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jq.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xd.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://su.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kt.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mj.hahajie.cn

[J09] 时区处理
来源：http://fe.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ue.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://co.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://to.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ky.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ix.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://np.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wh.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://uy.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pl.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sv.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rq.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ka.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ha.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ro.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://st.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rn.hahajie.cn

================================================================================
来源：http://qo.szxytkj.cn

K. JSON 与序列化
来源：http://vc.huixinmuqiang.cn

================================================================================
来源：http://ys.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://oy.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bk.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jf.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://ot.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://vj.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://na.9csxet.cn

Go:   json.Marshal(obj)
来源：http://zy.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://py.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hr.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://hz.lnxyls.cn

Py:   json.loads(s)
来源：http://pv.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ot.gzmigu.cn

JS:   JSON.parse(s)
来源：http://kc.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://au.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fa.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://qk.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://vt.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kh.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://kk.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gt.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ps.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ny.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ck.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mt.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hu.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xz.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://eh.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uk.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ni.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ja.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ha.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ur.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mf.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sz.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rg.shtwfgs.cn

[K05] 深拷贝对象
来源：http://kb.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://an.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://aq.nicolike.cn

JS:   structuredClone(obj)
来源：http://dp.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://de.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wc.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dt.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wd.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ni.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://ym.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ex.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vw.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cq.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ll.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mm.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ay.wgjwhj.cn

[K07] 进制转换
来源：http://bk.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oc.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gk.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jp.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://io.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bm.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sr.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wk.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cn.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://ih.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ec.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://mi.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://zv.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xz.jctech888.com.cn

Go:   encoding/gob
来源：http://uf.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://mb.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xu.jianghongdianzi.cn

================================================================================
来源：http://ba.newstarts.cn

L. 网络请求
来源：http://he.wgjwhj.cn

================================================================================
来源：http://nf.panjiajie.cn

[L01] 发送 GET 请求
来源：http://iz.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ly.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ui.asd995.cn

JS:   await fetch(url)
来源：http://hd.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://lx.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://en.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://nh.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cz.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ra.shxzskj.cn

[L02] 发送 POST JSON
来源：http://jz.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ov.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zu.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kk.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mc.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cl.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lz.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lu.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ss.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://fy.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://un.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ux.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ih.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qd.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hw.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://li.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mo.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cg.521024.cn

[L04] 设置超时
来源：http://tx.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://gg.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wh.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cg.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cx.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kw.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qh.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uz.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mh.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ji.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://va.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rk.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hb.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ew.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://im.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mj.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gx.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://km.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ax.colortex.cn


<!-- 参考信息 -->