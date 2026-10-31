代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nr.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uz.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ko.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xv.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tn.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cg.huixinmuqiang.cn

[I04] 正则替换
来源：http://am.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wj.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ec.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ft.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rj.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sh.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sc.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qh.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pd.szxytkj.cn

[I05] 按正则拆分
来源：http://dt.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qt.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://br.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://fv.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://fi.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://zm.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wz.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://la.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://el.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mj.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fe.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jc.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://by.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ts.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ym.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rs.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pt.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nw.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://st.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bw.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qs.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wp.haigaiapp.cn

TS:   /error/gim
来源：http://ea.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ub.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ap.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://iu.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sc.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ic.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tu.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mx.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zk.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lk.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ky.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nm.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://el.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ug.yuexingan06.cn

================================================================================
来源：http://uu.jctech888.com.cn

J. 日期与时间
来源：http://gs.yuexingan06.cn

================================================================================
来源：http://zm.jctech888.com.cn

[J01] 获取当前时间
来源：http://rr.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zm.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zo.nszjky.cn

JS:   new Date();  Date.now()
来源：http://iv.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://hb.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mw.muxihuayi.cn

Go:   time.Now()
来源：http://ju.wgjwhj.cn

Ruby: Time.now
来源：http://zc.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zr.shxzukj.cn

[J02] 格式化输出
来源：http://qk.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cm.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vy.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fp.9csxet.cn

TS:   d.toISOString()
来源：http://lx.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rf.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zd.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fl.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://ec.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rb.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wp.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://pt.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://rg.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mb.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wi.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://lj.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rc.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://jr.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wl.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gb.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://go.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wr.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jf.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gv.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kn.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wo.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://qx.521024.cn

Py:   now + timedelta(days=7)
来源：http://kl.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://au.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ru.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wc.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://bi.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wu.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://bq.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tj.521024.cn

[J06] 计算两时间之差
来源：http://sc.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://zx.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://jw.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sb.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wo.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://te.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://bn.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://xt.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ny.muxihuayi.cn

[J07] 比较两个日期
来源：http://oe.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://gv.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mw.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hu.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mu.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mt.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yx.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rp.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://mn.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://zi.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://re.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jv.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eu.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yw.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dy.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tk.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cq.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ej.shxzskj.cn

[J09] 时区处理
来源：http://rz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ta.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://li.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mm.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hk.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mm.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kj.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hb.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zq.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://lw.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tn.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xu.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yl.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://po.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ep.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bm.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zc.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ih.yuexingan06.cn

================================================================================
来源：http://jc.szsharing.cn

K. JSON 与序列化
来源：http://hb.huixinmuqiang.cn

================================================================================
来源：http://ks.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://xd.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fd.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dx.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ze.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://am.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yp.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://wx.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hq.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mb.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://pj.nicolike.cn

Py:   json.loads(s)
来源：http://ie.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fb.newstarts.cn

JS:   JSON.parse(s)
来源：http://ts.shxzukj.cn

TS:   JSON.parse(s)
来源：http://ti.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qn.9csxet.cn

Ruby: JSON.parse(s)
来源：http://om.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mq.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://cx.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xc.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vu.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xc.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tm.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://et.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wm.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tv.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ep.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ia.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://in.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tu.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://if.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gl.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ok.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gd.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kf.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kn.nszjky.cn

[K05] 深拷贝对象
来源：http://nz.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://ip.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://sy.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://da.lnxyls.cn

TS:   structuredClone(obj)
来源：http://fe.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rt.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zt.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bd.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ru.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://xq.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://za.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jx.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zb.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cq.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aw.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ar.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eq.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pz.shxzukj.cn

[K07] 进制转换
来源：http://rn.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hh.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yh.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bb.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ex.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qy.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nc.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rq.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ui.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ox.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://ud.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cn.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ms.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://lg.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ev.shxzukj.cn

Go:   encoding/gob
来源：http://bm.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://fo.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ts.muxihuayi.cn

================================================================================
来源：http://an.hnjuh.cn

L. 网络请求
来源：http://tw.hahajie.cn

================================================================================
来源：http://cu.gzmigu.cn

[L01] 发送 GET 请求
来源：http://gw.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ru.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kq.shxzukj.cn

JS:   await fetch(url)
来源：http://iz.hahajie.cn

TS:   await fetch(url)
来源：http://dl.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pg.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ea.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cs.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wx.shxzskj.cn

[L02] 发送 POST JSON
来源：http://hf.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ip.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ys.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://py.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kc.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ak.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wj.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kh.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ku.newstarts.cn

[L03] 设置自定义请求头
来源：http://bt.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ux.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hb.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ki.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ua.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zz.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gr.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cv.muxihuayi.cn

[L04] 设置超时
来源：http://zi.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://uz.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fw.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zj.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ew.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ym.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://os.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kf.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ky.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://mr.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tv.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oq.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kr.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vs.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ry.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wk.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ll.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://do.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://yp.yuexingan06.cn

Py:   resp.json()
来源：http://as.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://pk.bjjhwx.cn

JS:   await resp.json()
来源：http://zd.jctech888.com.cn

TS:   await resp.json()
来源：http://kc.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ag.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wq.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://am.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gv.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://qa.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jx.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hs.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://qp.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://ll.bjjhwx.cn

Java: resp.statusCode()
来源：http://fq.shxzukj.cn

Go:   resp.StatusCode
来源：http://za.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ws.colortex.cn

C#:   (int)resp.StatusCode
来源：http://iq.hnjuh.cn

[L08] 并发请求多个地址
来源：http://lw.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kc.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://cp.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jk.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qh.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tk.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qq.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sd.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fx.szsharing.cn

================================================================================
来源：http://ny.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://ln.szxytkj.cn

================================================================================
来源：http://ie.521024.cn

[M01] 读取命令行参数
来源：http://cw.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://zi.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://gn.gzmigu.cn


<!-- 参考信息 -->