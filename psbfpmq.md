代发 wailian999

================================================================================
来源：http://ue.jctech888.com.cn

I. 正则表达式
来源：http://bv.szsharing.cn

================================================================================
来源：http://ma.colortex.cn

[I01] 判断是否匹配
来源：http://dw.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cs.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ec.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://dm.asd995.cn

TS:   /\d+/.test(s)
来源：http://hl.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://me.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ys.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://fn.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nf.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://nz.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://bd.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bx.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xk.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://xc.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rd.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mf.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://vh.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ki.hnjuh.cn

[I03] 提取捕获分组
来源：http://px.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pq.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lq.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ni.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vc.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pa.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eo.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gb.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oz.panjiajie.cn

[I04] 正则替换
来源：http://rx.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sk.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qs.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xr.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ah.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mv.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dk.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jk.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ow.shxzukj.cn

[I05] 按正则拆分
来源：http://yl.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ll.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ud.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://oh.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://bx.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ye.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rh.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ox.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vq.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fw.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gk.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gj.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://to.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wi.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eq.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rh.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ee.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://kh.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qt.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://os.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qd.panjiajie.cn

TS:   /error/gim
来源：http://sr.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xn.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jx.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://ec.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ze.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://cr.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hm.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://je.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xc.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rj.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xy.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fv.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://py.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aw.yuexingan06.cn

================================================================================
来源：http://wv.shxzukj.cn

J. 日期与时间
来源：http://sw.521024.cn

================================================================================
来源：http://xc.jctech888.com.cn

[J01] 获取当前时间
来源：http://we.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dm.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cm.nicolike.cn

JS:   new Date();  Date.now()
来源：http://rf.szsharing.cn

TS:   new Date();  Date.now()
来源：http://bv.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vz.nszjky.cn

Go:   time.Now()
来源：http://ty.gzmigu.cn

Ruby: Time.now
来源：http://vb.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pg.newstarts.cn

[J02] 格式化输出
来源：http://ju.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pv.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xr.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eu.haigaiapp.cn

TS:   d.toISOString()
来源：http://ci.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rp.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rk.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lj.gzmigu.cn

[J03] 字符串解析为日期
来源：http://mw.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uc.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ke.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://ux.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://eu.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mb.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vm.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://wo.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qf.521024.cn

[J04] 时间戳与日期互转
来源：http://of.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ki.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://am.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hy.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mr.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lp.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://el.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sk.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vk.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://jq.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://vq.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lt.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ok.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ar.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://sy.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uj.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://ff.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vh.lnxyls.cn

[J06] 计算两时间之差
来源：http://se.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://fc.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ny.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zl.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xh.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tw.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://oi.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://pb.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://bc.hahajie.cn

[J07] 比较两个日期
来源：http://en.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ii.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wi.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dq.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gh.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dg.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wk.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ei.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://fi.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://rl.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ws.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://es.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fl.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lq.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://in.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bn.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uu.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eq.szxytkj.cn

[J09] 时区处理
来源：http://hz.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zw.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lm.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zt.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bp.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vm.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gb.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jc.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://av.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cl.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tq.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ea.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yt.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zs.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nq.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://db.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rc.huixinmuqiang.cn

================================================================================
来源：http://mw.521024.cn

K. JSON 与序列化
来源：http://le.newstarts.cn

================================================================================
来源：http://xd.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://dy.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bf.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yv.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://po.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://xx.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tw.521024.cn

Go:   json.Marshal(obj)
来源：http://rg.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dj.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jr.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://dt.shxzukj.cn

Py:   json.loads(s)
来源：http://ro.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zw.huanxung.cn

JS:   JSON.parse(s)
来源：http://pn.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://cd.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://am.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://jf.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://kf.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://is.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://zd.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://si.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ob.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oy.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rg.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ij.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qt.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://qs.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lx.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://id.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ms.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yd.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cg.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://km.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pz.panjiajie.cn

[K05] 深拷贝对象
来源：http://wq.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://lt.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://sd.colortex.cn

JS:   structuredClone(obj)
来源：http://eo.gzmigu.cn

TS:   structuredClone(obj)
来源：http://jk.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qv.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pn.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://id.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vn.nicolike.cn

[K06] 解析 URL 查询串
来源：http://qp.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tc.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oa.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sg.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mu.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gh.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oq.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vh.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fs.colortex.cn

[K07] 进制转换
来源：http://ps.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ub.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ll.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://on.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://el.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qt.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ft.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kh.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fk.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://gp.colortex.cn

Py:   pickle.dumps(obj)
来源：http://cg.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jj.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://xy.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://ra.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zh.nszjky.cn

Go:   encoding/gob
来源：http://lc.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://xw.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zz.jianghongdianzi.cn

================================================================================
来源：http://il.shtwfgs.cn

L. 网络请求
来源：http://so.shtwfgs.cn

================================================================================
来源：http://tk.colortex.cn

[L01] 发送 GET 请求
来源：http://ql.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sb.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vz.521024.cn

JS:   await fetch(url)
来源：http://mv.bjjhwx.cn

TS:   await fetch(url)
来源：http://hj.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mn.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://ab.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://la.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kh.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://is.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hy.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uf.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://je.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wx.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ir.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wb.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jt.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wc.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://eo.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rr.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jd.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tn.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cr.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mv.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ai.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sn.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kh.jianghongdianzi.cn

[L04] 设置超时
来源：http://rd.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://dt.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ln.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vq.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wl.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bq.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://on.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ej.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ar.huanxung.cn

[L05] 上传文件（multipart）
来源：http://wb.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qe.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gf.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hy.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lj.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://os.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://um.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pl.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ef.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://zh.yuntaijiaju.cn

Py:   resp.json()
来源：http://au.colortex.cn

PHP:  json_decode($body, true);
来源：http://nn.colortex.cn

JS:   await resp.json()
来源：http://jd.asd995.cn

TS:   await resp.json()
来源：http://lo.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zr.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qs.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://zm.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wo.wgjwhj.cn


<!-- 参考信息 -->