代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pl.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://et.shtwfgs.cn

[I04] 正则替换
来源：http://va.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ki.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qi.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yl.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ic.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rc.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ba.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ll.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zm.newstarts.cn

[I05] 按正则拆分
来源：http://fi.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hc.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ip.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://bn.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://qs.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://aw.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ps.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ea.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yb.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sn.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fd.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pi.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pt.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yz.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://my.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jy.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://br.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tq.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://sy.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ks.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jz.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xf.shxzskj.cn

TS:   /error/gim
来源：http://tm.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wj.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ex.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://ga.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fl.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://xh.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ju.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gp.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vu.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fa.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dn.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qp.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vm.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mc.huixinmuqiang.cn

================================================================================
来源：http://ll.gzmigu.cn

J. 日期与时间
来源：http://ee.shtwfgs.cn

================================================================================
来源：http://vk.chemitech.net.cn

[J01] 获取当前时间
来源：http://ie.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://am.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fw.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ku.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://bl.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://me.nicolike.cn

Go:   time.Now()
来源：http://dg.chemitech.net.cn

Ruby: Time.now
来源：http://vg.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qv.nszjky.cn

[J02] 格式化输出
来源：http://qw.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mf.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wf.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cy.hahajie.cn

TS:   d.toISOString()
来源：http://rs.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mv.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hn.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zw.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ul.nicolike.cn

[J03] 字符串解析为日期
来源：http://bt.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oi.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yr.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://df.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://zw.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jw.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nv.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://zb.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fg.huanxung.cn

[J04] 时间戳与日期互转
来源：http://lj.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eh.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://li.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gh.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rm.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mw.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gq.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bh.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sf.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://li.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://ja.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zs.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kx.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://xs.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sl.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://bw.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wt.shxzukj.cn

[J06] 计算两时间之差
来源：http://oa.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://xm.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://ol.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eb.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gq.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://df.521024.cn

Go:   end.Sub(start).Hours()
来源：http://lp.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://hp.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://jd.lnxyls.cn

[J07] 比较两个日期
来源：http://iq.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://po.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qo.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pb.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fh.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jl.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://np.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lx.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://do.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://zh.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bm.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qi.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lf.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://as.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://en.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qx.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://su.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gv.wgjwhj.cn

[J09] 时区处理
来源：http://ue.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ni.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sv.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://my.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ju.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hc.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ae.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sn.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tc.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://nl.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ge.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bj.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sh.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nb.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sm.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ze.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vm.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hr.shxzukj.cn

================================================================================
来源：http://mz.9csxet.cn

K. JSON 与序列化
来源：http://ce.panjiajie.cn

================================================================================
来源：http://sy.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://ad.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dx.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zh.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://wp.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://kh.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xr.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://am.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ts.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iy.9csxet.cn

[K02] JSON 字符串转对象
来源：http://ju.szxytkj.cn

Py:   json.loads(s)
来源：http://pm.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wp.hnjuh.cn

JS:   JSON.parse(s)
来源：http://bv.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://rt.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pj.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://fz.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://fq.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bd.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://lr.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://os.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://se.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ja.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nd.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nu.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hl.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ux.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sd.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://il.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://me.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sf.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gf.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yj.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sp.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://io.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xr.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gw.szxytkj.cn

[K05] 深拷贝对象
来源：http://fh.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://jq.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://ox.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://ji.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://hm.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://az.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ds.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fb.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://de.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://wg.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rr.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zh.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mu.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cv.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ls.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kn.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mu.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hm.yuexingan06.cn

[K07] 进制转换
来源：http://dd.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uf.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ll.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ks.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://up.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hg.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pj.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nu.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ep.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://fd.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://wg.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oa.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fv.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://qp.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sg.shxzukj.cn

Go:   encoding/gob
来源：http://bl.521024.cn

Ruby: Marshal.dump(obj)
来源：http://id.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pw.bjjhwx.cn

================================================================================
来源：http://bw.nicolike.cn

L. 网络请求
来源：http://dw.jctech888.com.cn

================================================================================
来源：http://hf.szsharing.cn

[L01] 发送 GET 请求
来源：http://jx.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cc.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://my.muxihuayi.cn

JS:   await fetch(url)
来源：http://gg.huanxung.cn

TS:   await fetch(url)
来源：http://pz.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xv.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ba.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://li.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vf.newstarts.cn

[L02] 发送 POST JSON
来源：http://bf.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qz.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gl.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xi.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rh.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hl.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jk.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uz.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vv.panjiajie.cn

[L03] 设置自定义请求头
来源：http://fm.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://df.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zh.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ie.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wv.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tl.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yf.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zd.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qa.huanxung.cn

[L04] 设置超时
来源：http://ng.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://kc.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://op.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://al.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lm.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://it.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ly.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://od.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dp.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ue.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rz.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://an.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gz.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wj.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fc.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rs.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xl.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://nw.bookmarksfly.cn

Py:   resp.json()
来源：http://fs.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://xs.nicolike.cn

JS:   await resp.json()
来源：http://wd.bookmarksfly.cn

TS:   await resp.json()
来源：http://zz.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gc.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dt.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://vl.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ol.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://bd.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nq.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eb.colortex.cn

JS:   resp.ok;  resp.status
来源：http://jm.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://mj.shxzukj.cn

Java: resp.statusCode()
来源：http://eq.jctech888.com.cn

Go:   resp.StatusCode
来源：http://go.shxzukj.cn

Ruby: resp.code.to_i
来源：http://hk.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://oq.521024.cn

[L08] 并发请求多个地址
来源：http://se.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ev.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://rh.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rf.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wi.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mq.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zc.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gr.bookmarksfly.cn

================================================================================
来源：http://iq.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://bq.nszjky.cn

================================================================================
来源：http://pw.chemitech.net.cn

[M01] 读取命令行参数
来源：http://wo.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://sp.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ex.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://ra.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://mw.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://as.nicolike.cn

Go:   os.Args[1:]
来源：http://wg.shxzukj.cn


<!-- 参考信息 -->