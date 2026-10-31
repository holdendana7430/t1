代发 wailian999

TS:   s.match(/\d+/g)
来源：http://gh.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dy.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://og.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://pr.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rr.colortex.cn

[I03] 提取捕获分组
来源：http://xb.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pu.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nf.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jh.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zc.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ro.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tn.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ao.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zo.521024.cn

[I04] 正则替换
来源：http://iw.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bc.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bu.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yg.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rf.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fa.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sf.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.huanxung.cn

[I05] 按正则拆分
来源：http://fy.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sp.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ee.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://yd.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://re.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://na.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gl.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ek.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ur.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hn.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oi.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mm.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://si.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zf.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tt.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yl.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fn.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pt.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://qa.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qn.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zk.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vy.szxytkj.cn

TS:   /error/gim
来源：http://vs.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xa.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ie.asd995.cn

Ruby: s.scan(/error/i)
来源：http://qm.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hq.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://jj.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://al.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kg.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://na.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ic.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wd.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ud.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zz.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zz.hnjuh.cn

================================================================================
来源：http://bp.panjiajie.cn

J. 日期与时间
来源：http://cr.9csxet.cn

================================================================================
来源：http://qh.hahajie.cn

[J01] 获取当前时间
来源：http://pj.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vq.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vz.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://bw.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://lz.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iu.huixinmuqiang.cn

Go:   time.Now()
来源：http://qh.shxzukj.cn

Ruby: Time.now
来源：http://fy.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ms.wgjwhj.cn

[J02] 格式化输出
来源：http://yi.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zy.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fr.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cw.newstarts.cn

TS:   d.toISOString()
来源：http://fg.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hr.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ux.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jl.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lv.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://wi.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ox.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mj.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://wh.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://pv.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qe.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mo.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://td.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vz.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://xe.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dm.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wr.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sq.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fk.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lw.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rl.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ka.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vx.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://kj.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://rg.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ss.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jv.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xk.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://uu.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ej.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://iq.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://na.huixiangedu.cn

[J06] 计算两时间之差
来源：http://yy.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://kt.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://go.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xj.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ua.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kf.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://us.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://os.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://bf.chemitech.net.cn

[J07] 比较两个日期
来源：http://xq.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://vd.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ta.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yl.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uf.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tk.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ce.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lm.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://da.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://nb.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iy.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vt.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tt.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://no.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ds.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lg.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hi.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kp.yuexingan06.cn

[J09] 时区处理
来源：http://qy.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bg.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xk.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://br.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://un.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ue.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ir.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fi.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zk.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://vb.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qd.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xr.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fd.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://po.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dg.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jd.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fa.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sl.huanxung.cn

================================================================================
来源：http://iv.lnxyls.cn

K. JSON 与序列化
来源：http://qg.haigaiapp.cn

================================================================================
来源：http://py.521024.cn

[K01] 对象转 JSON 字符串
来源：http://cq.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ja.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rf.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://ne.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://jv.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mq.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://ie.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zi.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kx.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://gd.hnjuh.cn

Py:   json.loads(s)
来源：http://nx.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://my.hahajie.cn

JS:   JSON.parse(s)
来源：http://iv.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ak.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ic.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://hs.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://yc.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://py.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wa.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rw.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qk.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hx.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uw.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ve.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pc.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lp.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://du.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://gr.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oo.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tu.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://og.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ac.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rw.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cl.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iv.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://xd.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ce.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://fr.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://ah.gzmigu.cn

TS:   structuredClone(obj)
来源：http://kk.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oy.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ju.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xx.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ku.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://wv.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gw.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ki.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ih.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yd.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yt.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://li.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ao.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lw.bookmarksfly.cn

[K07] 进制转换
来源：http://ln.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://po.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nd.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iz.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oq.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zd.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bx.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ur.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fz.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://rg.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://qq.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ul.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://vf.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://bt.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dt.asd995.cn

Go:   encoding/gob
来源：http://hy.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://mj.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cw.huanxung.cn

================================================================================
来源：http://sn.huixiangedu.cn

L. 网络请求
来源：http://fl.szsharing.cn

================================================================================
来源：http://ko.gzmigu.cn

[L01] 发送 GET 请求
来源：http://st.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vo.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ul.colortex.cn

JS:   await fetch(url)
来源：http://cu.chemitech.net.cn

TS:   await fetch(url)
来源：http://mr.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yl.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://ow.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://il.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xq.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ji.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yi.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rs.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://af.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zb.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ib.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xr.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dm.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bw.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://pn.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zb.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zv.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gy.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bx.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hl.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zq.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fa.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yu.yuntaijiaju.cn

[L04] 设置超时
来源：http://rg.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://na.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xo.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cj.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lg.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zj.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ny.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wa.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://zq.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ue.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lu.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wt.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yp.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://os.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tc.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zr.colortex.cn

[L06] 解析响应为 JSON
来源：http://yi.huixiangedu.cn

Py:   resp.json()
来源：http://uf.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://au.nszjky.cn

JS:   await resp.json()
来源：http://pn.szxytkj.cn

TS:   await resp.json()
来源：http://sm.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tg.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ai.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://ih.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rz.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://hz.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sj.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ee.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://pb.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://nq.muxihuayi.cn

Java: resp.statusCode()
来源：http://vi.wgjwhj.cn

Go:   resp.StatusCode
来源：http://fc.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ag.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://la.lnxyls.cn

[L08] 并发请求多个地址
来源：http://ke.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hk.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://qb.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zm.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pj.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vz.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qr.shxzskj.cn


<!-- 参考信息 -->