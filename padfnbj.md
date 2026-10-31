代发 wailian999

================================================================================
来源：http://mr.gzmigu.cn

I. 正则表达式
来源：http://eu.asd995.cn

================================================================================
来源：http://zi.hnjuh.cn

[I01] 判断是否匹配
来源：http://lo.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bm.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://im.nicolike.cn

JS:   /\d+/.test(s)
来源：http://el.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://da.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yr.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jh.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://vi.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mr.panjiajie.cn

[I02] 提取所有匹配
来源：http://rq.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://nv.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cd.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jr.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://pu.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ed.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gb.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ci.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mk.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://pj.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eg.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zx.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dr.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qv.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bs.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pc.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lg.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lz.asd995.cn

[I04] 正则替换
来源：http://kf.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tx.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kq.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mb.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ay.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ee.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lz.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iy.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pb.hnjuh.cn

[I05] 按正则拆分
来源：http://na.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dk.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lo.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://xh.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://er.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://gj.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://la.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ms.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pv.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yt.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fi.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ln.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uv.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vr.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ox.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://se.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bj.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://op.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://yw.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vn.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zx.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cn.huanxung.cn

TS:   /error/gim
来源：http://qf.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://he.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gt.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://tf.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://va.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://lx.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sh.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wl.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ox.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ea.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vy.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ny.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dx.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rl.yuntaijiaju.cn

================================================================================
来源：http://py.jianghongdianzi.cn

J. 日期与时间
来源：http://mx.panjiajie.cn

================================================================================
来源：http://kj.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://of.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lp.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ue.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://up.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://ea.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gy.huixinmuqiang.cn

Go:   time.Now()
来源：http://gi.huixiangedu.cn

Ruby: Time.now
来源：http://le.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kh.shxzukj.cn

[J02] 格式化输出
来源：http://ud.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ha.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ml.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mc.yuexingan06.cn

TS:   d.toISOString()
来源：http://tr.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ss.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://af.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tu.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uf.nszjky.cn

[J03] 字符串解析为日期
来源：http://gs.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ey.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qd.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://pb.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://nd.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wc.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ff.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://wn.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ch.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://xp.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ca.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ee.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sz.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://br.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ky.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dg.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ar.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nj.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://nw.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://fo.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ms.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ct.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://md.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://vq.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bv.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://jl.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ty.wgjwhj.cn

[J06] 计算两时间之差
来源：http://ry.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://nb.521024.cn

PHP:  $end->diff($start)->days;
来源：http://bf.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jy.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ob.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xn.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://jo.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://dg.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://kl.jctech888.com.cn

[J07] 比较两个日期
来源：http://bj.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://dd.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qk.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qd.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qa.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sy.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fp.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eb.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://mv.521024.cn

[J08] 提取年月日与星期
来源：http://cd.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://of.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sg.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cd.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ai.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cg.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gv.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tb.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yl.wgjwhj.cn

[J09] 时区处理
来源：http://qt.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pe.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iq.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zy.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wd.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wf.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uw.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ba.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wu.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://yu.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wv.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ab.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wt.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pa.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vb.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ve.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pq.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qv.chemitech.net.cn

================================================================================
来源：http://zp.haigaiapp.cn

K. JSON 与序列化
来源：http://kn.nicolike.cn

================================================================================
来源：http://dn.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://im.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lm.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jk.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ix.asd995.cn

TS:   JSON.stringify(obj)
来源：http://jt.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yx.9csxet.cn

Go:   json.Marshal(obj)
来源：http://qm.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uw.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ow.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ot.chemitech.net.cn

Py:   json.loads(s)
来源：http://kq.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zy.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://oc.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://ln.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gz.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://pq.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://dp.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ls.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://ai.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nm.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dn.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yj.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gb.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ov.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qa.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xs.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ge.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://tl.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mx.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tp.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rp.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yr.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mv.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ck.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://za.haigaiapp.cn

[K05] 深拷贝对象
来源：http://ph.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://rv.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://jb.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://ml.colortex.cn

TS:   structuredClone(obj)
来源：http://ox.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qi.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zy.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ro.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iw.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://wi.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rr.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ie.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vl.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sg.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://od.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://it.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fl.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wz.muxihuayi.cn

[K07] 进制转换
来源：http://vo.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ue.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ku.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wx.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dc.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jk.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zy.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nk.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gm.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://xf.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://vc.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sh.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://oj.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://te.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zw.muxihuayi.cn

Go:   encoding/gob
来源：http://ij.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://bw.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nx.haigaiapp.cn

================================================================================
来源：http://fn.bjjhwx.cn

L. 网络请求
来源：http://se.hahajie.cn

================================================================================
来源：http://jp.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://pl.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://px.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vy.chemitech.net.cn

JS:   await fetch(url)
来源：http://nk.panjiajie.cn

TS:   await fetch(url)
来源：http://tc.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wx.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://jh.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://el.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yn.huanxung.cn

[L02] 发送 POST JSON
来源：http://na.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nr.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fx.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ip.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jk.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qm.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ew.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ax.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yu.szsharing.cn

[L03] 设置自定义请求头
来源：http://hx.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xg.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xj.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://he.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cw.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://md.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gp.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tg.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fp.huixiangedu.cn

[L04] 设置超时
来源：http://dz.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://hh.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ul.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vi.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wi.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ow.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dy.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://so.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://re.huanxung.cn

[L05] 上传文件（multipart）
来源：http://im.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qp.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://il.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pv.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lq.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ji.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://me.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://tm.shtwfgs.cn

Py:   resp.json()
来源：http://ug.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://vz.huixiangedu.cn

JS:   await resp.json()
来源：http://di.huanxung.cn

TS:   await resp.json()
来源：http://yo.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jj.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ri.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://dw.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tz.9csxet.cn


<!-- 参考信息 -->