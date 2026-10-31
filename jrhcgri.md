代发 wailian999

[I02] 提取所有匹配
来源：http://gk.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://bu.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mr.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cx.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://qh.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wl.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pw.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://fu.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://al.yuexingan06.cn

[I03] 提取捕获分组
来源：http://kb.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://no.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ke.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xk.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dv.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sm.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uj.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wt.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cy.521024.cn

[I04] 正则替换
来源：http://eu.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vk.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yl.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iu.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qj.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ef.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yg.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gk.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ma.hahajie.cn

[I05] 按正则拆分
来源：http://fb.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oa.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://km.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://jt.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://oa.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://wg.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rx.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lk.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ly.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lx.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ms.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ee.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mr.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yc.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gs.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://si.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xe.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ok.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://pk.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fe.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gs.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kr.9csxet.cn

TS:   /error/gim
来源：http://wz.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ia.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wk.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://xb.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iy.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://tq.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vs.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iz.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ji.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yo.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://he.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qp.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://le.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fk.szsharing.cn

================================================================================
来源：http://ri.yuntaijiaju.cn

J. 日期与时间
来源：http://qg.bjjhwx.cn

================================================================================
来源：http://lv.wgjwhj.cn

[J01] 获取当前时间
来源：http://jc.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://th.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xt.nszjky.cn

JS:   new Date();  Date.now()
来源：http://cx.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://tk.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ls.yuntaijiaju.cn

Go:   time.Now()
来源：http://ce.bookmarksfly.cn

Ruby: Time.now
来源：http://lc.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hv.newstarts.cn

[J02] 格式化输出
来源：http://tq.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xl.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dj.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fb.gzmigu.cn

TS:   d.toISOString()
来源：http://vn.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dv.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yj.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ea.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qe.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://fs.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dg.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ng.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://jl.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://yh.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wl.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qm.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://en.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fn.521024.cn

[J04] 时间戳与日期互转
来源：http://na.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ws.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vx.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xx.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ol.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qr.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rx.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oj.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ju.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://tt.asd995.cn

Py:   now + timedelta(days=7)
来源：http://qw.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nu.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fv.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qg.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://rz.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uq.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://my.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vl.szsharing.cn

[J06] 计算两时间之差
来源：http://cv.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://qe.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://rd.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vj.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jt.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sj.521024.cn

Go:   end.Sub(start).Hours()
来源：http://pd.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://bu.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ug.bjjhwx.cn

[J07] 比较两个日期
来源：http://gr.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://wh.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yt.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ct.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lt.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pl.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://et.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vk.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://vp.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://hd.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ee.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vu.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hp.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kj.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pk.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bz.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hk.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xw.gzmigu.cn

[J09] 时区处理
来源：http://cd.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://be.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nv.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ml.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uh.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qr.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ny.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://am.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yj.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ok.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ft.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://js.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gv.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lt.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ul.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bp.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mp.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kt.jctech888.com.cn

================================================================================
来源：http://bw.bookmarksfly.cn

K. JSON 与序列化
来源：http://zo.shxzukj.cn

================================================================================
来源：http://yv.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://jn.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ga.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ob.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://un.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://pd.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wk.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://ji.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ns.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ub.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://ib.colortex.cn

Py:   json.loads(s)
来源：http://lh.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pb.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://mx.hahajie.cn

TS:   JSON.parse(s)
来源：http://mh.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://su.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://yn.huanxung.cn

Ruby: JSON.parse(s)
来源：http://ia.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eo.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ds.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iw.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qy.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qc.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gw.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sn.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eh.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ik.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ax.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://gt.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zb.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ar.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ua.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uu.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qw.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ac.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bn.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mp.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ie.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://eg.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://gs.szxytkj.cn

JS:   structuredClone(obj)
来源：http://aj.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ah.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lf.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ph.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fc.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yw.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://wx.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zi.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://em.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gs.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hq.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tj.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ow.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aw.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fz.nicolike.cn

[K07] 进制转换
来源：http://yc.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rl.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nb.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nq.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sc.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lk.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://if.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qc.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ji.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://eo.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://et.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uc.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://lt.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://rq.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nw.bookmarksfly.cn

Go:   encoding/gob
来源：http://rt.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://kg.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ly.nszjky.cn

================================================================================
来源：http://kq.asd995.cn

L. 网络请求
来源：http://dq.huixiangedu.cn

================================================================================
来源：http://zc.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://vq.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hy.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zt.yuexingan06.cn

JS:   await fetch(url)
来源：http://hc.hahajie.cn

TS:   await fetch(url)
来源：http://is.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yf.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://ro.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ke.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mn.9csxet.cn

[L02] 发送 POST JSON
来源：http://ti.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ha.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hc.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bl.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ec.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ux.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://st.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pf.szxytkj.cn

[L03] 设置自定义请求头
来源：http://pj.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hd.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tc.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bq.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ar.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vd.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bg.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jr.haigaiapp.cn

[L04] 设置超时
来源：http://cs.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://ne.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lo.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://od.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ol.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aw.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jq.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ll.huanxung.cn

[L05] 上传文件（multipart）
来源：http://hv.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jc.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://an.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vg.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://az.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xn.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://av.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kp.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ot.asd995.cn

[L06] 解析响应为 JSON
来源：http://xl.newstarts.cn

Py:   resp.json()
来源：http://kt.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://sj.nicolike.cn

JS:   await resp.json()
来源：http://px.hnjuh.cn

TS:   await resp.json()
来源：http://lk.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mc.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uk.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ng.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vr.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://es.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ko.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ig.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://or.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://fw.nicolike.cn

Java: resp.statusCode()
来源：http://gn.521024.cn

Go:   resp.StatusCode
来源：http://sy.9csxet.cn

Ruby: resp.code.to_i
来源：http://cz.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://ou.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ae.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rc.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://pl.bjjhwx.cn


<!-- 参考信息 -->