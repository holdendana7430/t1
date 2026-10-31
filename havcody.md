代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dk.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ut.hahajie.cn

[I04] 正则替换
来源：http://nx.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zm.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rp.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lh.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xu.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sv.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://la.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sw.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gg.bookmarksfly.cn

[I05] 按正则拆分
来源：http://as.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xe.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pl.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://ao.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://vo.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://eg.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fp.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nn.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bz.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cn.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sc.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vl.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tl.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jq.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ze.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kh.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nk.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rc.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://nk.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://to.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bs.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jl.shtwfgs.cn

TS:   /error/gim
来源：http://xm.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uj.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ry.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://el.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sj.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ec.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dc.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cv.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wa.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cp.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://do.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ek.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mt.newstarts.cn

================================================================================
来源：http://zt.huixinmuqiang.cn

J. 日期与时间
来源：http://fa.chemitech.net.cn

================================================================================
来源：http://oz.bjjhwx.cn

[J01] 获取当前时间
来源：http://vq.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://du.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dm.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://ks.colortex.cn

TS:   new Date();  Date.now()
来源：http://sw.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ln.colortex.cn

Go:   time.Now()
来源：http://gj.wgjwhj.cn

Ruby: Time.now
来源：http://yy.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ln.chemitech.net.cn

[J02] 格式化输出
来源：http://ci.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ys.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://um.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pf.huixiangedu.cn

TS:   d.toISOString()
来源：http://xk.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uy.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://js.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cq.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wq.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://cf.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ag.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ad.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://yf.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://mj.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zh.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://uc.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sn.newstarts.cn

[J04] 时间戳与日期互转
来源：http://zx.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ph.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hp.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fl.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xd.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sg.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fa.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hq.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yz.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://my.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://mt.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gr.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xy.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://og.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ds.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pp.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://mx.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ld.panjiajie.cn

[J06] 计算两时间之差
来源：http://vd.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://ri.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://eh.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jj.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ok.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gb.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://dx.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://tn.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://mr.shxzukj.cn

[J07] 比较两个日期
来源：http://hk.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qv.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jj.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://me.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xm.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xg.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nl.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gb.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://pg.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://xh.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hq.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rl.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jt.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://im.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aq.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ca.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ay.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://if.jianghongdianzi.cn

[J09] 时区处理
来源：http://ef.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://co.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jr.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jg.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bu.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kb.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rl.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pg.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hk.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://wa.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lb.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hx.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jz.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xh.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nv.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xi.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ol.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ff.521024.cn

================================================================================
来源：http://ju.szxytkj.cn

K. JSON 与序列化
来源：http://ze.jianghongdianzi.cn

================================================================================
来源：http://kg.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://pv.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eb.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://va.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://kd.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://pf.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zm.521024.cn

Go:   json.Marshal(obj)
来源：http://nf.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zu.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uk.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://dq.shtwfgs.cn

Py:   json.loads(s)
来源：http://om.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xb.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://hj.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://bv.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hm.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://li.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://up.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cs.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://qw.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ko.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ur.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zs.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hw.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://op.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uz.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kh.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xi.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://zg.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://si.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xw.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ek.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ll.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wd.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ie.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wr.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ey.gzmigu.cn

[K05] 深拷贝对象
来源：http://ko.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://mh.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://yl.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://kd.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://en.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hq.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tj.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bo.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lc.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://az.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://db.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tk.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yy.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ti.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://li.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sp.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cj.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xd.szxytkj.cn

[K07] 进制转换
来源：http://sn.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://df.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wp.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cc.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://on.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jw.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oc.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xn.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pq.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://wl.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://xp.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://md.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://bg.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://hl.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://in.yuexingan06.cn

Go:   encoding/gob
来源：http://jf.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://bt.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rt.gzmigu.cn

================================================================================
来源：http://hi.huixiangedu.cn

L. 网络请求
来源：http://rz.gzmigu.cn

================================================================================
来源：http://sp.gzmigu.cn

[L01] 发送 GET 请求
来源：http://vd.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yq.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pl.panjiajie.cn

JS:   await fetch(url)
来源：http://sh.lnxyls.cn

TS:   await fetch(url)
来源：http://rl.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uz.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://wo.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vs.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cu.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ch.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zi.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zl.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://na.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fd.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ka.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yv.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cb.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ng.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://qd.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qd.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ht.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://we.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jf.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xc.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ui.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ob.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ff.hahajie.cn

[L04] 设置超时
来源：http://zj.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://nm.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xa.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bj.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zu.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mm.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xy.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ps.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tf.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://zl.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sn.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qe.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yy.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mq.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xs.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qa.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pn.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mx.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://he.muxihuayi.cn

Py:   resp.json()
来源：http://my.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://gl.newstarts.cn

JS:   await resp.json()
来源：http://rw.shxzskj.cn

TS:   await resp.json()
来源：http://au.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lc.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xb.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://lr.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kn.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://xx.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gd.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ia.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://np.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://dp.hnjuh.cn

Java: resp.statusCode()
来源：http://wq.hnjuh.cn

Go:   resp.StatusCode
来源：http://bs.huanxung.cn

Ruby: resp.code.to_i
来源：http://ub.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://br.newstarts.cn

[L08] 并发请求多个地址
来源：http://si.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zf.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ku.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kj.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qk.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vx.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gp.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jr.huixinmuqiang.cn

================================================================================
来源：http://xc.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://tw.shxzukj.cn

================================================================================
来源：http://pw.panjiajie.cn

[M01] 读取命令行参数
来源：http://ep.colortex.cn

Py:   sys.argv[1:]
来源：http://hj.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://dk.newstarts.cn

JS:   process.argv.slice(2)
来源：http://pc.nicolike.cn

TS:   process.argv.slice(2)
来源：http://pg.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://ya.panjiajie.cn

Go:   os.Args[1:]
来源：http://yb.hahajie.cn


<!-- 参考信息 -->