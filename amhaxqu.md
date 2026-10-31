代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gg.haigaiapp.cn

[I03] 提取捕获分组
来源：http://bg.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vn.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oc.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oa.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cc.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://do.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ba.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hu.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hp.panjiajie.cn

[I04] 正则替换
来源：http://gf.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hh.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ku.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xi.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eo.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nu.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kh.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oe.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vo.wgjwhj.cn

[I05] 按正则拆分
来源：http://ga.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xi.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tx.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://dl.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://re.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://bg.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://np.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qv.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xg.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hq.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lj.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rk.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hm.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yg.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://id.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tb.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ld.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kt.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://pd.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://re.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://on.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vr.shxzskj.cn

TS:   /error/gim
来源：http://qf.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://do.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://me.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://zw.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ro.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://tw.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qd.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ro.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vv.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qb.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oz.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ao.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lj.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yb.jctech888.com.cn

================================================================================
来源：http://zt.yuntaijiaju.cn

J. 日期与时间
来源：http://ct.521024.cn

================================================================================
来源：http://vq.huixiangedu.cn

[J01] 获取当前时间
来源：http://te.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ix.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tr.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://kl.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://ta.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gy.hahajie.cn

Go:   time.Now()
来源：http://ta.nicolike.cn

Ruby: Time.now
来源：http://pk.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gc.jctech888.com.cn

[J02] 格式化输出
来源：http://gv.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vr.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tq.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://da.panjiajie.cn

TS:   d.toISOString()
来源：http://ce.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kg.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rm.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fe.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wl.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://sz.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zs.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nb.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://xi.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://af.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rh.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oy.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://jm.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://el.nszjky.cn

[J04] 时间戳与日期互转
来源：http://hm.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iu.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ic.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gb.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wj.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dp.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mv.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pt.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hn.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://wx.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://sg.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aj.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ry.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fa.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://zy.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gu.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://vc.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dg.szxytkj.cn

[J06] 计算两时间之差
来源：http://jx.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://nr.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://nt.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fk.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ff.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lo.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://xn.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://ro.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://mq.gzmigu.cn

[J07] 比较两个日期
来源：http://bc.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://yo.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qs.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gc.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xk.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dr.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oq.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nc.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://oq.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ky.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ho.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lg.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ce.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mb.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qd.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jz.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lt.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gx.hnjuh.cn

[J09] 时区处理
来源：http://di.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bz.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zy.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gn.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fq.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uz.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dp.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://on.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gx.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://kc.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rh.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ez.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qw.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cs.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xv.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qn.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qi.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zb.huixinmuqiang.cn

================================================================================
来源：http://gb.muxihuayi.cn

K. JSON 与序列化
来源：http://kq.nicolike.cn

================================================================================
来源：http://rf.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://pr.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ll.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://et.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://xs.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://iq.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pu.hahajie.cn

Go:   json.Marshal(obj)
来源：http://oh.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ot.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sx.szsharing.cn

[K02] JSON 字符串转对象
来源：http://of.hnjuh.cn

Py:   json.loads(s)
来源：http://ut.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ck.nszjky.cn

JS:   JSON.parse(s)
来源：http://jb.szsharing.cn

TS:   JSON.parse(s)
来源：http://da.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jb.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://lo.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://qm.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jl.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://mp.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ip.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dy.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gb.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iu.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://va.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://em.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jh.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fw.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://dm.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ki.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dh.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pj.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pv.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wv.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lq.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xh.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ci.gzmigu.cn

[K05] 深拷贝对象
来源：http://aj.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://zp.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://in.huanxung.cn

JS:   structuredClone(obj)
来源：http://kw.szxytkj.cn

TS:   structuredClone(obj)
来源：http://zo.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ba.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oa.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kd.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nh.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://oo.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pq.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hi.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ho.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xn.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bz.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ec.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sx.bjjhwx.cn

[K07] 进制转换
来源：http://da.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uz.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://be.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ea.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gh.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fr.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://og.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xv.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://od.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://pk.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kx.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://wu.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://mj.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nx.nszjky.cn

Go:   encoding/gob
来源：http://fp.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://pn.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bs.chemitech.net.cn

================================================================================
来源：http://jq.panjiajie.cn

L. 网络请求
来源：http://yf.haigaiapp.cn

================================================================================
来源：http://au.szxytkj.cn

[L01] 发送 GET 请求
来源：http://tf.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tb.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nf.9csxet.cn

JS:   await fetch(url)
来源：http://io.newstarts.cn

TS:   await fetch(url)
来源：http://lo.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ji.521024.cn

Go:   resp, err := http.Get(url)
来源：http://vs.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cd.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://um.nicolike.cn

[L02] 发送 POST JSON
来源：http://tv.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nm.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ji.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sv.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://av.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cs.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cs.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gg.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bi.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://nr.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ed.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rq.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pj.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uq.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ec.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://og.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yf.huixinmuqiang.cn

[L04] 设置超时
来源：http://xw.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://dn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uw.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bh.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://me.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tw.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fj.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ot.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mi.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://sn.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kq.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nf.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xx.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pm.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pv.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mc.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dt.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vu.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ou.nicolike.cn

Py:   resp.json()
来源：http://od.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://hb.chemitech.net.cn

JS:   await resp.json()
来源：http://gj.lnxyls.cn

TS:   await resp.json()
来源：http://cn.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hg.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hl.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://zq.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://we.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ir.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kz.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://cd.asd995.cn

TS:   resp.ok;  resp.status
来源：http://bj.nszjky.cn

Java: resp.statusCode()
来源：http://pq.haigaiapp.cn

Go:   resp.StatusCode
来源：http://jt.panjiajie.cn

Ruby: resp.code.to_i
来源：http://yr.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://ma.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://uh.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mm.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://od.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vn.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ix.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yw.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zc.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yf.9csxet.cn

================================================================================
来源：http://en.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://ry.huixinmuqiang.cn


<!-- 参考信息 -->