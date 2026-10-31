代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qq.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://te.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zt.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bz.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bb.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ru.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pn.chemitech.net.cn

[I05] 按正则拆分
来源：http://ra.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bm.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lz.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://qr.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ss.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://wp.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hv.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gv.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aa.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vh.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zf.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yx.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ce.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xy.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jo.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wl.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yp.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hr.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://qh.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nw.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xb.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ph.bjjhwx.cn

TS:   /error/gim
来源：http://hf.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nx.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jk.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://wy.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jz.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ld.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://he.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eu.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ip.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xm.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bi.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xw.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ok.huixiangedu.cn

================================================================================
来源：http://es.9csxet.cn

J. 日期与时间
来源：http://kg.hahajie.cn

================================================================================
来源：http://rw.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://mu.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ck.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sq.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://qc.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://yj.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tu.colortex.cn

Go:   time.Now()
来源：http://ii.521024.cn

Ruby: Time.now
来源：http://wq.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mm.newstarts.cn

[J02] 格式化输出
来源：http://dz.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uu.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ez.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vm.haigaiapp.cn

TS:   d.toISOString()
来源：http://vi.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://py.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ef.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yr.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xx.lnxyls.cn

[J03] 字符串解析为日期
来源：http://ca.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gg.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jh.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://uc.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://sg.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://va.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://li.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://xj.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mw.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://bg.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qo.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mr.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rw.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xa.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://um.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://no.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://jt.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yy.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oa.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tu.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://rt.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://qx.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jw.jctech888.com.cn

[J06] 计算两时间之差
来源：http://gf.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://bo.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://gj.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aw.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rb.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gf.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://gu.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://mu.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://ee.szxytkj.cn

[J07] 比较两个日期
来源：http://sn.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yw.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oy.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gm.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://un.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wp.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vv.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://it.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://dc.szsharing.cn

[J08] 提取年月日与星期
来源：http://ab.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ul.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://my.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bt.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fa.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cn.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pp.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cl.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bu.newstarts.cn

[J09] 时区处理
来源：http://ws.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ye.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wo.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ug.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fb.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rx.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zh.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qg.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nr.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://py.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vz.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rz.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xb.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ln.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kx.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mp.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hq.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wi.wgjwhj.cn

================================================================================
来源：http://kh.huanxung.cn

K. JSON 与序列化
来源：http://ai.szsharing.cn

================================================================================
来源：http://ik.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://jf.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sm.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dg.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://cm.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://iw.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qb.hahajie.cn

Go:   json.Marshal(obj)
来源：http://go.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hl.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kv.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://lb.haigaiapp.cn

Py:   json.loads(s)
来源：http://xn.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rp.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://uv.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://wj.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://vk.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://vg.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dd.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ax.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yh.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fb.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ch.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tl.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://te.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eh.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ks.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yv.hahajie.cn

[K04] 读取 JSON 文件
来源：http://bs.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zo.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wu.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eh.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://py.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ni.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xl.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xr.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zn.muxihuayi.cn

[K05] 深拷贝对象
来源：http://cu.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://at.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://qm.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://yb.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://my.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gr.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gj.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lc.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ru.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://zw.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xa.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qf.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dq.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ur.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fs.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ap.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qz.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://it.shxzskj.cn

[K07] 进制转换
来源：http://zv.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://og.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bz.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gt.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://je.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lh.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nf.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://om.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iq.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://xg.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://yj.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eo.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://wp.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ts.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ld.newstarts.cn

Go:   encoding/gob
来源：http://qg.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ao.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vn.nszjky.cn

================================================================================
来源：http://ae.jianghongdianzi.cn

L. 网络请求
来源：http://ef.9csxet.cn

================================================================================
来源：http://th.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ir.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wj.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xk.shxzukj.cn

JS:   await fetch(url)
来源：http://wq.lnxyls.cn

TS:   await fetch(url)
来源：http://jl.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ot.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ud.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yy.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wk.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ya.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tm.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ba.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yc.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xl.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nh.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xo.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ua.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rg.521024.cn

[L03] 设置自定义请求头
来源：http://rl.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://av.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bg.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kk.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://to.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ay.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ar.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ic.nszjky.cn

[L04] 设置超时
来源：http://jq.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://eo.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ws.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://au.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://if.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tt.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mt.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nv.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mx.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://jy.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://km.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kv.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pg.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mi.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pl.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dg.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fm.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cq.newstarts.cn

[L06] 解析响应为 JSON
来源：http://zw.521024.cn

Py:   resp.json()
来源：http://vr.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://vd.9csxet.cn

JS:   await resp.json()
来源：http://sx.huanxung.cn

TS:   await resp.json()
来源：http://oq.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jj.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ao.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://km.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sp.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://rc.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mu.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uf.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://lj.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://gh.bookmarksfly.cn

Java: resp.statusCode()
来源：http://hu.newstarts.cn

Go:   resp.StatusCode
来源：http://ur.shxzukj.cn

Ruby: resp.code.to_i
来源：http://na.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://qg.lnxyls.cn

[L08] 并发请求多个地址
来源：http://fv.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vm.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://av.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nm.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zb.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://th.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xw.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://an.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fd.muxihuayi.cn

================================================================================
来源：http://uj.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://fx.huixinmuqiang.cn

================================================================================
来源：http://bd.newstarts.cn

[M01] 读取命令行参数
来源：http://ud.shxzskj.cn

Py:   sys.argv[1:]
来源：http://mw.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://fr.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://bo.nszjky.cn

TS:   process.argv.slice(2)
来源：http://fg.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://jl.lnxyls.cn

Go:   os.Args[1:]
来源：http://dk.bookmarksfly.cn

Ruby: ARGV
来源：http://zv.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://ut.colortex.cn

[M02] 读取环境变量
来源：http://tg.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://qg.panjiajie.cn


<!-- 参考信息 -->