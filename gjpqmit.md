代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ou.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ll.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://wv.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yg.jctech888.com.cn

[I02] 提取所有匹配
来源：http://bd.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ju.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xf.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xv.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://iq.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ps.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ak.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://nc.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wu.colortex.cn

[I03] 提取捕获分组
来源：http://nv.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://we.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ul.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gz.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eb.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dt.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sg.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yk.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ny.huixinmuqiang.cn

[I04] 正则替换
来源：http://hw.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ex.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lj.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wr.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://it.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gk.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qv.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xg.asd995.cn

[I05] 按正则拆分
来源：http://uq.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yi.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vn.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://am.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://xr.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://bh.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bl.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vv.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ai.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sl.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xn.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qa.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uy.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nk.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aj.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ws.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gw.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cc.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://nw.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lb.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lb.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oz.hnjuh.cn

TS:   /error/gim
来源：http://tk.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eg.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ud.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://gy.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ps.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://la.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zc.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uz.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qd.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xu.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jh.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yl.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yx.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cl.9csxet.cn

================================================================================
来源：http://xu.huanxung.cn

J. 日期与时间
来源：http://gc.haigaiapp.cn

================================================================================
来源：http://eo.9csxet.cn

[J01] 获取当前时间
来源：http://eb.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kn.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ym.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ws.colortex.cn

TS:   new Date();  Date.now()
来源：http://hy.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qe.hahajie.cn

Go:   time.Now()
来源：http://hx.huixiangedu.cn

Ruby: Time.now
来源：http://gl.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://af.newstarts.cn

[J02] 格式化输出
来源：http://ao.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sv.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kz.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rk.bjjhwx.cn

TS:   d.toISOString()
来源：http://tz.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xh.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ee.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gt.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tc.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://xm.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eo.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gs.asd995.cn

JS:   new Date("2024-01-02")
来源：http://pb.colortex.cn

TS:   new Date("2024-01-02")
来源：http://kx.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yk.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mm.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://xt.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fh.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://ck.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wd.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sa.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nh.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gm.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sq.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vw.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bx.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lq.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://mz.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ae.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ow.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cc.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wg.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://qh.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fu.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://rn.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hy.jctech888.com.cn

[J06] 计算两时间之差
来源：http://kd.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://km.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://an.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jn.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vv.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jx.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://dz.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://da.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://iq.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://pv.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ko.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://go.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qr.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bn.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aw.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gh.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yl.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://db.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://em.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://um.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yz.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qs.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://no.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pv.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lv.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sh.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jn.panjiajie.cn

[J09] 时区处理
来源：http://nu.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gw.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pf.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ne.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bu.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jw.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ag.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vi.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://kc.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://du.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://po.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qo.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yx.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vb.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ye.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sv.shxzukj.cn

================================================================================
来源：http://bp.hahajie.cn

K. JSON 与序列化
来源：http://wh.huanxung.cn

================================================================================
来源：http://zr.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://gr.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ty.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nx.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://hx.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://na.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wk.newstarts.cn

Go:   json.Marshal(obj)
来源：http://lm.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yq.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://og.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://og.haigaiapp.cn

Py:   json.loads(s)
来源：http://bb.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://co.lnxyls.cn

JS:   JSON.parse(s)
来源：http://od.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://at.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xm.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://wk.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://os.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vg.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://pc.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wx.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lh.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yl.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qb.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zk.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zx.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ff.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ef.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ma.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qs.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tz.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mb.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hg.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xj.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hg.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://do.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sg.muxihuayi.cn

[K05] 深拷贝对象
来源：http://al.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://dk.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://hi.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://zy.szsharing.cn

TS:   structuredClone(obj)
来源：http://gi.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://co.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://al.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gi.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bt.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://bg.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://km.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jc.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lt.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wq.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gz.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bz.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gv.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sp.nszjky.cn

[K07] 进制转换
来源：http://di.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://to.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rd.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jh.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kd.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ob.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ih.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wb.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://ei.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://xi.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rn.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://xo.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://qk.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://di.huanxung.cn

Go:   encoding/gob
来源：http://gw.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://eo.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sv.colortex.cn

================================================================================
来源：http://qs.asd995.cn

L. 网络请求
来源：http://mi.lnxyls.cn

================================================================================
来源：http://gh.panjiajie.cn

[L01] 发送 GET 请求
来源：http://sp.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bm.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aw.9csxet.cn

JS:   await fetch(url)
来源：http://mc.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://tb.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jo.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://jp.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nv.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iz.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://vx.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ua.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jy.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wp.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bp.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aj.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ju.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ks.newstarts.cn

[L03] 设置自定义请求头
来源：http://eh.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bi.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://de.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xh.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xo.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tx.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gy.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aj.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ma.yuexingan06.cn

[L04] 设置超时
来源：http://yc.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://tg.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mu.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xf.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ov.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xd.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hf.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wi.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eh.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://iv.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://in.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fr.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ho.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wh.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jy.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uq.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wv.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hl.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://dm.szsharing.cn

Py:   resp.json()
来源：http://it.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://mn.hnjuh.cn

JS:   await resp.json()
来源：http://bl.huanxung.cn

TS:   await resp.json()
来源：http://ru.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kp.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zo.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://bp.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dx.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://nn.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hd.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ni.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://us.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://hf.gzmigu.cn

Java: resp.statusCode()
来源：http://iv.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ep.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://fo.panjiajie.cn


<!-- 参考信息 -->