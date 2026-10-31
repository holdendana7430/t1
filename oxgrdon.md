代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vx.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xp.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tn.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oc.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ou.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fl.bjjhwx.cn

[I04] 正则替换
来源：http://qy.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qs.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ei.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vb.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oa.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pz.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jr.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dr.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yc.yuexingan06.cn

[I05] 按正则拆分
来源：http://vg.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vf.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aa.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://wb.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://fl.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://mi.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://it.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zm.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://js.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ax.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vj.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mf.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://os.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nd.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nz.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kw.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kb.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://tb.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yr.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://el.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ej.hahajie.cn

TS:   /error/gim
来源：http://yi.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lq.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tr.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://qk.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ii.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://ov.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tp.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fr.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://md.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qe.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xi.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lm.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ew.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hk.yuexingan06.cn

================================================================================
来源：http://wl.gzmigu.cn

J. 日期与时间
来源：http://vm.haigaiapp.cn

================================================================================
来源：http://rz.bookmarksfly.cn

[J01] 获取当前时间
来源：http://fi.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gj.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fj.colortex.cn

JS:   new Date();  Date.now()
来源：http://ym.nszjky.cn

TS:   new Date();  Date.now()
来源：http://dw.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mh.wgjwhj.cn

Go:   time.Now()
来源：http://qs.szxytkj.cn

Ruby: Time.now
来源：http://yc.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dh.gzmigu.cn

[J02] 格式化输出
来源：http://bl.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pj.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hk.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lw.chemitech.net.cn

TS:   d.toISOString()
来源：http://sp.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zz.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vj.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pl.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hx.hahajie.cn

[J03] 字符串解析为日期
来源：http://jc.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kq.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bg.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://jg.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://yl.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sc.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ba.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://lf.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xw.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://ey.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jl.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zu.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cx.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sv.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ku.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dn.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qg.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fs.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://hz.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://el.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zc.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://au.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lz.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://wc.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eb.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ym.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ou.wgjwhj.cn

[J06] 计算两时间之差
来源：http://se.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://co.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://cw.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uf.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ye.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://da.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://yr.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://xu.wgjwhj.cn

[J07] 比较两个日期
来源：http://jf.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://xi.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yu.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fy.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://op.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kv.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sm.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ba.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://er.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://cu.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fy.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fz.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://du.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zf.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zc.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dp.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bm.shxzukj.cn

[J09] 时区处理
来源：http://ne.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hu.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uc.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bk.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xn.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kq.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zg.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lp.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kj.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://ji.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ov.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://na.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uc.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mz.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://an.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tp.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pb.jctech888.com.cn

================================================================================
来源：http://xa.asd995.cn

K. JSON 与序列化
来源：http://jv.szsharing.cn

================================================================================
来源：http://nx.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ca.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cr.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zo.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ug.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://ia.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ug.521024.cn

Go:   json.Marshal(obj)
来源：http://kc.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ex.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hm.newstarts.cn

[K02] JSON 字符串转对象
来源：http://fv.nicolike.cn

Py:   json.loads(s)
来源：http://bx.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iq.asd995.cn

JS:   JSON.parse(s)
来源：http://gu.gzmigu.cn

TS:   JSON.parse(s)
来源：http://yc.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ja.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://po.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ta.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ny.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ee.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://no.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qc.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ym.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wm.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mx.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pb.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iq.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://we.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://ny.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yk.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gv.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cp.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qe.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uq.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wa.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nf.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fk.szsharing.cn

[K05] 深拷贝对象
来源：http://ho.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://jj.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://cv.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://mn.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://fb.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bs.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tg.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xl.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://na.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://bf.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yg.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wf.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dd.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://no.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mc.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://op.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ws.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ax.shxzskj.cn

[K07] 进制转换
来源：http://tb.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zu.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kr.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xr.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pp.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://na.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rb.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mc.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://ly.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://wf.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://um.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://rw.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://wz.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xv.jianghongdianzi.cn

Go:   encoding/gob
来源：http://di.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://bi.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mg.gzmigu.cn

================================================================================
来源：http://ag.jianghongdianzi.cn

L. 网络请求
来源：http://xh.shxzukj.cn

================================================================================
来源：http://by.9csxet.cn

[L01] 发送 GET 请求
来源：http://yn.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tk.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mm.haigaiapp.cn

JS:   await fetch(url)
来源：http://it.newstarts.cn

TS:   await fetch(url)
来源：http://hw.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://js.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://lu.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nc.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gq.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://cx.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nm.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wr.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gs.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tl.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ct.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hf.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yb.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tw.hnjuh.cn

[L03] 设置自定义请求头
来源：http://gg.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wx.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pa.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yu.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pa.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oh.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ak.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eq.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sl.chemitech.net.cn

[L04] 设置超时
来源：http://yk.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://vq.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ac.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lx.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tu.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hs.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yu.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ew.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hp.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://dd.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rz.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jb.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hl.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ka.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ez.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cc.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tg.nicolike.cn

[L06] 解析响应为 JSON
来源：http://eq.jctech888.com.cn

Py:   resp.json()
来源：http://tk.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ki.9csxet.cn

JS:   await resp.json()
来源：http://wn.huanxung.cn

TS:   await resp.json()
来源：http://de.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vs.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wh.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://dd.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sz.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://jz.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://de.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yg.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://nf.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://au.gzmigu.cn

Java: resp.statusCode()
来源：http://yx.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://dl.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://pq.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://xk.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ev.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dw.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ah.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://go.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://da.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hv.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uy.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vb.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cs.szsharing.cn

================================================================================
来源：http://qi.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://hn.huanxung.cn

================================================================================
来源：http://hl.bjjhwx.cn

[M01] 读取命令行参数
来源：http://cm.szsharing.cn

Py:   sys.argv[1:]
来源：http://tq.nszjky.cn

PHP:  $argv;  $argc;
来源：http://zv.nszjky.cn


<!-- 参考信息 -->