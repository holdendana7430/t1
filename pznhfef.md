代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fq.bjjhwx.cn

[I03] 提取捕获分组
来源：http://uc.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gc.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bn.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://po.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bb.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eh.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nn.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zr.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ae.newstarts.cn

[I04] 正则替换
来源：http://zw.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bu.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://im.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oz.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://we.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://di.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ee.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xs.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uu.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://he.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ee.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jo.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://zd.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://sa.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://gn.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kj.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gv.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yr.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qq.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vh.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ys.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ef.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bd.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ng.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ax.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yb.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cn.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://dt.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cw.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://si.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kg.hnjuh.cn

TS:   /error/gim
来源：http://vy.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sc.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vh.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ra.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sm.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://gt.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gs.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ys.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zl.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jl.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yj.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xy.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nt.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yk.gzmigu.cn

================================================================================
来源：http://nm.panjiajie.cn

J. 日期与时间
来源：http://il.hahajie.cn

================================================================================
来源：http://mt.bookmarksfly.cn

[J01] 获取当前时间
来源：http://qn.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://so.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dz.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ph.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://qr.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sj.shxzukj.cn

Go:   time.Now()
来源：http://ym.bookmarksfly.cn

Ruby: Time.now
来源：http://sw.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vb.9csxet.cn

[J02] 格式化输出
来源：http://rx.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jr.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tf.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dg.lnxyls.cn

TS:   d.toISOString()
来源：http://tx.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ej.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ln.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sl.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vg.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://mv.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zy.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iq.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://sn.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ds.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wt.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hf.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://us.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cr.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://gj.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kc.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jk.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vm.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jq.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iq.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vo.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wq.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hx.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://pz.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://bn.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wc.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ic.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nr.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://gb.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vp.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://ad.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://in.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://cp.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mn.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rm.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hg.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://gx.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://so.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ap.bookmarksfly.cn

[J07] 比较两个日期
来源：http://tu.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://ts.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bt.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wl.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mi.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://op.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://px.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tp.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://vh.asd995.cn

[J08] 提取年月日与星期
来源：http://wu.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fu.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mw.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tw.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zb.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://py.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://te.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sh.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kg.panjiajie.cn

[J09] 时区处理
来源：http://xp.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mw.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gf.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ov.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nz.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://py.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tu.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kn.521024.cn

[J10] 取今天 / 本月第一天
来源：http://ow.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dy.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ow.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pg.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://io.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wm.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oo.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wb.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://id.asd995.cn

================================================================================
来源：http://oq.yuexingan06.cn

K. JSON 与序列化
来源：http://qe.szxytkj.cn

================================================================================
来源：http://ng.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://vf.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://at.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qa.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ab.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://tn.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ud.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://wf.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hj.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uw.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://do.asd995.cn

Py:   json.loads(s)
来源：http://hz.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xm.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ij.9csxet.cn

TS:   JSON.parse(s)
来源：http://vk.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ms.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://de.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://cl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fe.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://et.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xv.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nl.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zr.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qs.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hr.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gi.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kn.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://up.newstarts.cn

[K04] 读取 JSON 文件
来源：http://gc.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ro.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zd.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pn.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fs.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lt.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ab.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qz.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ee.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://by.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://fk.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://fu.colortex.cn

JS:   structuredClone(obj)
来源：http://uz.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://hl.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gi.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ny.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ay.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ae.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://le.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yi.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cw.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zz.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wr.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oy.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uf.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wf.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zy.bookmarksfly.cn

[K07] 进制转换
来源：http://fo.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tp.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hq.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nj.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ww.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wz.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ad.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hq.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xh.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ts.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://vj.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lm.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mb.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://im.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pb.jctech888.com.cn

Go:   encoding/gob
来源：http://os.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ls.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ls.jctech888.com.cn

================================================================================
来源：http://yj.huanxung.cn

L. 网络请求
来源：http://bj.shtwfgs.cn

================================================================================
来源：http://rn.asd995.cn

[L01] 发送 GET 请求
来源：http://aq.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yb.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xx.panjiajie.cn

JS:   await fetch(url)
来源：http://jb.hnjuh.cn

TS:   await fetch(url)
来源：http://ku.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ko.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://xb.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qq.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ay.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ou.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vi.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ps.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://re.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ny.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mp.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kw.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://it.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://it.szxytkj.cn

[L03] 设置自定义请求头
来源：http://tv.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mf.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lm.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xw.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zr.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kc.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://et.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ks.gzmigu.cn

[L04] 设置超时
来源：http://os.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://dq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ye.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jy.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vn.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mk.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://po.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://hg.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://av.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ck.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lq.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bk.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aw.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nc.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://hz.newstarts.cn

Py:   resp.json()
来源：http://ol.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ej.shtwfgs.cn

JS:   await resp.json()
来源：http://gs.gzmigu.cn

TS:   await resp.json()
来源：http://ga.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oq.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hr.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ip.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://io.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://jq.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pi.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://at.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://uu.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://ns.nicolike.cn

Java: resp.statusCode()
来源：http://rd.hahajie.cn

Go:   resp.StatusCode
来源：http://qi.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://yl.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://xj.hahajie.cn

[L08] 并发请求多个地址
来源：http://xv.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dz.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://dk.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oy.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ve.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sl.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lo.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jt.hnjuh.cn

================================================================================
来源：http://ek.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ur.szxytkj.cn


<!-- 参考信息 -->