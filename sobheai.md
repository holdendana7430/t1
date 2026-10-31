代发 wailian999

================================================================================
来源：http://bl.szsharing.cn

I. 正则表达式
来源：http://tk.nicolike.cn

================================================================================
来源：http://iu.chemitech.net.cn

[I01] 判断是否匹配
来源：http://os.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kp.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fo.9csxet.cn

JS:   /\d+/.test(s)
来源：http://bk.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://ae.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wo.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rf.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://mr.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fu.huixiangedu.cn

[I02] 提取所有匹配
来源：http://az.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://km.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xn.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ar.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://mj.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jq.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ee.521024.cn

Ruby: s.scan(/\d+/)
来源：http://az.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lf.jctech888.com.cn

[I03] 提取捕获分组
来源：http://im.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lm.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ff.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mc.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pn.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mk.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zs.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ac.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oy.huanxung.cn

[I04] 正则替换
来源：http://xs.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://if.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tf.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://um.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qv.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cb.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mb.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://og.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yi.szsharing.cn

[I05] 按正则拆分
来源：http://bt.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://un.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nj.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://bb.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://jm.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://on.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ug.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kd.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nu.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xt.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://na.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pb.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vo.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vo.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eh.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ai.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tx.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kj.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://qh.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bl.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dp.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sd.chemitech.net.cn

TS:   /error/gim
来源：http://wq.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rb.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rp.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://dr.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ph.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://ea.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oi.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bw.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vk.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rf.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ek.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://to.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xp.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bt.jctech888.com.cn

================================================================================
来源：http://pw.yuntaijiaju.cn

J. 日期与时间
来源：http://in.bjjhwx.cn

================================================================================
来源：http://nu.colortex.cn

[J01] 获取当前时间
来源：http://qr.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hm.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://be.521024.cn

JS:   new Date();  Date.now()
来源：http://br.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://pz.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ns.yuntaijiaju.cn

Go:   time.Now()
来源：http://wb.szsharing.cn

Ruby: Time.now
来源：http://vo.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ou.hnjuh.cn

[J02] 格式化输出
来源：http://gx.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wb.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ht.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ow.panjiajie.cn

TS:   d.toISOString()
来源：http://xf.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zw.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mi.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hs.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vj.9csxet.cn

[J03] 字符串解析为日期
来源：http://gd.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fk.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nz.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://ma.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://gs.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mc.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qo.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://qx.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yv.huanxung.cn

[J04] 时间戳与日期互转
来源：http://fs.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://io.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hd.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rx.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ob.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yv.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xa.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wy.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://br.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ju.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://so.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ui.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mi.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qk.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://hp.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dw.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://qc.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vr.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://xl.521024.cn

Py:   (end - start).total_seconds()
来源：http://xz.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://jx.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ov.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zv.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yo.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://gu.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hr.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://yt.bjjhwx.cn

[J07] 比较两个日期
来源：http://jl.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://dp.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uh.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ud.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ow.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ml.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bj.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cf.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://vq.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://nf.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tu.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vw.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kk.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jq.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ty.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://de.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qd.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fd.lnxyls.cn

[J09] 时区处理
来源：http://hn.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://we.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sb.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://so.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nj.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nw.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oi.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mg.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nt.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://xb.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vt.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ks.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dn.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ag.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://na.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dx.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hc.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jj.shtwfgs.cn

================================================================================
来源：http://qx.haigaiapp.cn

K. JSON 与序列化
来源：http://bl.colortex.cn

================================================================================
来源：http://xa.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://lu.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://on.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zc.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://fn.asd995.cn

TS:   JSON.stringify(obj)
来源：http://aj.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ms.asd995.cn

Go:   json.Marshal(obj)
来源：http://cv.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ue.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cq.hahajie.cn

[K02] JSON 字符串转对象
来源：http://gu.haigaiapp.cn

Py:   json.loads(s)
来源：http://mg.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fr.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://yy.szxytkj.cn

TS:   JSON.parse(s)
来源：http://vd.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://df.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://iq.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://dz.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://yr.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vh.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hd.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tc.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ri.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://we.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ks.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://go.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fp.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://uw.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ea.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cb.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nh.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qz.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://us.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://db.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rz.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yr.chemitech.net.cn

[K05] 深拷贝对象
来源：http://in.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://yy.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://fp.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://ui.szsharing.cn

TS:   structuredClone(obj)
来源：http://ns.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rq.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fm.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nn.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://av.hahajie.cn

[K06] 解析 URL 查询串
来源：http://un.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xj.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qg.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vh.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ei.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jq.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kw.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vv.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bc.jianghongdianzi.cn

[K07] 进制转换
来源：http://kc.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ei.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xp.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://il.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zf.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jt.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lj.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://st.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cv.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://cc.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://so.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rk.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://fh.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://oe.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mi.huanxung.cn

Go:   encoding/gob
来源：http://zm.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://vr.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://up.bookmarksfly.cn

================================================================================
来源：http://az.huixiangedu.cn

L. 网络请求
来源：http://vj.hahajie.cn

================================================================================
来源：http://ka.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://dp.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hj.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ft.bjjhwx.cn

JS:   await fetch(url)
来源：http://bt.yuexingan06.cn

TS:   await fetch(url)
来源：http://fg.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kr.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://xg.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oj.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xv.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://kz.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eq.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xi.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fb.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://my.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vo.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qd.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wg.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mk.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://gg.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hh.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tn.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qm.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tg.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gb.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nu.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://li.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ou.bjjhwx.cn

[L04] 设置超时
来源：http://dp.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://qx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xc.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nn.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mn.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ii.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dr.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dl.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ez.9csxet.cn

[L05] 上传文件（multipart）
来源：http://rf.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://go.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wr.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lx.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qe.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dy.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sk.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oh.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oo.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ot.huixinmuqiang.cn

Py:   resp.json()
来源：http://zw.huanxung.cn

PHP:  json_decode($body, true);
来源：http://nq.nszjky.cn

JS:   await resp.json()
来源：http://aw.9csxet.cn

TS:   await resp.json()
来源：http://fs.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fj.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ye.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://lu.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yj.nszjky.cn


<!-- 参考信息 -->