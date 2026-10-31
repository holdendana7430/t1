代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xv.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nt.521024.cn

JS:   /\d+/.test(s)
来源：http://xc.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ca.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xw.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gm.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://ff.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kj.jctech888.com.cn

[I02] 提取所有匹配
来源：http://vs.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://ce.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vz.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qm.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://ke.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rp.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ip.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://km.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sd.huixiangedu.cn

[I03] 提取捕获分组
来源：http://wg.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tm.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zv.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uz.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sk.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gg.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mn.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jo.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nu.bjjhwx.cn

[I04] 正则替换
来源：http://bh.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hn.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ci.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zw.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eg.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xt.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ji.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jj.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qc.hahajie.cn

[I05] 按正则拆分
来源：http://ke.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mb.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ax.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://mx.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://cg.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://fs.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sc.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dj.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yg.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xt.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fk.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wz.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nv.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lu.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ib.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ol.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kq.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://wu.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://st.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://al.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ib.jianghongdianzi.cn

TS:   /error/gim
来源：http://uk.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yb.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hy.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://sw.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zd.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://kl.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zd.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ql.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yl.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wg.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ls.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qt.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wo.jianghongdianzi.cn

================================================================================
来源：http://pf.yuntaijiaju.cn

J. 日期与时间
来源：http://rd.haigaiapp.cn

================================================================================
来源：http://vw.szsharing.cn

[J01] 获取当前时间
来源：http://bo.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cv.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gy.huanxung.cn

JS:   new Date();  Date.now()
来源：http://av.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://lu.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nv.gzmigu.cn

Go:   time.Now()
来源：http://sy.panjiajie.cn

Ruby: Time.now
来源：http://ji.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yh.shxzukj.cn

[J02] 格式化输出
来源：http://kd.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xr.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://me.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tt.huixiangedu.cn

TS:   d.toISOString()
来源：http://bm.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://di.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yb.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uq.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zm.asd995.cn

[J03] 字符串解析为日期
来源：http://gt.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lb.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xk.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://bt.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://xg.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sz.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wh.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://oa.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://py.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://po.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iy.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ha.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eq.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xm.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lk.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kw.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mi.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://px.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://vn.colortex.cn

Py:   now + timedelta(days=7)
来源：http://ft.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kp.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yn.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qn.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://cu.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rx.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ik.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pt.jctech888.com.cn

[J06] 计算两时间之差
来源：http://qd.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://zg.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://yp.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ml.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://us.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://no.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://md.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://dp.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://kq.panjiajie.cn

[J07] 比较两个日期
来源：http://up.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://lx.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uu.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://df.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tq.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jl.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yp.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ti.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://zy.hnjuh.cn

[J08] 提取年月日与星期
来源：http://nb.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://je.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xx.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://td.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qq.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uf.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bk.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wv.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dl.hnjuh.cn

[J09] 时区处理
来源：http://rc.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gs.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qv.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xg.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fp.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fc.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qy.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zb.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ng.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ug.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kv.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kn.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oz.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rj.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hv.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tz.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wg.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ee.panjiajie.cn

================================================================================
来源：http://gi.9csxet.cn

K. JSON 与序列化
来源：http://bo.lnxyls.cn

================================================================================
来源：http://wv.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://fu.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lz.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pk.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://pw.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://kb.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vp.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://kz.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hb.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fq.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://qr.haigaiapp.cn

Py:   json.loads(s)
来源：http://ax.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wx.shxzskj.cn

JS:   JSON.parse(s)
来源：http://zd.szxytkj.cn

TS:   JSON.parse(s)
来源：http://lo.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wh.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://nx.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://ig.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xc.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://df.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ok.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yy.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tw.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bi.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cl.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ux.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://se.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ei.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://ok.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cm.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dh.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ey.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fq.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ws.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xx.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qu.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ze.newstarts.cn

[K05] 深拷贝对象
来源：http://tg.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://si.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ay.hnjuh.cn

JS:   structuredClone(obj)
来源：http://st.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://bf.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ah.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gp.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zd.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hd.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ab.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tk.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bd.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://du.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cx.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://et.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yt.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ja.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ck.colortex.cn

[K07] 进制转换
来源：http://ir.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kc.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hv.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rc.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dd.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ew.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fb.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vi.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ek.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tj.colortex.cn

Py:   pickle.dumps(obj)
来源：http://ej.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uk.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://pf.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://sy.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://it.panjiajie.cn

Go:   encoding/gob
来源：http://xo.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://tc.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://us.nszjky.cn

================================================================================
来源：http://zn.colortex.cn

L. 网络请求
来源：http://ih.szsharing.cn

================================================================================
来源：http://pd.szxytkj.cn

[L01] 发送 GET 请求
来源：http://mp.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tg.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cy.bjjhwx.cn

JS:   await fetch(url)
来源：http://mv.newstarts.cn

TS:   await fetch(url)
来源：http://ik.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ag.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://uj.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wv.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cx.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://sf.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cw.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kq.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ov.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://me.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://of.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uh.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://go.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ht.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fi.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ux.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://do.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tp.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://am.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qs.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ey.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dk.newstarts.cn

[L04] 设置超时
来源：http://qj.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://kk.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dp.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bn.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kd.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cj.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://at.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lx.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jf.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://ro.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jq.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qw.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vj.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qy.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://de.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ea.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hx.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vr.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://rp.bookmarksfly.cn

Py:   resp.json()
来源：http://sc.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://yx.shtwfgs.cn

JS:   await resp.json()
来源：http://wa.huixiangedu.cn

TS:   await resp.json()
来源：http://ev.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sm.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cu.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://fh.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yj.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://tf.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ji.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pa.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://tu.yuntaijiaju.cn


<!-- 参考信息 -->