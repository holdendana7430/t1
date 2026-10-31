代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lq.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://qr.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://so.jctech888.com.cn

[I02] 提取所有匹配
来源：http://vl.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://zn.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gn.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zw.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://bb.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xb.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sk.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://mm.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://so.szxytkj.cn

[I03] 提取捕获分组
来源：http://wt.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://za.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fp.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ug.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ku.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nn.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xt.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yo.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gn.colortex.cn

[I04] 正则替换
来源：http://qu.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://od.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xc.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rh.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://um.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ez.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ef.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wl.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rl.shxzskj.cn

[I05] 按正则拆分
来源：http://qd.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ph.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kc.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://ie.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://cg.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://js.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wt.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dl.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kv.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ej.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://py.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ho.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ck.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gn.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ej.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eg.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wd.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mx.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://fm.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nj.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wd.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hm.muxihuayi.cn

TS:   /error/gim
来源：http://vy.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yt.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dh.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://ft.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lr.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ud.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pi.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fe.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ba.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tt.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vn.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://my.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dq.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hv.panjiajie.cn

================================================================================
来源：http://uh.521024.cn

J. 日期与时间
来源：http://bh.nicolike.cn

================================================================================
来源：http://ic.newstarts.cn

[J01] 获取当前时间
来源：http://aw.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qr.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zg.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://vf.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ex.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ap.jianghongdianzi.cn

Go:   time.Now()
来源：http://fm.shxzukj.cn

Ruby: Time.now
来源：http://wh.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lc.nicolike.cn

[J02] 格式化输出
来源：http://uf.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wy.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dv.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vd.hahajie.cn

TS:   d.toISOString()
来源：http://id.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xi.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ud.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uz.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ap.asd995.cn

[J03] 字符串解析为日期
来源：http://cn.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://im.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zt.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://fv.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://ns.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dg.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sb.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ok.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ug.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://bi.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://te.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zh.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nz.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rb.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ik.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fj.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yn.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://on.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://sa.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://fu.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pu.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pl.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mx.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://sb.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xb.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://mf.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yh.szsharing.cn

[J06] 计算两时间之差
来源：http://ve.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://pu.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://rq.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sy.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hk.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mu.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://dx.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://vy.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://sh.shxzskj.cn

[J07] 比较两个日期
来源：http://nu.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://rx.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hp.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gr.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pj.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://af.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qt.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vj.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://ee.huanxung.cn

[J08] 提取年月日与星期
来源：http://en.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rj.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pm.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bq.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mh.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gt.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ve.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ip.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tk.9csxet.cn

[J09] 时区处理
来源：http://qo.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://px.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ej.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ex.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://up.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vs.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ky.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://an.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jk.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://ur.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uv.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kg.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zc.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zy.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wx.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xr.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mm.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uu.nicolike.cn

================================================================================
来源：http://th.szsharing.cn

K. JSON 与序列化
来源：http://tt.colortex.cn

================================================================================
来源：http://na.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://my.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sk.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hf.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://br.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://lc.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://du.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ah.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yr.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://if.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://bg.jctech888.com.cn

Py:   json.loads(s)
来源：http://lr.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fj.hahajie.cn

JS:   JSON.parse(s)
来源：http://oo.521024.cn

TS:   JSON.parse(s)
来源：http://ea.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rx.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://zs.huanxung.cn

Ruby: JSON.parse(s)
来源：http://zz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ia.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://zf.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fs.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://km.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ce.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ig.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zc.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gq.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bi.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sb.asd995.cn

[K04] 读取 JSON 文件
来源：http://fq.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hx.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://su.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qy.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lv.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ey.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gu.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bu.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bn.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ml.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://pw.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://sb.521024.cn

JS:   structuredClone(obj)
来源：http://ep.9csxet.cn

TS:   structuredClone(obj)
来源：http://lq.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qp.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://um.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hp.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qb.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://hg.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bx.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mr.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wh.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mu.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zu.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ym.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://it.jctech888.com.cn

[K07] 进制转换
来源：http://rv.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ch.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ks.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yb.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sz.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sq.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://md.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lw.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kn.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qj.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://bd.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oc.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://pq.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://gx.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qq.hnjuh.cn

Go:   encoding/gob
来源：http://ac.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://jk.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bf.jctech888.com.cn

================================================================================
来源：http://lu.shtwfgs.cn

L. 网络请求
来源：http://zo.9csxet.cn

================================================================================
来源：http://wv.nicolike.cn

[L01] 发送 GET 请求
来源：http://by.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ah.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xs.huanxung.cn

JS:   await fetch(url)
来源：http://jg.yuexingan06.cn

TS:   await fetch(url)
来源：http://zm.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yj.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://tw.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ec.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uu.521024.cn

[L02] 发送 POST JSON
来源：http://qz.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cl.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xd.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://za.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zn.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xc.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vc.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fi.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wa.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://ed.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hh.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pv.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vw.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ur.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uw.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lb.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xg.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bq.bookmarksfly.cn

[L04] 设置超时
来源：http://ex.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://rf.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bg.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mh.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gl.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hi.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kv.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lz.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xm.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ym.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qd.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://na.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lp.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bx.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ld.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cm.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://us.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bt.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://kq.jctech888.com.cn

Py:   resp.json()
来源：http://pm.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://bp.shxzukj.cn

JS:   await resp.json()
来源：http://vq.9csxet.cn

TS:   await resp.json()
来源：http://rc.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gz.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://da.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://xq.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wf.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://cr.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wu.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kd.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://ua.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://sr.huanxung.cn

Java: resp.statusCode()
来源：http://db.newstarts.cn

Go:   resp.StatusCode
来源：http://vd.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://xy.shxzukj.cn


<!-- 参考信息 -->