代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uy.bjjhwx.cn

[I03] 提取捕获分组
来源：http://qn.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ba.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kt.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ah.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://va.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qg.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nr.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://os.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://me.bjjhwx.cn

[I04] 正则替换
来源：http://gp.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hb.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cr.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xq.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qk.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://md.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nx.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tc.gzmigu.cn

[I05] 按正则拆分
来源：http://fd.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ws.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ig.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://hu.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://lo.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://nx.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ps.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ls.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dh.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ej.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ij.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jp.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cp.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rp.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pu.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://co.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://fq.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zi.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vm.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pa.shxzukj.cn

TS:   /error/gim
来源：http://ch.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tp.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tf.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://do.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rm.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://to.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ln.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://is.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ru.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rj.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uq.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ez.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pn.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://my.nszjky.cn

J. 日期与时间
来源：http://rr.521024.cn

================================================================================
来源：http://rt.jctech888.com.cn

[J01] 获取当前时间
来源：http://bl.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lz.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qz.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://xx.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://yj.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wl.hnjuh.cn

Go:   time.Now()
来源：http://xx.huixiangedu.cn

Ruby: Time.now
来源：http://ch.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bw.hnjuh.cn

[J02] 格式化输出
来源：http://mm.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fg.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pr.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qz.wgjwhj.cn

TS:   d.toISOString()
来源：http://ni.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xo.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wv.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iv.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ix.lnxyls.cn

[J03] 字符串解析为日期
来源：http://is.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pf.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xw.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://rn.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://nu.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ab.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dd.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://aw.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wa.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://fe.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uz.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zh.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://je.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ld.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jq.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hl.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sf.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gq.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://hv.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://kf.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tg.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bs.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mh.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ue.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ca.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://hj.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sq.newstarts.cn

[J06] 计算两时间之差
来源：http://rb.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://fp.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ea.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lc.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uc.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://au.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://wi.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://mi.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://hd.bookmarksfly.cn

[J07] 比较两个日期
来源：http://qv.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://nf.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zo.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bv.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vn.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oi.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ws.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://os.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://uw.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://uj.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kn.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://of.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ji.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bj.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wb.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zb.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://an.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sq.haigaiapp.cn

[J09] 时区处理
来源：http://xv.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://di.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ba.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uc.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ej.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://in.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://et.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ue.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://os.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uu.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hl.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ol.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wp.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sz.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wr.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lg.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xp.szsharing.cn

================================================================================
来源：http://zv.521024.cn

K. JSON 与序列化
来源：http://yb.shxzukj.cn

================================================================================
来源：http://zf.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://bp.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qh.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gf.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://fe.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://da.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zs.hahajie.cn

Go:   json.Marshal(obj)
来源：http://hb.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dc.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://ye.bjjhwx.cn

Py:   json.loads(s)
来源：http://ob.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ny.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://ut.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://sh.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vj.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://li.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://rk.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xn.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://xw.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://po.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yn.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rx.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jm.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zp.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bu.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qs.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ue.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://wz.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fz.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ji.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oa.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kr.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gs.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sb.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://bm.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://pp.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://mz.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://fn.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ro.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mf.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tm.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ot.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ue.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://bz.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dn.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ps.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ui.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zi.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://da.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xd.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ue.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://km.gzmigu.cn

[K07] 进制转换
来源：http://wj.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mw.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yg.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yw.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hw.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wc.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uk.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wh.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://la.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://fh.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://nm.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vc.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://pm.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://rn.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mv.shxzskj.cn

Go:   encoding/gob
来源：http://vh.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://bz.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://it.9csxet.cn

================================================================================
来源：http://wc.panjiajie.cn

L. 网络请求
来源：http://he.szxytkj.cn

================================================================================
来源：http://kz.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://mx.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jk.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dp.szsharing.cn

JS:   await fetch(url)
来源：http://gy.chemitech.net.cn

TS:   await fetch(url)
来源：http://zv.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sx.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://lp.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pw.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zs.521024.cn

[L02] 发送 POST JSON
来源：http://lm.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fl.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dq.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oa.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oz.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qc.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hx.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ht.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qo.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://qu.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ew.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hh.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jq.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fa.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cg.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tr.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qc.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lf.huixiangedu.cn

[L04] 设置超时
来源：http://xn.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://jk.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mc.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fi.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wt.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fp.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oz.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ru.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oq.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://zj.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pw.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cu.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uf.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ac.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pg.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ju.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qr.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ko.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ln.newstarts.cn

Py:   resp.json()
来源：http://fw.asd995.cn

PHP:  json_decode($body, true);
来源：http://gz.colortex.cn

JS:   await resp.json()
来源：http://js.panjiajie.cn

TS:   await resp.json()
来源：http://rt.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nc.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vq.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://bi.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qy.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://lw.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yn.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tr.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://lb.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://fn.gzmigu.cn

Java: resp.statusCode()
来源：http://ts.szsharing.cn

Go:   resp.StatusCode
来源：http://np.shxzukj.cn

Ruby: resp.code.to_i
来源：http://pv.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://rr.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://lm.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eg.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ak.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gg.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oh.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mz.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ks.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ao.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xy.jianghongdianzi.cn

================================================================================
来源：http://je.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://wu.gzmigu.cn


<!-- 参考信息 -->