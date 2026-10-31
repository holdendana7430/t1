代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dx.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ah.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zg.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ip.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://of.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cc.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ef.bjjhwx.cn

[I05] 按正则拆分
来源：http://ua.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rl.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dx.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ge.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://cd.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://mn.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yx.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lg.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tu.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hc.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fq.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ek.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hk.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ps.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hv.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gi.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://du.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://dm.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://if.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fa.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qd.gzmigu.cn

TS:   /error/gim
来源：http://vd.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ay.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bk.521024.cn

Ruby: s.scan(/error/i)
来源：http://bt.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ni.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://zv.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tb.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fb.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://so.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hb.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://di.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ss.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yx.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vv.bookmarksfly.cn

================================================================================
来源：http://kl.szxytkj.cn

J. 日期与时间
来源：http://qx.nicolike.cn

================================================================================
来源：http://jy.nicolike.cn

[J01] 获取当前时间
来源：http://yn.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wd.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ar.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ci.nszjky.cn

TS:   new Date();  Date.now()
来源：http://qt.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://en.shxzskj.cn

Go:   time.Now()
来源：http://zd.szsharing.cn

Ruby: Time.now
来源：http://zq.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ad.huixiangedu.cn

[J02] 格式化输出
来源：http://zd.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kt.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gu.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wx.lnxyls.cn

TS:   d.toISOString()
来源：http://cn.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jv.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hl.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ga.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sa.panjiajie.cn

[J03] 字符串解析为日期
来源：http://gf.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gt.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pi.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://je.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://fg.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rf.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bn.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://jp.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sh.szsharing.cn

[J04] 时间戳与日期互转
来源：http://mi.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jc.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ix.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iy.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qz.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://go.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jr.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wb.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ni.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://ki.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ke.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aj.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ez.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bq.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://kk.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://df.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://di.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qu.shtwfgs.cn

[J06] 计算两时间之差
来源：http://vw.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://mj.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://zm.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qm.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://go.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rz.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://sj.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://ih.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://vh.muxihuayi.cn

[J07] 比较两个日期
来源：http://qr.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://eu.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://by.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rg.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wq.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ca.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sr.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iv.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://bg.asd995.cn

[J08] 提取年月日与星期
来源：http://nx.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xw.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lz.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://id.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ty.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kx.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ph.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xo.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://im.jctech888.com.cn

[J09] 时区处理
来源：http://lv.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aa.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fv.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pb.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cr.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wz.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cy.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nl.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://ld.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aa.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ly.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ew.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cz.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ly.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rk.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zs.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lr.521024.cn

================================================================================
来源：http://bt.nszjky.cn

K. JSON 与序列化
来源：http://ju.huixinmuqiang.cn

================================================================================
来源：http://gx.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://gf.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fd.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ls.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://kp.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://jp.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tv.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://vh.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uo.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mk.colortex.cn

[K02] JSON 字符串转对象
来源：http://an.szsharing.cn

Py:   json.loads(s)
来源：http://fa.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cd.szxytkj.cn

JS:   JSON.parse(s)
来源：http://tp.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://us.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rx.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://el.9csxet.cn

Ruby: JSON.parse(s)
来源：http://io.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uo.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ax.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vc.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ee.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zx.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hh.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wo.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ll.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://be.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yk.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://lo.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hk.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pa.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ti.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wk.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ob.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jd.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sj.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fq.chemitech.net.cn

[K05] 深拷贝对象
来源：http://ew.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://ju.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://jo.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://ue.shxzskj.cn

TS:   structuredClone(obj)
来源：http://az.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xz.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fo.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hf.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hk.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://fa.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wm.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ww.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ks.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://da.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://io.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vq.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://su.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ge.huixiangedu.cn

[K07] 进制转换
来源：http://rc.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mi.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pw.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bo.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://za.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cj.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iy.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pl.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://me.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://nx.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://rr.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qz.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://hz.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://fv.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kl.lnxyls.cn

Go:   encoding/gob
来源：http://bf.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ac.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kg.lnxyls.cn

================================================================================
来源：http://un.muxihuayi.cn

L. 网络请求
来源：http://cz.shxzukj.cn

================================================================================
来源：http://fr.colortex.cn

[L01] 发送 GET 请求
来源：http://dr.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://op.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ky.shxzukj.cn

JS:   await fetch(url)
来源：http://fg.chemitech.net.cn

TS:   await fetch(url)
来源：http://ud.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uc.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://km.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uf.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ep.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://up.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tg.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://in.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ss.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yx.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sl.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wx.9csxet.cn

[L03] 设置自定义请求头
来源：http://hp.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://md.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yu.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ji.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mw.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sj.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wx.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ck.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://av.haigaiapp.cn

[L04] 设置超时
来源：http://fn.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://xi.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fs.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ae.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vc.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bb.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eo.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nu.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ge.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://um.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ji.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hl.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xq.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zg.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jo.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kp.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pk.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ac.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://sx.jianghongdianzi.cn

Py:   resp.json()
来源：http://mh.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://ig.nicolike.cn

JS:   await resp.json()
来源：http://zv.yuexingan06.cn

TS:   await resp.json()
来源：http://ee.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fj.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ql.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://za.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yn.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://ts.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qu.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yz.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://gg.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ni.huixiangedu.cn

Java: resp.statusCode()
来源：http://zd.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://dp.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://pw.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://du.szxytkj.cn

[L08] 并发请求多个地址
来源：http://wz.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dw.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://cq.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mn.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cw.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://px.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ls.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mq.bjjhwx.cn

================================================================================
来源：http://ba.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://mi.shtwfgs.cn

================================================================================
来源：http://lq.szsharing.cn

[M01] 读取命令行参数
来源：http://zi.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://ly.hahajie.cn

PHP:  $argv;  $argc;
来源：http://rp.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://td.nicolike.cn

TS:   process.argv.slice(2)
来源：http://sw.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://sm.shxzukj.cn

Go:   os.Args[1:]
来源：http://gs.nszjky.cn

Ruby: ARGV
来源：http://yw.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://kj.yuexingan06.cn

[M02] 读取环境变量
来源：http://ms.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://xh.bjjhwx.cn


<!-- 参考信息 -->