代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mu.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tb.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://sh.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bp.haigaiapp.cn

[I02] 提取所有匹配
来源：http://zl.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://mx.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sf.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dd.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://av.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cb.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://va.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://je.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ht.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://rv.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ov.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dv.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kb.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oa.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ww.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rm.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rb.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ez.huixiangedu.cn

[I04] 正则替换
来源：http://eb.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eu.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kf.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yo.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://od.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ip.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fh.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jf.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ak.nicolike.cn

[I05] 按正则拆分
来源：http://kc.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://od.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uy.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://sq.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://yg.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://tm.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sq.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vb.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tl.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kt.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cj.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bg.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://op.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vs.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ei.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gc.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bx.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pu.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://xx.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eh.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ag.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hx.yuexingan06.cn

TS:   /error/gim
来源：http://ud.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ix.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rp.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://qc.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gf.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://sm.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gd.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xv.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cb.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mj.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rb.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kh.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://os.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dt.haigaiapp.cn

================================================================================
来源：http://ad.9csxet.cn

J. 日期与时间
来源：http://wx.nicolike.cn

================================================================================
来源：http://lw.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://or.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mg.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://to.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://lb.hahajie.cn

TS:   new Date();  Date.now()
来源：http://ca.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kj.hahajie.cn

Go:   time.Now()
来源：http://xc.hahajie.cn

Ruby: Time.now
来源：http://oh.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.szsharing.cn

[J02] 格式化输出
来源：http://cv.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jn.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mi.shxzskj.cn

TS:   d.toISOString()
来源：http://nh.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://em.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mb.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yc.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jw.hnjuh.cn

[J03] 字符串解析为日期
来源：http://xk.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tl.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lv.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://fn.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://gn.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vw.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jv.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ws.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bv.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://ez.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lf.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wr.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eu.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ro.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eh.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bm.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nw.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jf.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ux.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://gw.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kn.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zi.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ok.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://pz.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qf.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://hs.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://re.chemitech.net.cn

[J06] 计算两时间之差
来源：http://vn.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://uc.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://vd.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cz.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pp.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ue.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://fb.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ci.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://tk.chemitech.net.cn

[J07] 比较两个日期
来源：http://zc.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://qh.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gu.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tg.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pr.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://di.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xq.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aa.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://bd.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://am.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iy.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xc.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ew.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ij.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yw.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pr.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nv.hnjuh.cn

[J09] 时区处理
来源：http://xt.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fy.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fz.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cz.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wy.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ch.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zu.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cw.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ib.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ap.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eu.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gw.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vq.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://og.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uo.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bf.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wl.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uk.521024.cn

================================================================================
来源：http://ab.muxihuayi.cn

K. JSON 与序列化
来源：http://pf.colortex.cn

================================================================================
来源：http://fm.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://qw.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mf.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dl.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://dx.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://qy.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pj.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://qy.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fr.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xi.hahajie.cn

[K02] JSON 字符串转对象
来源：http://eh.huixiangedu.cn

Py:   json.loads(s)
来源：http://zr.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wr.nicolike.cn

JS:   JSON.parse(s)
来源：http://yi.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://ps.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pp.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ny.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://pe.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jl.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ul.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nv.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ys.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gv.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mv.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zh.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qc.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mk.szsharing.cn

[K04] 读取 JSON 文件
来源：http://ke.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dr.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zm.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bk.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xo.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yk.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://df.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xm.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iq.haigaiapp.cn

[K05] 深拷贝对象
来源：http://fq.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://op.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://fy.shxzukj.cn

JS:   structuredClone(obj)
来源：http://pc.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://qs.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ws.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ap.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gb.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://li.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://kv.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oe.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fd.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dw.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nk.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tq.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bw.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kw.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ak.yuexingan06.cn

[K07] 进制转换
来源：http://zk.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ee.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uh.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kt.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wb.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ad.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lg.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rd.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ny.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://pe.521024.cn

Py:   pickle.dumps(obj)
来源：http://fj.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bz.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mk.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://je.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pc.shtwfgs.cn

Go:   encoding/gob
来源：http://xq.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://jc.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yf.shxzskj.cn

================================================================================
来源：http://xr.wgjwhj.cn

L. 网络请求
来源：http://jf.shtwfgs.cn

================================================================================
来源：http://hd.nszjky.cn

[L01] 发送 GET 请求
来源：http://ry.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://re.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://te.521024.cn

JS:   await fetch(url)
来源：http://ny.gzmigu.cn

TS:   await fetch(url)
来源：http://rz.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://td.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://nn.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qp.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ts.szxytkj.cn

[L02] 发送 POST JSON
来源：http://ju.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ws.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ym.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://st.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pp.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lf.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ea.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rk.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ml.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://im.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ur.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ic.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ms.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lt.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uq.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://is.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ke.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xe.hnjuh.cn

[L04] 设置超时
来源：http://tp.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://bl.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yh.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zh.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fl.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qe.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fz.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nk.9csxet.cn

[L05] 上传文件（multipart）
来源：http://xk.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ds.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mx.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nu.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://we.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://po.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sj.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wt.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dz.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://sw.9csxet.cn

Py:   resp.json()
来源：http://lm.9csxet.cn

PHP:  json_decode($body, true);
来源：http://gn.lnxyls.cn

JS:   await resp.json()
来源：http://jy.521024.cn

TS:   await resp.json()
来源：http://kf.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ru.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wc.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://xo.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qa.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://be.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qc.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cl.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://wg.521024.cn

TS:   resp.ok;  resp.status
来源：http://yt.bookmarksfly.cn

Java: resp.statusCode()
来源：http://os.shxzukj.cn

Go:   resp.StatusCode
来源：http://on.asd995.cn

Ruby: resp.code.to_i
来源：http://sw.asd995.cn


<!-- 参考信息 -->