代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ot.bjjhwx.cn

[I03] 提取捕获分组
来源：http://wa.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fb.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lz.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ud.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pc.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ss.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oe.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hu.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bz.jianghongdianzi.cn

[I04] 正则替换
来源：http://uj.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vl.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wk.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pn.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hr.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kp.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kp.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rj.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wn.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://ku.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fo.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ov.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://hv.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rf.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://va.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ei.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ws.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oc.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lm.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://as.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iu.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://an.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mm.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bs.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ec.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ar.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://hx.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ew.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xt.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sh.hnjuh.cn

TS:   /error/gim
来源：http://ja.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kq.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ju.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://lg.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tq.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://bo.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ud.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kz.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lb.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nh.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ef.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://un.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bt.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gi.asd995.cn

================================================================================
来源：http://jc.bjjhwx.cn

J. 日期与时间
来源：http://rn.521024.cn

================================================================================
来源：http://vj.bjjhwx.cn

[J01] 获取当前时间
来源：http://hg.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vp.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://os.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://jw.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://fa.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ii.hahajie.cn

Go:   time.Now()
来源：http://st.bookmarksfly.cn

Ruby: Time.now
来源：http://xl.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wl.bjjhwx.cn

[J02] 格式化输出
来源：http://su.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pk.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ed.lnxyls.cn

TS:   d.toISOString()
来源：http://xf.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aq.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ei.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vm.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jv.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://of.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uy.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ep.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://zg.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://vf.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sk.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wl.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ur.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://py.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://fa.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kg.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qn.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bc.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://co.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kh.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yz.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gu.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qm.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://mq.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://of.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://td.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ro.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cq.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://cc.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fy.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://bl.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jv.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ok.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://sl.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://gc.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oz.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xf.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iv.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://qm.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://gj.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ay.chemitech.net.cn

[J07] 比较两个日期
来源：http://qs.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://tl.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oc.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qi.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pk.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nv.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rm.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ic.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://va.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://si.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://le.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://na.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rk.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bm.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pc.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zp.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gu.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rj.newstarts.cn

[J09] 时区处理
来源：http://by.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qd.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://va.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qt.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dm.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nf.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gl.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qu.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://li.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://tq.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gq.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xh.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lp.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dy.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nf.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://td.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zr.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qv.yuntaijiaju.cn

================================================================================
来源：http://mn.huanxung.cn

K. JSON 与序列化
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://rz.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://bl.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eh.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qq.521024.cn

JS:   JSON.stringify(obj)
来源：http://po.asd995.cn

TS:   JSON.stringify(obj)
来源：http://vi.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pc.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://vx.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ge.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://do.nszjky.cn

[K02] JSON 字符串转对象
来源：http://kp.bjjhwx.cn

Py:   json.loads(s)
来源：http://xh.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dg.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://rv.hahajie.cn

TS:   JSON.parse(s)
来源：http://jc.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vk.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://zp.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://os.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bz.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://tg.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bh.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sr.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yv.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ml.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vv.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dl.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ts.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xl.huanxung.cn

[K04] 读取 JSON 文件
来源：http://xz.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dw.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bw.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ad.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ob.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ws.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vn.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sg.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zs.shtwfgs.cn

[K05] 深拷贝对象
来源：http://vj.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://zn.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://yj.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://gu.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://fs.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vu.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ie.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cq.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xa.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ug.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ml.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pe.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dk.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ts.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qs.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ud.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://td.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zn.huixinmuqiang.cn

[K07] 进制转换
来源：http://xd.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wt.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bb.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mf.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kb.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gj.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pm.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tx.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gb.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://vp.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://as.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lb.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://wx.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://jt.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qb.nszjky.cn

Go:   encoding/gob
来源：http://on.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://hk.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ac.nszjky.cn

================================================================================
来源：http://vi.nicolike.cn

L. 网络请求
来源：http://ev.hnjuh.cn

================================================================================
来源：http://qu.szsharing.cn

[L01] 发送 GET 请求
来源：http://lx.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ue.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.bookmarksfly.cn

JS:   await fetch(url)
来源：http://dy.shtwfgs.cn

TS:   await fetch(url)
来源：http://qd.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jj.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://wy.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mx.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ev.lnxyls.cn

[L02] 发送 POST JSON
来源：http://fz.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sl.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://em.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nm.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lf.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ad.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://on.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ip.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://go.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://ss.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mj.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zv.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://it.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://be.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lw.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nj.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wv.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qv.lnxyls.cn

[L04] 设置超时
来源：http://vn.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://pa.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nq.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lm.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kb.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uy.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yr.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://du.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://or.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://cz.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dk.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sw.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wz.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kp.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fu.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vh.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mn.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sy.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://nc.shtwfgs.cn

Py:   resp.json()
来源：http://nk.nszjky.cn

PHP:  json_decode($body, true);
来源：http://hq.hahajie.cn

JS:   await resp.json()
来源：http://cp.yuexingan06.cn

TS:   await resp.json()
来源：http://op.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ec.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mt.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://rt.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tw.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://cv.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pc.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fr.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://dz.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://bg.huixiangedu.cn

Java: resp.statusCode()
来源：http://ln.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://ab.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://ak.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://ak.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://jg.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tw.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://ut.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gh.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sa.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ry.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ss.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pj.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cl.shtwfgs.cn

================================================================================
来源：http://ud.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://nk.panjiajie.cn


<!-- 参考信息 -->