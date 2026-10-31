代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dc.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://rn.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qq.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nn.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vz.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ca.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gm.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ec.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bq.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kv.gzmigu.cn

[I04] 正则替换
来源：http://gh.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://at.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iz.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ou.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mh.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xp.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bl.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fs.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ve.yuexingan06.cn

[I05] 按正则拆分
来源：http://rk.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nu.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ac.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://fs.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://go.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://km.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gp.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://je.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sq.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ng.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://my.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ni.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ak.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ee.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ri.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://jt.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://up.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dm.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://na.yuntaijiaju.cn

TS:   /error/gim
来源：http://zi.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lg.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sa.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://wg.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hv.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://qy.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cm.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lc.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bv.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qp.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nk.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tv.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bd.shxzskj.cn

================================================================================
来源：http://wh.szsharing.cn

J. 日期与时间
来源：http://wu.huanxung.cn

================================================================================
来源：http://ef.bookmarksfly.cn

[J01] 获取当前时间
来源：http://tg.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zr.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uo.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ck.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://fb.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hj.colortex.cn

Go:   time.Now()
来源：http://ru.huanxung.cn

Ruby: Time.now
来源：http://ql.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ye.wgjwhj.cn

[J02] 格式化输出
来源：http://ao.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aw.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ig.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nm.hahajie.cn

TS:   d.toISOString()
来源：http://wc.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wn.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nh.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zu.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://to.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://xa.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jd.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qd.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://rl.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://tr.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hg.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gr.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://xq.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qn.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://vk.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ay.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cv.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gr.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fj.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wh.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bh.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bp.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ki.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://sj.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://eo.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qt.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qo.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sz.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://dz.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qj.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://tf.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ei.muxihuayi.cn

[J06] 计算两时间之差
来源：http://sa.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://ai.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://yc.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zt.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ak.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ne.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://lk.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://cg.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://qt.newstarts.cn

[J07] 比较两个日期
来源：http://nh.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://hk.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ax.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mo.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ex.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oh.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sb.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ac.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://yg.hahajie.cn

[J08] 提取年月日与星期
来源：http://af.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lw.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xg.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pi.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://av.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vp.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ed.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xv.hnjuh.cn

[J09] 时区处理
来源：http://qj.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xn.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cw.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qf.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ee.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jj.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ju.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ve.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://bo.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xp.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yk.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://th.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ex.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kt.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cz.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yc.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gx.panjiajie.cn

================================================================================
来源：http://tr.hnjuh.cn

K. JSON 与序列化
来源：http://qq.9csxet.cn

================================================================================
来源：http://ix.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://gj.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ak.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mc.colortex.cn

JS:   JSON.stringify(obj)
来源：http://sf.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://uv.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yk.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://bz.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mg.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zg.nszjky.cn

[K02] JSON 字符串转对象
来源：http://bk.bookmarksfly.cn

Py:   json.loads(s)
来源：http://el.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fv.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://hm.hahajie.cn

TS:   JSON.parse(s)
来源：http://xl.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://va.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ri.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://si.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qq.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://go.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gl.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cn.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sc.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qk.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ho.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jl.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ep.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hb.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://gp.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xf.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hs.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ku.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yd.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lw.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zo.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nh.shtwfgs.cn

[K05] 深拷贝对象
来源：http://je.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://gg.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://bb.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://fn.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ge.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nb.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xz.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lr.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qa.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://em.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://te.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://es.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pd.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tw.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xf.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iv.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tc.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ec.bookmarksfly.cn

[K07] 进制转换
来源：http://yu.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gi.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hc.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ii.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://of.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nv.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://me.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iu.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gp.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://xr.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://sf.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kt.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://kr.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://oa.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tv.huanxung.cn

Go:   encoding/gob
来源：http://iv.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://ei.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lf.asd995.cn

================================================================================
来源：http://os.huanxung.cn

L. 网络请求
来源：http://cq.huanxung.cn

================================================================================
来源：http://ep.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://bx.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jx.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hi.nszjky.cn

JS:   await fetch(url)
来源：http://ef.gzmigu.cn

TS:   await fetch(url)
来源：http://pi.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bk.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://cp.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hp.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://un.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zy.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ef.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cm.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ur.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tu.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zd.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cf.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xp.hnjuh.cn

[L03] 设置自定义请求头
来源：http://am.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nf.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mc.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fb.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jt.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jj.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cl.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sy.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://or.9csxet.cn

[L04] 设置超时
来源：http://se.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://jw.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dd.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ua.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://he.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ps.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kf.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sm.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jl.huanxung.cn

[L05] 上传文件（multipart）
来源：http://sg.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://st.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zy.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://so.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bz.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tp.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oa.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wa.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zc.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://yi.shxzskj.cn

Py:   resp.json()
来源：http://hr.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://bn.gzmigu.cn

JS:   await resp.json()
来源：http://ly.jianghongdianzi.cn

TS:   await resp.json()
来源：http://kz.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ze.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mw.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://ea.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nr.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://mt.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hm.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://do.521024.cn

TS:   resp.ok;  resp.status
来源：http://wt.panjiajie.cn

Java: resp.statusCode()
来源：http://ea.yuexingan06.cn

Go:   resp.StatusCode
来源：http://fq.lnxyls.cn

Ruby: resp.code.to_i
来源：http://op.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://db.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://fr.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qw.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://if.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ww.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hw.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://po.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xc.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wa.chemitech.net.cn

================================================================================
来源：http://da.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://lf.colortex.cn


<!-- 参考信息 -->