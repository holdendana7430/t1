代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ko.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ui.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dm.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wo.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://by.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lo.jianghongdianzi.cn

[I04] 正则替换
来源：http://gq.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jf.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rv.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zb.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ii.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fm.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lh.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xz.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ms.bookmarksfly.cn

[I05] 按正则拆分
来源：http://kv.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tv.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://ex.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://ci.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://xj.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vc.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yh.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pd.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ex.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rr.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qn.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iv.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gc.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vk.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cr.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://od.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tq.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://hd.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hy.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wq.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wo.nicolike.cn

TS:   /error/gim
来源：http://tg.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jv.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wo.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://ew.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dd.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://go.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wl.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kv.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ol.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vm.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ak.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://os.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lv.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rd.yuntaijiaju.cn

================================================================================
来源：http://aj.newstarts.cn

J. 日期与时间
来源：http://ra.bookmarksfly.cn

================================================================================
来源：http://th.newstarts.cn

[J01] 获取当前时间
来源：http://cj.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fk.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ig.nszjky.cn

JS:   new Date();  Date.now()
来源：http://on.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://qx.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://io.wgjwhj.cn

Go:   time.Now()
来源：http://iu.huixiangedu.cn

Ruby: Time.now
来源：http://ob.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bw.wgjwhj.cn

[J02] 格式化输出
来源：http://ih.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rx.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tz.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xf.shtwfgs.cn

TS:   d.toISOString()
来源：http://xy.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ex.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qo.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ek.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://za.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://cc.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bg.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nc.asd995.cn

JS:   new Date("2024-01-02")
来源：http://tl.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://vx.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xq.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zc.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://zg.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ok.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://os.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iw.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gm.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gn.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ao.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://me.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hh.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ni.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dt.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://np.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://km.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jq.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://um.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jq.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://yy.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bj.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://mj.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wd.huanxung.cn

[J06] 计算两时间之差
来源：http://uk.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://ln.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://px.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ju.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ib.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xj.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://af.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://lo.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://mc.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://vh.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://rl.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ft.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ia.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ww.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pf.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://de.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://km.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://yg.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://pr.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ow.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://af.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sc.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://je.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://im.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qv.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ce.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wq.nszjky.cn

[J09] 时区处理
来源：http://sz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://km.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vw.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yh.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jz.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jb.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wh.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ml.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://ba.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cr.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://we.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mn.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lc.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eu.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yc.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qr.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sc.521024.cn

================================================================================
来源：http://om.shtwfgs.cn

K. JSON 与序列化
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://bw.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://qg.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oc.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cv.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://yn.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://wt.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hc.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ao.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mj.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vi.nszjky.cn

[K02] JSON 字符串转对象
来源：http://iy.521024.cn

Py:   json.loads(s)
来源：http://fx.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wz.szsharing.cn

JS:   JSON.parse(s)
来源：http://li.asd995.cn

TS:   JSON.parse(s)
来源：http://vm.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zf.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://kb.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://nu.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jq.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ql.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ga.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bg.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pt.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cf.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ll.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kp.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kd.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sv.newstarts.cn

[K04] 读取 JSON 文件
来源：http://cp.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sy.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ru.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ml.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cc.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zb.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wa.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qh.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://at.521024.cn

[K05] 深拷贝对象
来源：http://xn.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://co.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://ri.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ii.nszjky.cn

TS:   structuredClone(obj)
来源：http://xd.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ma.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gk.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ol.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qz.newstarts.cn

[K06] 解析 URL 查询串
来源：http://uh.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vu.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lw.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jq.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kr.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ve.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://au.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ua.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gk.asd995.cn

[K07] 进制转换
来源：http://dt.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cs.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qo.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dd.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tq.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jk.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xx.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hg.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kg.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://kr.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://sa.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uh.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://fk.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://we.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dx.shxzskj.cn

Go:   encoding/gob
来源：http://xs.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://sv.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ng.shxzukj.cn

================================================================================
来源：http://qq.lnxyls.cn

L. 网络请求
来源：http://gr.asd995.cn

================================================================================
来源：http://hl.szsharing.cn

[L01] 发送 GET 请求
来源：http://lw.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lt.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://td.nicolike.cn

JS:   await fetch(url)
来源：http://bq.shxzukj.cn

TS:   await fetch(url)
来源：http://ix.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kb.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://or.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yq.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yc.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://gd.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fw.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://br.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fo.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ed.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://op.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bs.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sh.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pv.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://xy.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ql.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fo.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ms.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ky.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ni.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zu.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zw.yuntaijiaju.cn

[L04] 设置超时
来源：http://wb.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://tl.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://no.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uw.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iy.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jn.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bc.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://up.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://ca.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://af.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vy.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kx.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oy.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yh.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mx.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lg.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pl.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://fo.hahajie.cn

Py:   resp.json()
来源：http://oe.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://pv.szsharing.cn

JS:   await resp.json()
来源：http://fu.shxzskj.cn

TS:   await resp.json()
来源：http://vi.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ky.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ar.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://gp.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hj.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ya.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ef.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xm.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://av.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://tc.nszjky.cn

Java: resp.statusCode()
来源：http://ag.hnjuh.cn

Go:   resp.StatusCode
来源：http://zu.9csxet.cn

Ruby: resp.code.to_i
来源：http://sa.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://jf.szsharing.cn

[L08] 并发请求多个地址
来源：http://yt.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sv.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://xr.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tf.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xr.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cs.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sj.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://su.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bh.muxihuayi.cn

================================================================================
来源：http://ld.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://on.asd995.cn

================================================================================
来源：http://pl.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://tz.szsharing.cn

Py:   sys.argv[1:]
来源：http://qz.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://mp.lnxyls.cn


<!-- 参考信息 -->