代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://na.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vr.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://uq.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pj.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://tv.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://qm.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gr.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wz.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://tj.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lm.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jr.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://tq.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fx.hahajie.cn

[I03] 提取捕获分组
来源：http://qg.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ke.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://au.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lo.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://if.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pe.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ua.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yz.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mc.huixinmuqiang.cn

[I04] 正则替换
来源：http://ex.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vb.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ml.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cr.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zy.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rx.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qt.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qr.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pb.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://ev.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ll.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wh.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://zy.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://yt.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ed.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zf.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://az.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mm.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xe.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kk.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ru.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lk.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hb.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jz.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cn.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pv.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://vg.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fv.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rr.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wn.jctech888.com.cn

TS:   /error/gim
来源：http://hb.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sb.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ze.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://te.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wc.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://rr.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ab.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qg.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vz.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oj.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tk.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zx.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gu.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lm.yuexingan06.cn

================================================================================
来源：http://um.muxihuayi.cn

J. 日期与时间
来源：http://oo.newstarts.cn

================================================================================
来源：http://rw.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://au.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fi.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xl.nszjky.cn

JS:   new Date();  Date.now()
来源：http://pr.hahajie.cn

TS:   new Date();  Date.now()
来源：http://gn.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qq.nicolike.cn

Go:   time.Now()
来源：http://ny.szxytkj.cn

Ruby: Time.now
来源：http://uo.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mq.huixinmuqiang.cn

[J02] 格式化输出
来源：http://sy.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bo.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sn.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pb.chemitech.net.cn

TS:   d.toISOString()
来源：http://gj.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mu.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://li.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ed.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ko.shxzskj.cn

[J03] 字符串解析为日期
来源：http://og.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lk.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qy.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://hg.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ov.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vs.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://so.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://hk.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mr.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://jq.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pl.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ow.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mr.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fc.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dv.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oq.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zq.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ri.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://tc.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://gw.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bn.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qb.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wo.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://vb.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mx.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://na.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://je.shtwfgs.cn

[J06] 计算两时间之差
来源：http://in.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://ai.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ek.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jl.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nv.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bp.521024.cn

Go:   end.Sub(start).Hours()
来源：http://su.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://ss.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://la.bjjhwx.cn

[J07] 比较两个日期
来源：http://mp.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://zn.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jo.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mr.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rm.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ke.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hn.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ht.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://uk.lnxyls.cn

[J08] 提取年月日与星期
来源：http://fe.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ob.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ts.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wu.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mz.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ea.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jg.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tj.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gl.yuexingan06.cn

[J09] 时区处理
来源：http://cu.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dh.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iu.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ex.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cl.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fw.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://il.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ht.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zy.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://mq.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lm.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mg.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eo.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kp.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zw.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rq.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://an.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://to.chemitech.net.cn

================================================================================
来源：http://zn.szxytkj.cn

K. JSON 与序列化
来源：http://de.shtwfgs.cn

================================================================================
来源：http://dq.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://dn.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nn.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wk.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://wr.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://th.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lj.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://xn.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vh.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vl.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ow.szsharing.cn

Py:   json.loads(s)
来源：http://me.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jm.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ft.lnxyls.cn

TS:   JSON.parse(s)
来源：http://lu.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ml.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://bt.nszjky.cn

Ruby: JSON.parse(s)
来源：http://xr.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pp.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xi.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uf.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kq.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wx.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xr.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jk.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dx.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tw.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gi.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://qe.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ee.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dw.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fr.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xd.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hs.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://la.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ko.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ep.panjiajie.cn

[K05] 深拷贝对象
来源：http://mk.521024.cn

Py:   copy.deepcopy(obj)
来源：http://wj.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://js.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://we.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://oy.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hp.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://be.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xu.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sp.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://wa.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ur.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hn.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://da.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vp.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ot.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://za.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gp.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gw.chemitech.net.cn

[K07] 进制转换
来源：http://wb.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qm.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://an.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nl.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pw.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lk.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://il.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yj.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rh.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://kb.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://js.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ts.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://hj.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://vy.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ez.jctech888.com.cn

Go:   encoding/gob
来源：http://ac.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://wv.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fh.newstarts.cn

================================================================================
来源：http://pt.newstarts.cn

L. 网络请求
来源：http://ev.huixiangedu.cn

================================================================================
来源：http://nj.9csxet.cn

[L01] 发送 GET 请求
来源：http://sj.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kc.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cq.panjiajie.cn

JS:   await fetch(url)
来源：http://no.jctech888.com.cn

TS:   await fetch(url)
来源：http://kc.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pu.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://wv.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gm.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fp.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://fk.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gf.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vp.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xx.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cj.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nq.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yg.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xs.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bq.panjiajie.cn

[L03] 设置自定义请求头
来源：http://an.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hu.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kt.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bx.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yd.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ed.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pa.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nz.wgjwhj.cn

[L04] 设置超时
来源：http://uk.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://oz.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tm.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://go.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eb.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nj.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gi.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rl.nicolike.cn

[L05] 上传文件（multipart）
来源：http://fq.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xy.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pg.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zp.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ah.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fk.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sx.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jz.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aa.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ek.9csxet.cn

Py:   resp.json()
来源：http://lw.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ak.shxzukj.cn

JS:   await resp.json()
来源：http://rb.hahajie.cn

TS:   await resp.json()
来源：http://ha.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qx.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kz.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://lq.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zz.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://an.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pk.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ra.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://me.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://ou.muxihuayi.cn

Java: resp.statusCode()
来源：http://fk.asd995.cn

Go:   resp.StatusCode
来源：http://gy.9csxet.cn

Ruby: resp.code.to_i
来源：http://er.shtwfgs.cn


<!-- 参考信息 -->