代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ut.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cz.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://bj.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vx.jctech888.com.cn

[I02] 提取所有匹配
来源：http://zk.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://mi.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hb.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zz.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://qk.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pk.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sg.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://uu.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mk.bjjhwx.cn

[I03] 提取捕获分组
来源：http://lx.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qx.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pk.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qw.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lx.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mc.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://se.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wg.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://er.chemitech.net.cn

[I04] 正则替换
来源：http://gw.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zw.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://to.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nn.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vw.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://au.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uf.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ea.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ea.panjiajie.cn

[I05] 按正则拆分
来源：http://qs.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qg.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://na.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://th.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://ak.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://ey.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jx.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ca.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aj.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lq.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://np.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yx.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wc.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rq.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://je.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rr.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://de.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gx.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://hk.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wk.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://by.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fc.nszjky.cn

TS:   /error/gim
来源：http://fb.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mw.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jd.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://cf.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fk.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://wf.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rf.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://od.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ce.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cz.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lh.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ou.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bq.shxzskj.cn

================================================================================
来源：http://iy.haigaiapp.cn

J. 日期与时间
来源：http://ne.szxytkj.cn

================================================================================
来源：http://jg.hnjuh.cn

[J01] 获取当前时间
来源：http://ho.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zv.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gr.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://kp.szsharing.cn

TS:   new Date();  Date.now()
来源：http://uu.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cx.nszjky.cn

Go:   time.Now()
来源：http://ti.yuexingan06.cn

Ruby: Time.now
来源：http://wi.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oc.muxihuayi.cn

[J02] 格式化输出
来源：http://es.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://og.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hs.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ws.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://wp.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wf.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qt.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ne.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ae.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://qa.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hv.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pf.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://zn.asd995.cn

TS:   new Date("2024-01-02")
来源：http://pk.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eb.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hh.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://vp.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dc.nszjky.cn

[J04] 时间戳与日期互转
来源：http://nr.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yv.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ln.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ez.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hg.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vt.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wi.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rs.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dl.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://xa.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ib.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jj.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uf.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ne.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://yq.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vb.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://bd.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jt.wgjwhj.cn

[J06] 计算两时间之差
来源：http://hk.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://rh.521024.cn

PHP:  $end->diff($start)->days;
来源：http://xh.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ze.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bn.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oa.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ae.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ir.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://sb.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://mp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://hz.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gx.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kr.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ji.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tw.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ji.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mz.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://aj.huanxung.cn

[J08] 提取年月日与星期
来源：http://hp.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ab.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://an.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nw.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mf.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mh.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dn.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kq.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nj.szxytkj.cn

[J09] 时区处理
来源：http://iv.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ec.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kg.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kb.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pe.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tq.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mv.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rm.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mx.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://hg.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://od.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mv.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://us.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dw.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ws.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gs.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bg.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wo.shxzukj.cn

================================================================================
来源：http://ya.hahajie.cn

K. JSON 与序列化
来源：http://jy.521024.cn

================================================================================
来源：http://pv.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://az.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qc.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zb.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://qt.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://qg.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zq.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ox.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xy.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://nu.gzmigu.cn

Py:   json.loads(s)
来源：http://wc.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fw.colortex.cn

JS:   JSON.parse(s)
来源：http://ct.colortex.cn

TS:   JSON.parse(s)
来源：http://ys.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ih.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://lz.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://uw.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eq.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://br.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rc.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ky.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ig.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kw.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jo.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qw.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ao.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oi.nszjky.cn

[K04] 读取 JSON 文件
来源：http://wa.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ac.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zm.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kk.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ou.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rk.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://em.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rb.shxzukj.cn

[K05] 深拷贝对象
来源：http://gy.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://rg.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://pm.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://zu.colortex.cn

TS:   structuredClone(obj)
来源：http://hi.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dj.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ri.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tk.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wp.szsharing.cn

[K06] 解析 URL 查询串
来源：http://wv.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zq.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://il.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://at.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vi.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ji.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bv.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xl.lnxyls.cn

[K07] 进制转换
来源：http://jl.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ue.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oh.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bz.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pl.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://or.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qf.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ok.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://km.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://gb.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://bu.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sv.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://vd.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://sm.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://je.colortex.cn

Go:   encoding/gob
来源：http://xl.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://di.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dv.gzmigu.cn

================================================================================
来源：http://ph.nicolike.cn

L. 网络请求
来源：http://sl.shtwfgs.cn

================================================================================
来源：http://qm.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ip.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jx.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://na.newstarts.cn

JS:   await fetch(url)
来源：http://el.bjjhwx.cn

TS:   await fetch(url)
来源：http://xt.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qq.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://ds.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uz.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fv.lnxyls.cn

[L02] 发送 POST JSON
来源：http://ow.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://in.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bu.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gz.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ca.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fl.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ci.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xa.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bm.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://vj.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aj.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dv.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aq.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fv.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jt.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mp.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sx.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cy.hahajie.cn

[L04] 设置超时
来源：http://th.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://vj.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ub.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qp.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lp.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://un.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cp.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ez.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sy.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://mt.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qh.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ca.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ia.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ac.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mf.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://or.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zf.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://io.szsharing.cn

[L06] 解析响应为 JSON
来源：http://bx.jctech888.com.cn

Py:   resp.json()
来源：http://hz.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://qm.colortex.cn

JS:   await resp.json()
来源：http://ur.jianghongdianzi.cn

TS:   await resp.json()
来源：http://ap.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qh.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gi.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://nn.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lq.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://ou.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yw.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ui.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://jc.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://tp.9csxet.cn

Java: resp.statusCode()
来源：http://nc.521024.cn

Go:   resp.StatusCode
来源：http://xw.lnxyls.cn

Ruby: resp.code.to_i
来源：http://is.521024.cn


<!-- 参考信息 -->