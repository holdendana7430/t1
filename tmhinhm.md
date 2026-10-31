代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://an.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://is.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nx.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dr.jctech888.com.cn

================================================================================
来源：http://uv.521024.cn

I. 正则表达式
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://wl.hnjuh.cn

[I01] 判断是否匹配
来源：http://av.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zz.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xp.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://tr.asd995.cn

TS:   /\d+/.test(s)
来源：http://dz.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ie.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://mm.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sg.hnjuh.cn

[I02] 提取所有匹配
来源：http://vk.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://ml.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mt.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://de.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://zq.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ki.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tt.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://nb.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ed.521024.cn

[I03] 提取捕获分组
来源：http://nv.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ug.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sq.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cq.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tt.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gc.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jr.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pw.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mj.hnjuh.cn

[I04] 正则替换
来源：http://hp.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qj.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nz.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pa.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hn.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wy.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lh.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xd.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cl.yuexingan06.cn

[I05] 按正则拆分
来源：http://ca.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yl.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aj.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://mv.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://ej.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://wa.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xp.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xp.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dw.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jx.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gi.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cj.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sc.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pf.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bl.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rw.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xw.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pl.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://di.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qq.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hk.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://go.huixiangedu.cn

TS:   /error/gim
来源：http://nr.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mz.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://up.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ne.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jo.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://hv.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oy.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ur.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jn.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aj.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ex.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tp.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rh.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kr.521024.cn

================================================================================
来源：http://ev.newstarts.cn

J. 日期与时间
来源：http://ac.panjiajie.cn

================================================================================
来源：http://cv.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://er.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ru.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ql.newstarts.cn

JS:   new Date();  Date.now()
来源：http://fc.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ex.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pq.shxzskj.cn

Go:   time.Now()
来源：http://tu.shxzskj.cn

Ruby: Time.now
来源：http://on.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://si.huixiangedu.cn

[J02] 格式化输出
来源：http://ge.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wx.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uv.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://px.colortex.cn

TS:   d.toISOString()
来源：http://vm.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iy.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tl.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wx.nicolike.cn

[J03] 字符串解析为日期
来源：http://va.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tp.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cu.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://rp.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://we.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ml.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yw.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://dr.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iz.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://go.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ms.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://je.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fc.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://px.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rx.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://md.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yl.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://af.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://kv.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://ly.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tq.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cj.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bz.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://mk.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ct.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://vh.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nc.szsharing.cn

[J06] 计算两时间之差
来源：http://ka.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://rw.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://vp.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xu.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://do.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://je.521024.cn

Go:   end.Sub(start).Hours()
来源：http://xo.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://lx.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://db.huixiangedu.cn

[J07] 比较两个日期
来源：http://kw.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://be.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nc.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uk.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bn.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nw.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ql.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ig.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://du.panjiajie.cn

[J08] 提取年月日与星期
来源：http://kx.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://if.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cy.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qt.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ng.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yt.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://is.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ys.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ud.newstarts.cn

[J09] 时区处理
来源：http://hq.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nv.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zq.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zc.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wy.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cy.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ra.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ja.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ov.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://nl.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fh.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iz.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kp.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zd.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gh.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ew.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qm.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gh.huixiangedu.cn

================================================================================
来源：http://qr.colortex.cn

K. JSON 与序列化
来源：http://ym.jianghongdianzi.cn

================================================================================
来源：http://do.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://kp.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://il.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cj.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ic.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://mw.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bl.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://om.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uc.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wz.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://rb.panjiajie.cn

Py:   json.loads(s)
来源：http://zq.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ji.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://mh.szsharing.cn

TS:   JSON.parse(s)
来源：http://cn.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ni.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://pl.newstarts.cn

Ruby: JSON.parse(s)
来源：http://pa.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hx.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://tn.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oi.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cu.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wl.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aj.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cu.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://po.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zm.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gx.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ze.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oq.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ph.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dz.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uj.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cs.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yp.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://df.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ln.huanxung.cn

[K05] 深拷贝对象
来源：http://lg.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://dg.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://yq.huanxung.cn

JS:   structuredClone(obj)
来源：http://zp.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://bu.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jj.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mt.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dp.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zu.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://ae.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wx.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ar.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rj.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nq.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nj.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hs.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rz.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jr.colortex.cn

[K07] 进制转换
来源：http://mc.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ei.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ws.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zd.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ss.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://df.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tn.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ck.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fa.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://oh.asd995.cn

Py:   pickle.dumps(obj)
来源：http://fg.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lc.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://um.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://zu.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fn.bookmarksfly.cn

Go:   encoding/gob
来源：http://hw.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://bc.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zk.shxzukj.cn

================================================================================
来源：http://fq.shtwfgs.cn

L. 网络请求
来源：http://cn.shxzukj.cn

================================================================================
来源：http://dv.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://yt.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://we.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tr.gzmigu.cn

JS:   await fetch(url)
来源：http://av.gzmigu.cn

TS:   await fetch(url)
来源：http://ra.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cq.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://lw.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://og.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xa.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ox.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://df.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kx.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vx.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xm.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qq.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qm.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oc.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oe.shxzukj.cn

[L03] 设置自定义请求头
来源：http://re.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nl.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vo.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pi.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dq.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://la.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wy.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jb.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xy.jctech888.com.cn

[L04] 设置超时
来源：http://pp.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://xc.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ub.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ts.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://in.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zn.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vv.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wn.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gv.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://im.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zg.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://km.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cb.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oq.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pu.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ke.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://av.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rf.shxzskj.cn

Py:   resp.json()
来源：http://kx.nszjky.cn

PHP:  json_decode($body, true);
来源：http://hy.nszjky.cn

JS:   await resp.json()
来源：http://hx.lnxyls.cn

TS:   await resp.json()
来源：http://ct.asd995.cn


<!-- 参考信息 -->