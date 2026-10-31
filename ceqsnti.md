代发 wailian999

[I02] 提取所有匹配
来源：http://hg.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ti.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fh.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yv.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://pw.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eb.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://my.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://qx.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hl.hahajie.cn

[I03] 提取捕获分组
来源：http://rk.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zj.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sy.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vq.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ai.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jx.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://za.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bp.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jn.szxytkj.cn

[I04] 正则替换
来源：http://mo.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ey.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pi.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oy.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lf.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hq.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cv.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ta.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://os.colortex.cn

[I05] 按正则拆分
来源：http://yw.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://se.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ja.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://kg.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://yw.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://ku.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xb.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ub.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xs.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://va.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eg.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ja.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bp.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vv.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jj.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ow.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cr.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dd.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ql.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sp.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ni.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kc.yuntaijiaju.cn

TS:   /error/gim
来源：http://ws.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wh.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nw.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://fz.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gl.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://mp.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iu.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gd.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://es.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yr.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cb.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xp.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vh.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ov.huanxung.cn

================================================================================
来源：http://qf.jianghongdianzi.cn

J. 日期与时间
来源：http://lb.huixinmuqiang.cn

================================================================================
来源：http://wt.bjjhwx.cn

[J01] 获取当前时间
来源：http://nq.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vg.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tw.huanxung.cn

JS:   new Date();  Date.now()
来源：http://he.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://gv.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ib.huanxung.cn

Go:   time.Now()
来源：http://kg.hahajie.cn

Ruby: Time.now
来源：http://oa.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pm.wgjwhj.cn

[J02] 格式化输出
来源：http://ze.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vy.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zg.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aq.huixiangedu.cn

TS:   d.toISOString()
来源：http://iq.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://es.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ok.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mc.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kj.huanxung.cn

[J03] 字符串解析为日期
来源：http://we.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ec.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://th.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://mm.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://gw.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gj.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eg.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://fi.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eb.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://wi.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gu.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qh.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wm.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ic.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oa.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yx.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nf.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aa.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://kn.521024.cn

Py:   now + timedelta(days=7)
来源：http://pl.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ol.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vn.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://tz.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jr.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://hf.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://th.9csxet.cn

[J06] 计算两时间之差
来源：http://vr.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://zy.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://uz.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kl.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ym.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wa.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://xq.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ao.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://vy.lnxyls.cn

[J07] 比较两个日期
来源：http://dm.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://cm.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fp.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qr.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vz.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tk.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qo.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bm.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://fz.szsharing.cn

[J08] 提取年月日与星期
来源：http://rf.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ni.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wz.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cz.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wp.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mm.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fx.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gr.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kz.szsharing.cn

[J09] 时区处理
来源：http://mx.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ak.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nk.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uw.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://av.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hw.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pm.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bd.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wq.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://rr.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ef.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kx.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ad.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wx.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xm.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hw.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://td.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bw.hahajie.cn

================================================================================
来源：http://rj.muxihuayi.cn

K. JSON 与序列化
来源：http://aj.9csxet.cn

================================================================================
来源：http://sv.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://cw.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qg.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mj.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://wl.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://ed.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lz.colortex.cn

Go:   json.Marshal(obj)
来源：http://rh.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dk.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gm.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://ya.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://qx.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wm.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ip.shxzukj.cn

TS:   JSON.parse(s)
来源：http://sp.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ip.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://bm.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://gf.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ro.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ei.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hl.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kp.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://at.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rx.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fx.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oa.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://et.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://rf.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xi.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dj.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://td.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ve.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ao.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nl.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://es.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://td.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://po.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ph.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://av.nicolike.cn

JS:   structuredClone(obj)
来源：http://qw.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://ld.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cu.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ug.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ev.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://og.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://uc.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jk.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zq.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lm.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://az.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ok.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ik.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vt.hnjuh.cn

[K07] 进制转换
来源：http://dn.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://on.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rd.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kc.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iw.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fd.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nb.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jy.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fc.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://tz.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://zg.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ts.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://qg.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://ge.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ux.gzmigu.cn

Go:   encoding/gob
来源：http://if.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://tu.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ko.521024.cn

================================================================================
来源：http://jg.huanxung.cn

L. 网络请求
来源：http://uo.colortex.cn

================================================================================
来源：http://jk.panjiajie.cn

[L01] 发送 GET 请求
来源：http://wm.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pm.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jo.newstarts.cn

JS:   await fetch(url)
来源：http://qo.panjiajie.cn

TS:   await fetch(url)
来源：http://ad.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xz.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://gn.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cb.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ub.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://fm.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ju.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://co.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mx.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hm.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ky.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://co.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ko.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sk.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pf.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bk.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gk.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ir.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ky.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uo.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rn.521024.cn

[L04] 设置超时
来源：http://bv.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://bx.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pm.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vu.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sf.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ts.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yz.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uj.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://hw.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ne.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ff.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ud.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pv.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rc.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://it.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fz.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://of.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://kw.9csxet.cn

Py:   resp.json()
来源：http://vu.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ze.9csxet.cn

JS:   await resp.json()
来源：http://fq.nszjky.cn

TS:   await resp.json()
来源：http://us.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zy.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zo.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://jj.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lv.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://eq.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nk.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gj.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://fa.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://sw.asd995.cn

Java: resp.statusCode()
来源：http://pd.asd995.cn

Go:   resp.StatusCode
来源：http://nh.newstarts.cn

Ruby: resp.code.to_i
来源：http://lf.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://fh.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://kf.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mc.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://nk.jctech888.com.cn


<!-- 参考信息 -->