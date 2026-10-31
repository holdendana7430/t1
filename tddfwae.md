代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rk.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://re.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://hx.hahajie.cn

TS:   /\d+/.test(s)
来源：http://bs.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zu.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gk.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://rf.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://et.shtwfgs.cn

[I02] 提取所有匹配
来源：http://je.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://ce.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zf.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dl.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://gp.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fn.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cq.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://mv.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pq.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://vp.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xq.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eb.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lu.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://df.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fh.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rm.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tz.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bx.gzmigu.cn

[I04] 正则替换
来源：http://di.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gb.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yl.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uu.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vm.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bw.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ut.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cx.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zy.lnxyls.cn

[I05] 按正则拆分
来源：http://gs.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gg.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ot.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://hq.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ap.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://at.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ew.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ir.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xh.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ku.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vx.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xt.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iw.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lq.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hp.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dg.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ha.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://in.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://jh.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mv.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ys.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qv.jianghongdianzi.cn

TS:   /error/gim
来源：http://pw.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pc.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://os.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://bq.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jf.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ph.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qn.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zl.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uq.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ov.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ts.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cu.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nd.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dt.chemitech.net.cn

================================================================================
来源：http://jr.yuexingan06.cn

J. 日期与时间
来源：http://sl.colortex.cn

================================================================================
来源：http://va.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://zc.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oj.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pm.9csxet.cn

JS:   new Date();  Date.now()
来源：http://qb.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://qp.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pc.panjiajie.cn

Go:   time.Now()
来源：http://fj.szxytkj.cn

Ruby: Time.now
来源：http://nz.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hd.huixinmuqiang.cn

[J02] 格式化输出
来源：http://qs.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://up.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aa.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gv.jctech888.com.cn

TS:   d.toISOString()
来源：http://yu.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gs.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rn.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ln.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://te.szsharing.cn

[J03] 字符串解析为日期
来源：http://zw.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oo.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sm.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://ik.colortex.cn

TS:   new Date("2024-01-02")
来源：http://cm.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://la.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lc.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://kl.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ui.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://vl.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nb.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vk.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ii.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://re.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hh.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aw.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xo.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ni.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ev.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ho.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://td.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://th.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xm.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://uu.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://me.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://pu.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yz.gzmigu.cn

[J06] 计算两时间之差
来源：http://ix.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://st.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://xy.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qs.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uk.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://te.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://ko.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://xy.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://fq.bookmarksfly.cn

[J07] 比较两个日期
来源：http://gm.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://qs.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bu.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://se.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kt.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oy.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://na.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gz.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://eu.szxytkj.cn

[J08] 提取年月日与星期
来源：http://jl.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mp.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ft.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bh.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yp.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qz.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ab.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nv.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.wgjwhj.cn

[J09] 时区处理
来源：http://mj.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://td.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://st.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bs.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pu.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://va.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://de.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tj.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vt.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://fv.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vm.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nl.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tx.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vo.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dw.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yr.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fq.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vy.bookmarksfly.cn

================================================================================
来源：http://eb.newstarts.cn

K. JSON 与序列化
来源：http://bd.bookmarksfly.cn

================================================================================
来源：http://zo.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://yw.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ua.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ya.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://dq.colortex.cn

TS:   JSON.stringify(obj)
来源：http://na.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lq.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ds.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tn.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gf.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://bd.hahajie.cn

Py:   json.loads(s)
来源：http://zf.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rh.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://fm.asd995.cn

TS:   JSON.parse(s)
来源：http://mt.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yd.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://kq.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://hp.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ue.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://by.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bs.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ff.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pn.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ca.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ny.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kx.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nv.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pt.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://dx.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eb.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fn.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://br.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xd.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kw.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ul.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bi.yuexingan06.cn

[K05] 深拷贝对象
来源：http://wh.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://si.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://qk.gzmigu.cn

JS:   structuredClone(obj)
来源：http://nm.gzmigu.cn

TS:   structuredClone(obj)
来源：http://rf.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ek.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vh.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mf.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cl.nicolike.cn

[K06] 解析 URL 查询串
来源：http://rm.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ct.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ix.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wz.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xg.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bd.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://di.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wv.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ki.szsharing.cn

[K07] 进制转换
来源：http://mw.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kn.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bt.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rv.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tn.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wk.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://an.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ar.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://as.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://zy.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ol.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vd.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://li.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://ww.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ux.yuexingan06.cn

Go:   encoding/gob
来源：http://cr.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://bb.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fi.bjjhwx.cn

================================================================================
来源：http://jb.szxytkj.cn

L. 网络请求
来源：http://va.bookmarksfly.cn

================================================================================
来源：http://yz.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ma.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://me.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vr.shxzskj.cn

JS:   await fetch(url)
来源：http://iw.9csxet.cn

TS:   await fetch(url)
来源：http://bd.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kb.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://io.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vl.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pb.lnxyls.cn

[L02] 发送 POST JSON
来源：http://nr.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ae.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://az.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aj.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ns.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dp.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kq.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tu.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xz.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://xj.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cs.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qy.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xn.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uv.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fi.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jr.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ly.hahajie.cn

[L04] 设置超时
来源：http://zo.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://fo.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xi.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wd.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pu.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fm.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rp.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rn.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://qt.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://co.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sj.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yq.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wu.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rd.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tg.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nz.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wv.hahajie.cn

[L06] 解析响应为 JSON
来源：http://of.huanxung.cn

Py:   resp.json()
来源：http://fu.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ac.bjjhwx.cn

JS:   await resp.json()
来源：http://pj.huixiangedu.cn

TS:   await resp.json()
来源：http://wa.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://do.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pc.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ux.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pc.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://gp.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yg.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lt.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://gv.shtwfgs.cn


<!-- 参考信息 -->