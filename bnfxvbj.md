代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://td.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iv.9csxet.cn

[I04] 正则替换
来源：http://oj.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lh.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sp.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ka.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dq.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ec.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://df.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://il.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jr.hahajie.cn

[I05] 按正则拆分
来源：http://ii.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ft.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fo.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://pq.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://qk.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://yi.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ek.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ux.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kb.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ux.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jq.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ix.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ds.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wr.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rf.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bj.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://of.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bc.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://ol.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tu.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tz.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qj.bjjhwx.cn

TS:   /error/gim
来源：http://pu.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nd.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xy.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://hw.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vp.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://tw.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ha.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dz.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vd.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://np.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zh.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://me.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://az.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oa.hahajie.cn

================================================================================
来源：http://oa.shxzskj.cn

J. 日期与时间
来源：http://ay.shxzskj.cn

================================================================================
来源：http://ne.newstarts.cn

[J01] 获取当前时间
来源：http://ds.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ci.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xf.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://wc.asd995.cn

TS:   new Date();  Date.now()
来源：http://an.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://so.shxzskj.cn

Go:   time.Now()
来源：http://qo.jianghongdianzi.cn

Ruby: Time.now
来源：http://yy.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pa.jianghongdianzi.cn

[J02] 格式化输出
来源：http://al.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jv.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sq.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ct.yuexingan06.cn

TS:   d.toISOString()
来源：http://yi.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dd.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qi.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bh.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xa.shxzskj.cn

[J03] 字符串解析为日期
来源：http://xr.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nd.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jc.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://me.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://kg.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kv.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rc.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://pz.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://or.nicolike.cn

[J04] 时间戳与日期互转
来源：http://jy.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mf.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tf.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mn.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xr.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://za.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sq.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lp.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yn.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://nm.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://tj.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nb.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wz.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ob.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://mf.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ro.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://uq.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ke.panjiajie.cn

[J06] 计算两时间之差
来源：http://rp.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://ob.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://cy.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lo.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://if.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gu.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://ia.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://js.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://wx.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ks.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://uh.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gg.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://db.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kc.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vo.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dp.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ur.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://kq.panjiajie.cn

[J08] 提取年月日与星期
来源：http://sq.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ac.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rc.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://og.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wt.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lp.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hk.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ak.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ph.chemitech.net.cn

[J09] 时区处理
来源：http://bq.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kd.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ua.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ed.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tz.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://te.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ft.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://do.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xj.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://lf.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dk.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xk.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zb.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sb.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bi.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lh.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rm.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vj.yuntaijiaju.cn

================================================================================
来源：http://af.huixinmuqiang.cn

K. JSON 与序列化
来源：http://jq.nszjky.cn

================================================================================
来源：http://dm.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://wy.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tg.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://uk.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://oq.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ih.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://th.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aj.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ka.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://mp.bjjhwx.cn

Py:   json.loads(s)
来源：http://mt.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ik.nicolike.cn

JS:   JSON.parse(s)
来源：http://ug.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://tr.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ha.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://gn.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://iu.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://du.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://nh.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ps.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://he.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dv.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tp.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://na.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gk.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pd.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ar.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://vm.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pk.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mg.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kq.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nr.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mq.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dc.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wf.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ej.521024.cn

[K05] 深拷贝对象
来源：http://tj.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://xr.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://sd.hnjuh.cn

JS:   structuredClone(obj)
来源：http://wk.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://oy.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lz.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hl.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gl.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jh.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://zx.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qi.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ja.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pw.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ck.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://an.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cd.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hq.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zn.chemitech.net.cn

[K07] 进制转换
来源：http://yl.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qx.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fp.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jd.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ci.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xf.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uc.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cc.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qw.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://tz.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ch.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nn.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://fk.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://te.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fd.shxzskj.cn

Go:   encoding/gob
来源：http://fg.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://jc.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://em.huanxung.cn

================================================================================
来源：http://ta.shtwfgs.cn

L. 网络请求
来源：http://zw.newstarts.cn

================================================================================
来源：http://vw.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://pk.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qv.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iz.szxytkj.cn

JS:   await fetch(url)
来源：http://jn.szxytkj.cn

TS:   await fetch(url)
来源：http://kd.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ip.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://kj.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tn.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://es.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://st.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zn.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ai.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kx.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mx.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sk.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hf.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gq.9csxet.cn

[L03] 设置自定义请求头
来源：http://ps.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gd.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ei.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xg.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pk.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pg.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gw.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ub.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gd.asd995.cn

[L04] 设置超时
来源：http://uq.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://zs.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pv.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sr.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xd.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xu.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://la.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fc.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wi.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://fn.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ln.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fs.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tm.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://io.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ax.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vr.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hb.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://di.521024.cn

[L06] 解析响应为 JSON
来源：http://bn.huanxung.cn

Py:   resp.json()
来源：http://ek.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://vf.newstarts.cn

JS:   await resp.json()
来源：http://zh.szsharing.cn

TS:   await resp.json()
来源：http://dn.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ca.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dc.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://ep.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sb.521024.cn

[L07] 处理 HTTP 状态码
来源：http://tu.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ot.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://dm.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://ut.jctech888.com.cn

Java: resp.statusCode()
来源：http://xt.gzmigu.cn

Go:   resp.StatusCode
来源：http://dg.9csxet.cn

Ruby: resp.code.to_i
来源：http://oi.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://vd.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://ej.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ys.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://wr.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xm.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pi.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vt.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sq.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://as.bookmarksfly.cn

================================================================================
来源：http://pu.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://oe.hahajie.cn

================================================================================
来源：http://fx.shxzukj.cn

[M01] 读取命令行参数
来源：http://ut.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://rt.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://gp.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://jc.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://nc.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ff.wgjwhj.cn

Go:   os.Args[1:]
来源：http://hp.szsharing.cn


<!-- 参考信息 -->