代发 wailian999

TS:   s.match(/\d+/g)
来源：http://pa.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zi.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ng.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://pd.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kn.yuexingan06.cn

[I03] 提取捕获分组
来源：http://oo.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cy.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kv.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zi.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ml.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gn.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fe.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ny.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yp.shxzukj.cn

[I04] 正则替换
来源：http://ly.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vm.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wj.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vp.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yu.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wo.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rl.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ok.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://do.haigaiapp.cn

[I05] 按正则拆分
来源：http://er.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ub.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hj.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://zw.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://tr.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://th.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bj.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qu.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ma.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uq.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qr.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zv.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pe.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ax.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mu.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hw.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ai.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://js.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://vm.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pq.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zz.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wz.nszjky.cn

TS:   /error/gim
来源：http://yt.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gn.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yw.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://az.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ia.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ti.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zb.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dy.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zj.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bm.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aj.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vb.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ua.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yc.jianghongdianzi.cn

================================================================================
来源：http://yc.huanxung.cn

J. 日期与时间
来源：http://zi.huixinmuqiang.cn

================================================================================
来源：http://da.gzmigu.cn

[J01] 获取当前时间
来源：http://vh.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uq.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ka.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://lh.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://oh.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gt.chemitech.net.cn

Go:   time.Now()
来源：http://sg.chemitech.net.cn

Ruby: Time.now
来源：http://is.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zk.jctech888.com.cn

[J02] 格式化输出
来源：http://su.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aw.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://di.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://an.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://ak.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fg.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yw.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ir.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gf.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://rb.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qa.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://py.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://al.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://hn.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ia.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lv.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://bw.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qg.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ga.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ws.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bq.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mb.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wu.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yw.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yl.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://os.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://th.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://fl.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://al.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jg.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://es.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://gu.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nm.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://sx.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ed.chemitech.net.cn

[J06] 计算两时间之差
来源：http://xw.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://bz.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://oe.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yf.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://le.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vx.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://av.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://ff.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://xf.chemitech.net.cn

[J07] 比较两个日期
来源：http://zx.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://pq.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wy.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cx.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pv.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qi.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jn.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tn.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://jx.nszjky.cn

[J08] 提取年月日与星期
来源：http://qb.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zl.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sk.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sp.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://do.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ex.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dx.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://et.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cl.newstarts.cn

[J09] 时区处理
来源：http://rz.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gp.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iw.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gc.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ge.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cq.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lx.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tk.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mt.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://zn.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nl.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yy.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ua.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vu.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hj.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pl.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ac.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sy.nszjky.cn

================================================================================
来源：http://fh.nszjky.cn

K. JSON 与序列化
来源：http://eu.newstarts.cn

================================================================================
来源：http://ux.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://op.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ga.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wl.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://et.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://cz.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tv.newstarts.cn

Go:   json.Marshal(obj)
来源：http://wd.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xq.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ma.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://vt.chemitech.net.cn

Py:   json.loads(s)
来源：http://hc.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cc.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ks.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://pg.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vs.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://jq.colortex.cn

Ruby: JSON.parse(s)
来源：http://gn.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zb.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://lq.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ft.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xj.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yg.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hw.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wq.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wp.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ff.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://fn.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://av.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://es.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ro.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hc.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kt.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qx.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pv.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kv.szsharing.cn

[K05] 深拷贝对象
来源：http://tu.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://qh.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://oq.gzmigu.cn

JS:   structuredClone(obj)
来源：http://ho.colortex.cn

TS:   structuredClone(obj)
来源：http://ph.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zd.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yv.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yz.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fy.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://na.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yh.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pz.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yk.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qr.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fl.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://js.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kn.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rj.hahajie.cn

[K07] 进制转换
来源：http://mj.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rw.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nl.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mc.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iv.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tw.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dc.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ha.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ib.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://si.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://fs.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://da.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://ba.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://dh.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mc.wgjwhj.cn

Go:   encoding/gob
来源：http://qt.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://og.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zm.huixiangedu.cn

================================================================================
来源：http://hi.szxytkj.cn

L. 网络请求
来源：http://ih.szsharing.cn

================================================================================
来源：http://eh.colortex.cn

[L01] 发送 GET 请求
来源：http://px.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jb.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oa.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ol.panjiajie.cn

TS:   await fetch(url)
来源：http://bq.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lh.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://xa.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ih.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pa.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://yb.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ja.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tl.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qa.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wu.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nc.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ek.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ye.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://ij.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yb.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pd.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wc.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yo.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hg.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zx.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gq.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://il.hnjuh.cn

[L04] 设置超时
来源：http://mf.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://xm.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pq.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://so.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://id.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ni.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gn.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://wl.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://al.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sp.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pt.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kx.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ly.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rw.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iy.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cb.nicolike.cn

[L06] 解析响应为 JSON
来源：http://li.asd995.cn

Py:   resp.json()
来源：http://xl.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://eg.lnxyls.cn

JS:   await resp.json()
来源：http://kv.huixiangedu.cn

TS:   await resp.json()
来源：http://ju.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mv.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sa.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://og.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ty.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://ta.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jz.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lu.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://sd.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://qm.hahajie.cn

Java: resp.statusCode()
来源：http://on.yuexingan06.cn

Go:   resp.StatusCode
来源：http://si.shxzskj.cn

Ruby: resp.code.to_i
来源：http://iq.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://dv.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://wf.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tn.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ch.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dn.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ei.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ap.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://os.asd995.cn


<!-- 参考信息 -->