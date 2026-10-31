代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ss.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gk.hnjuh.cn

[I04] 正则替换
来源：http://tw.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://op.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://at.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nv.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ab.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ti.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ex.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ih.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://al.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://bc.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ez.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wu.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ml.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://kp.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://pv.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vp.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zi.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jp.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tp.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://we.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vd.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xn.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ih.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sv.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ud.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fq.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://um.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://lp.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ta.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://an.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ls.colortex.cn

TS:   /error/gim
来源：http://sf.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qu.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bo.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://iu.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vd.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://yd.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xo.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wd.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://to.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fi.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rn.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iv.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ui.muxihuayi.cn

================================================================================
来源：http://pc.chemitech.net.cn

J. 日期与时间
来源：http://bk.shtwfgs.cn

================================================================================
来源：http://or.lnxyls.cn

[J01] 获取当前时间
来源：http://ru.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yu.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://al.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://rc.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://qw.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gi.521024.cn

Go:   time.Now()
来源：http://ll.jianghongdianzi.cn

Ruby: Time.now
来源：http://mg.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bt.haigaiapp.cn

[J02] 格式化输出
来源：http://pb.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nq.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nt.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hr.huixiangedu.cn

TS:   d.toISOString()
来源：http://fl.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pd.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ss.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://js.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vm.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://fy.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qp.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eh.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://wc.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://yd.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aj.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://du.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://us.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fb.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://es.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ct.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sb.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zl.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lb.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ro.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oz.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ad.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qm.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ek.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ec.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hh.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dl.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hk.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ug.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://po.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://dg.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://he.9csxet.cn

[J06] 计算两时间之差
来源：http://yl.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://ki.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://rf.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ds.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iw.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sq.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ki.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://qp.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://zb.jctech888.com.cn

[J07] 比较两个日期
来源：http://ej.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://il.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xp.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dp.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rn.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://km.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cu.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xu.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zn.panjiajie.cn

[J08] 提取年月日与星期
来源：http://yc.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jb.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vc.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fi.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qo.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wv.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wp.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ph.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fb.szxytkj.cn

[J09] 时区处理
来源：http://ea.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://po.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mr.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yb.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://km.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rc.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fm.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xd.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rk.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://yi.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uy.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ti.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cv.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fh.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mv.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://un.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ta.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uy.9csxet.cn

================================================================================
来源：http://bf.nicolike.cn

K. JSON 与序列化
来源：http://du.9csxet.cn

================================================================================
来源：http://rw.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://wd.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kx.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pi.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://rh.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://wv.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://os.colortex.cn

Go:   json.Marshal(obj)
来源：http://ua.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cu.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dj.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://wc.huixiangedu.cn

Py:   json.loads(s)
来源：http://su.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://km.shxzukj.cn

JS:   JSON.parse(s)
来源：http://ok.9csxet.cn

TS:   JSON.parse(s)
来源：http://fr.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ya.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://tj.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://wz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cy.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://bt.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ev.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://al.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ky.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ti.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wn.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ko.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qq.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hw.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://tl.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cj.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ez.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qq.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://om.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hu.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wm.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wr.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pe.szxytkj.cn

[K05] 深拷贝对象
来源：http://zy.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://cy.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://qy.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://mc.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://eu.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wb.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fc.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qk.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fh.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://tf.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zu.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xc.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xi.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ck.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://os.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zj.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ss.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://px.panjiajie.cn

[K07] 进制转换
来源：http://ai.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bg.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gm.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cb.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lz.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vy.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aa.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ow.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mj.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://gt.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://wa.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ln.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ll.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://tk.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hw.lnxyls.cn

Go:   encoding/gob
来源：http://ug.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://wj.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vv.shxzskj.cn

================================================================================
来源：http://uq.yuntaijiaju.cn

L. 网络请求
来源：http://cf.huixiangedu.cn

================================================================================
来源：http://ad.9csxet.cn

[L01] 发送 GET 请求
来源：http://cq.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ir.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mp.hahajie.cn

JS:   await fetch(url)
来源：http://xc.yuexingan06.cn

TS:   await fetch(url)
来源：http://dg.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vv.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://eu.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jo.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://id.hnjuh.cn

[L02] 发送 POST JSON
来源：http://sm.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wb.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yq.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wj.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rt.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zk.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ka.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rw.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gv.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://ih.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vi.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jk.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gb.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tz.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xr.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://co.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vq.huanxung.cn

[L04] 设置超时
来源：http://ed.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://nm.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ru.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://di.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ck.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qe.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://la.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uf.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hc.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://fo.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fl.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bn.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aa.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nq.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pr.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ha.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://si.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://km.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://op.shxzukj.cn

Py:   resp.json()
来源：http://eh.szsharing.cn

PHP:  json_decode($body, true);
来源：http://jt.yuexingan06.cn

JS:   await resp.json()
来源：http://lb.asd995.cn

TS:   await resp.json()
来源：http://ja.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kj.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gn.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://cc.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sj.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ts.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://il.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ri.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://gm.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://dy.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://eu.shtwfgs.cn

Go:   resp.StatusCode
来源：http://nk.nszjky.cn

Ruby: resp.code.to_i
来源：http://wu.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://rn.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://fb.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ff.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://kl.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gp.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gt.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hq.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sh.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://to.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gf.521024.cn

================================================================================
来源：http://qr.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://mv.colortex.cn

================================================================================
来源：http://pa.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://si.nszjky.cn

Py:   sys.argv[1:]
来源：http://kf.newstarts.cn

PHP:  $argv;  $argc;
来源：http://pt.asd995.cn

JS:   process.argv.slice(2)
来源：http://jb.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://sr.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ib.colortex.cn

Go:   os.Args[1:]
来源：http://fg.huanxung.cn


<!-- 参考信息 -->