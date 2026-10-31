代发 wailian999

TS:   s.match(/\d+/g)
来源：http://yl.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eq.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qm.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://sx.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hs.521024.cn

[I03] 提取捕获分组
来源：http://sf.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kk.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://av.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ed.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hn.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xw.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dq.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://as.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hu.huixinmuqiang.cn

[I04] 正则替换
来源：http://yo.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://on.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nr.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gk.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jb.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sr.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xq.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hr.9csxet.cn

[I05] 按正则拆分
来源：http://fh.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tx.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uc.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ir.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://xo.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://la.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fh.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://el.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kp.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://av.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zn.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dj.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fz.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pw.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jw.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ac.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fh.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hd.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://cb.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sc.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://no.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rt.huixinmuqiang.cn

TS:   /error/gim
来源：http://zd.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xv.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wa.521024.cn

Ruby: s.scan(/error/i)
来源：http://bs.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wt.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://uv.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wg.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ah.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gh.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ik.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://la.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qx.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rf.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://li.bjjhwx.cn

================================================================================
来源：http://tm.shxzukj.cn

J. 日期与时间
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://fs.521024.cn

[J01] 获取当前时间
来源：http://mr.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oh.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://le.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://wi.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://yb.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tk.nicolike.cn

Go:   time.Now()
来源：http://vg.shtwfgs.cn

Ruby: Time.now
来源：http://ae.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ez.hahajie.cn

[J02] 格式化输出
来源：http://hv.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lb.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kr.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tj.9csxet.cn

TS:   d.toISOString()
来源：http://xq.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gt.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://by.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zl.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://dl.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uo.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qx.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://se.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://zf.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://my.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mw.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://gt.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ie.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://nr.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ku.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hx.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nu.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sm.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vm.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cj.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://co.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gb.521024.cn

[J05] 时间加减（加 7 天）
来源：http://in.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://vi.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dj.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lo.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oj.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ek.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ki.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://lm.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xb.haigaiapp.cn

[J06] 计算两时间之差
来源：http://he.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://qq.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://ui.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://he.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://af.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ic.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://iv.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://gk.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://ji.hnjuh.cn

[J07] 比较两个日期
来源：http://lh.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://em.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dg.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zb.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sd.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ha.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://um.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://so.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://nv.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://kv.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nt.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xo.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nx.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yk.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oo.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eg.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ra.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uq.bjjhwx.cn

[J09] 时区处理
来源：http://jc.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bk.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tb.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wb.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bx.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xd.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fy.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ua.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tg.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://ns.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://re.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://by.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://my.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cm.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bg.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ha.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wh.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lh.panjiajie.cn

================================================================================
来源：http://vz.hnjuh.cn

K. JSON 与序列化
来源：http://mc.panjiajie.cn

================================================================================
来源：http://lr.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://qa.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gb.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xg.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://sj.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://tz.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vj.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://dm.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tw.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vc.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ke.szsharing.cn

Py:   json.loads(s)
来源：http://mg.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rj.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://bc.nicolike.cn

TS:   JSON.parse(s)
来源：http://qj.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rl.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://vi.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://yv.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gs.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://td.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ni.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vy.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rw.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://py.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zl.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gr.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dc.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jc.huanxung.cn

[K04] 读取 JSON 文件
来源：http://yv.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wi.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ua.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ev.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zu.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tc.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hh.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gf.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mj.chemitech.net.cn

[K05] 深拷贝对象
来源：http://nf.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ys.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://xe.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://wo.colortex.cn

TS:   structuredClone(obj)
来源：http://qg.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yo.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jr.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ap.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ea.colortex.cn

[K06] 解析 URL 查询串
来源：http://pf.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cc.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rl.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xz.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zt.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jv.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://da.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://of.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jo.hahajie.cn

[K07] 进制转换
来源：http://om.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nu.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ly.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ie.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rp.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dw.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pu.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tg.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ol.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://wa.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://fu.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xk.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://do.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ia.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oo.muxihuayi.cn

Go:   encoding/gob
来源：http://wv.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://ds.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vr.nszjky.cn

================================================================================
来源：http://yg.hnjuh.cn

L. 网络请求
来源：http://eo.nszjky.cn

================================================================================
来源：http://jr.shxzskj.cn

[L01] 发送 GET 请求
来源：http://vb.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fq.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tk.yuexingan06.cn

JS:   await fetch(url)
来源：http://uk.panjiajie.cn

TS:   await fetch(url)
来源：http://cp.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dq.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ii.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kh.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://id.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ix.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ut.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ff.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hq.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ju.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ze.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xx.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uf.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bl.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://mz.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zf.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rw.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://br.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kw.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xg.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kc.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uq.huixiangedu.cn

[L04] 设置超时
来源：http://np.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://vn.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wg.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dw.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fs.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yo.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zu.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iq.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://ps.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://on.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kt.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tv.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ig.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wy.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hn.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qh.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://mj.huixiangedu.cn

Py:   resp.json()
来源：http://df.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://pk.haigaiapp.cn

JS:   await resp.json()
来源：http://nr.muxihuayi.cn

TS:   await resp.json()
来源：http://ck.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vi.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tp.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://bi.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xo.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ab.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qd.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fc.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://if.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://lq.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://og.wgjwhj.cn

Go:   resp.StatusCode
来源：http://kh.huanxung.cn

Ruby: resp.code.to_i
来源：http://qy.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://id.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://nd.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fl.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://fq.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wk.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://op.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yv.huixinmuqiang.cn


<!-- 参考信息 -->