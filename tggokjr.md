代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hf.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hc.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gt.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://up.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ht.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wx.szxytkj.cn

[I04] 正则替换
来源：http://sz.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fm.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ho.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dg.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jz.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://we.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ce.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sc.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pw.muxihuayi.cn

[I05] 按正则拆分
来源：http://px.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fy.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pc.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://qt.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://dy.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://gi.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://et.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ta.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yc.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jz.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xc.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pn.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lp.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pe.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dj.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ez.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jj.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lw.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://ss.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ln.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lc.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vd.hnjuh.cn

TS:   /error/gim
来源：http://fu.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ei.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qa.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://rc.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://az.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ex.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://os.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wx.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pp.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://de.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xt.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nj.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fk.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bb.szsharing.cn

================================================================================
来源：http://ht.shxzskj.cn

J. 日期与时间
来源：http://po.haigaiapp.cn

================================================================================
来源：http://ov.szxytkj.cn

[J01] 获取当前时间
来源：http://im.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kq.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://so.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://se.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://kd.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cb.shxzskj.cn

Go:   time.Now()
来源：http://me.jianghongdianzi.cn

Ruby: Time.now
来源：http://gx.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vs.hnjuh.cn

[J02] 格式化输出
来源：http://cc.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ki.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fp.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://op.huixiangedu.cn

TS:   d.toISOString()
来源：http://uc.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ws.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vq.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sb.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gr.lnxyls.cn

[J03] 字符串解析为日期
来源：http://jq.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fa.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mn.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://xo.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://mm.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yp.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cr.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://au.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lx.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ra.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ud.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pd.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ue.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lg.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cf.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vx.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qz.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nl.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://gs.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://gw.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mv.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vk.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://na.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://qk.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bl.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://mb.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://po.panjiajie.cn

[J06] 计算两时间之差
来源：http://fb.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://jm.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://rs.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pv.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ch.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nf.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://lc.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://vg.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://pn.gzmigu.cn

[J07] 比较两个日期
来源：http://gv.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ao.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vd.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yu.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sh.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ut.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pj.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tc.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://er.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://vn.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ah.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yq.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tx.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://if.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mx.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wg.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ki.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cg.huixiangedu.cn

[J09] 时区处理
来源：http://ee.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dt.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ly.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fh.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rk.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ek.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://as.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ty.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gp.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://pk.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uy.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ko.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://or.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hd.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ue.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qj.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mi.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qi.szsharing.cn

================================================================================
来源：http://ai.panjiajie.cn

K. JSON 与序列化
来源：http://np.jctech888.com.cn

================================================================================
来源：http://wd.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://kf.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gg.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qt.colortex.cn

JS:   JSON.stringify(obj)
来源：http://db.colortex.cn

TS:   JSON.stringify(obj)
来源：http://bq.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://df.nicolike.cn

Go:   json.Marshal(obj)
来源：http://qe.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gj.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eg.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://oh.muxihuayi.cn

Py:   json.loads(s)
来源：http://zw.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nn.panjiajie.cn

JS:   JSON.parse(s)
来源：http://fy.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://ad.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vd.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://kv.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://ne.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ch.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://td.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://df.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kv.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://my.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hn.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wh.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nx.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zs.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sp.szsharing.cn

[K04] 读取 JSON 文件
来源：http://hn.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ou.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vr.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cj.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://te.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qb.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kk.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vs.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mk.gzmigu.cn

[K05] 深拷贝对象
来源：http://mr.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://gd.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://yf.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://na.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://ro.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ae.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ep.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xm.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rd.szsharing.cn

[K06] 解析 URL 查询串
来源：http://fi.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ew.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zt.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oz.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dh.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cm.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gb.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mr.9csxet.cn

[K07] 进制转换
来源：http://je.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pw.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vh.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rw.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zx.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qx.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ub.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cv.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uv.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://sd.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://lv.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lq.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://vt.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://zv.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rn.yuexingan06.cn

Go:   encoding/gob
来源：http://rz.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://rm.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fy.521024.cn

================================================================================
来源：http://mt.newstarts.cn

L. 网络请求
来源：http://ez.521024.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://dz.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oa.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jg.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ku.bjjhwx.cn

TS:   await fetch(url)
来源：http://tk.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fq.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://fi.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fu.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ds.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://zj.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ah.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qs.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fs.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ld.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gi.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pr.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oy.shxzskj.cn

[L03] 设置自定义请求头
来源：http://gy.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hb.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ay.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ke.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ts.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aj.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ih.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yo.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ve.haigaiapp.cn

[L04] 设置超时
来源：http://xx.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://mp.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uw.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gn.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pq.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ku.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ve.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kq.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ou.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://te.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ap.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ck.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mv.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ng.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ef.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zi.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rc.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ld.muxihuayi.cn

Py:   resp.json()
来源：http://jc.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://tq.wgjwhj.cn

JS:   await resp.json()
来源：http://fb.nszjky.cn

TS:   await resp.json()
来源：http://md.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ne.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ra.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://qh.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bg.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://cn.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ep.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xz.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://nl.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://it.lnxyls.cn

Java: resp.statusCode()
来源：http://cq.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://la.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://hk.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://tb.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://kj.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ae.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://cp.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eq.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ht.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uv.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fm.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xt.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sw.wgjwhj.cn

================================================================================
来源：http://ch.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://yv.asd995.cn

================================================================================
来源：http://xu.jctech888.com.cn

[M01] 读取命令行参数
来源：http://tl.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://nw.nszjky.cn

PHP:  $argv;  $argc;
来源：http://bz.asd995.cn


<!-- 参考信息 -->