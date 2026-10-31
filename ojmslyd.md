代发 wailian999

[I02] 提取所有匹配
来源：http://fa.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://bo.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bp.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ps.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://fb.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xy.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sy.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://ta.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ed.yuexingan06.cn

[I03] 提取捕获分组
来源：http://js.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xc.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qj.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wb.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xf.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nf.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xx.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fn.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vt.jianghongdianzi.cn

[I04] 正则替换
来源：http://of.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lk.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nm.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ud.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://px.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rz.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nh.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mv.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uy.shxzukj.cn

[I05] 按正则拆分
来源：http://fz.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qs.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tc.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://no.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://kz.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://kh.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qk.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zt.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tz.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cf.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fu.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sa.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gm.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ci.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ez.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bk.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hu.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nc.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://nf.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aj.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yf.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jc.521024.cn

TS:   /error/gim
来源：http://wj.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nw.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hf.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://mo.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gd.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://oh.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mh.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qw.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oc.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pq.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yz.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pq.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jq.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://am.9csxet.cn

================================================================================
来源：http://mj.szsharing.cn

J. 日期与时间
来源：http://hv.hnjuh.cn

================================================================================
来源：http://rz.asd995.cn

[J01] 获取当前时间
来源：http://zm.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yh.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rw.521024.cn

JS:   new Date();  Date.now()
来源：http://tr.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ae.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tt.hahajie.cn

Go:   time.Now()
来源：http://ab.haigaiapp.cn

Ruby: Time.now
来源：http://qh.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ox.shxzskj.cn

[J02] 格式化输出
来源：http://pi.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xa.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wn.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jk.lnxyls.cn

TS:   d.toISOString()
来源：http://wr.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mo.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dd.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ev.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aw.szxytkj.cn

[J03] 字符串解析为日期
来源：http://la.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://du.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lb.asd995.cn

JS:   new Date("2024-01-02")
来源：http://wx.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://uc.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ok.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://en.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://lb.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vx.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://hu.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://om.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://or.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tj.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ut.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sd.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fw.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vl.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kz.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://qx.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://te.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ac.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qa.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rk.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ar.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ti.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://nv.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://li.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ul.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://vv.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ii.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vi.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://xx.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://zw.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://ji.jctech888.com.cn

[J07] 比较两个日期
来源：http://sf.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://ol.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qt.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fi.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hu.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gm.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xj.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mv.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://uz.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://kd.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://om.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ni.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mw.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mm.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lj.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://is.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eh.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qt.nszjky.cn

[J09] 时区处理
来源：http://ps.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yu.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ub.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pd.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jb.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ld.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ej.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wc.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://qx.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zr.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tk.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nk.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pt.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jq.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yc.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dv.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zq.nszjky.cn

================================================================================
来源：http://tu.huixiangedu.cn

K. JSON 与序列化
来源：http://kb.jianghongdianzi.cn

================================================================================
来源：http://qo.521024.cn

[K01] 对象转 JSON 字符串
来源：http://uk.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uh.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rz.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://nw.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://si.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iv.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://we.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nx.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yj.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://oy.chemitech.net.cn

Py:   json.loads(s)
来源：http://cz.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hn.gzmigu.cn

JS:   JSON.parse(s)
来源：http://yj.nszjky.cn

TS:   JSON.parse(s)
来源：http://iq.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yw.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ub.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://dm.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://et.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://sl.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sr.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fz.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ak.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vj.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://io.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vj.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oy.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ty.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zc.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://au.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cc.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://me.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bv.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yw.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cd.shtwfgs.cn

[K05] 深拷贝对象
来源：http://sb.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://de.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://es.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://zf.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://dv.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lw.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bk.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nz.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hg.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://nl.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ev.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sw.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pg.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wl.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ub.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gc.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lw.yuntaijiaju.cn

[K07] 进制转换
来源：http://jz.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tl.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qe.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zf.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mc.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gn.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cp.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bj.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fe.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://yp.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://bx.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nj.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cq.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://fw.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ow.9csxet.cn

Go:   encoding/gob
来源：http://qb.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://is.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sj.yuntaijiaju.cn

================================================================================
来源：http://bn.bookmarksfly.cn

L. 网络请求
来源：http://gy.hnjuh.cn

================================================================================
来源：http://pe.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ej.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dq.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rr.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://sp.chemitech.net.cn

TS:   await fetch(url)
来源：http://ah.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pl.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://he.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cd.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qd.9csxet.cn

[L02] 发送 POST JSON
来源：http://td.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://af.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dh.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ig.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gc.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jy.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hg.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ud.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rl.huanxung.cn

[L03] 设置自定义请求头
来源：http://wg.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fb.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ih.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ii.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fx.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xp.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dy.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uj.hahajie.cn

[L04] 设置超时
来源：http://gs.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://hz.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hc.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hv.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cj.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rp.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vz.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zj.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://df.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://qb.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yz.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vc.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bw.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dl.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yl.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fv.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yo.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://np.asd995.cn

[L06] 解析响应为 JSON
来源：http://ks.colortex.cn

Py:   resp.json()
来源：http://uu.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://hk.9csxet.cn

JS:   await resp.json()
来源：http://bb.huixinmuqiang.cn

TS:   await resp.json()
来源：http://hv.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jy.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ja.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://bu.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gp.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://lr.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bc.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qi.521024.cn

JS:   resp.ok;  resp.status
来源：http://ok.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://cg.haigaiapp.cn

Java: resp.statusCode()
来源：http://zo.newstarts.cn

Go:   resp.StatusCode
来源：http://zz.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://io.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://oc.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://sv.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bp.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://tz.nszjky.cn


<!-- 参考信息 -->