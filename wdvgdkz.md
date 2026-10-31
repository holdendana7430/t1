代发 wailian999

================================================================================
来源：http://jz.huanxung.cn

I. 正则表达式
来源：http://if.huanxung.cn

================================================================================
来源：http://ub.hahajie.cn

[I01] 判断是否匹配
来源：http://qp.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kb.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vz.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://ht.hahajie.cn

TS:   /\d+/.test(s)
来源：http://jv.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gj.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aj.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://bc.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bx.jctech888.com.cn

[I02] 提取所有匹配
来源：http://fn.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://in.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://df.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jg.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://vd.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zy.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rq.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://su.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xe.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://yq.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://py.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ks.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hl.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rr.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pa.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yz.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://js.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://af.jctech888.com.cn

[I04] 正则替换
来源：http://qr.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ev.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qj.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ke.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yn.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dt.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sj.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mj.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ox.asd995.cn

[I05] 按正则拆分
来源：http://wj.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hn.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ho.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://lh.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://pk.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://tz.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://li.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xs.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mg.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zv.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oa.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yt.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bb.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bl.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jf.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pu.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qu.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dy.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://wb.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fv.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gr.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ta.bjjhwx.cn

TS:   /error/gim
来源：http://bd.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fx.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iz.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://qc.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jg.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yw.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://il.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bo.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fr.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vb.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nh.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nh.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zt.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jr.gzmigu.cn

================================================================================
来源：http://mq.asd995.cn

J. 日期与时间
来源：http://om.panjiajie.cn

================================================================================
来源：http://ey.huanxung.cn

[J01] 获取当前时间
来源：http://ed.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xt.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kr.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://ng.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://yk.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nv.szxytkj.cn

Go:   time.Now()
来源：http://oy.nszjky.cn

Ruby: Time.now
来源：http://zq.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jv.nszjky.cn

[J02] 格式化输出
来源：http://se.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uc.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bv.lnxyls.cn

TS:   d.toISOString()
来源：http://qj.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://go.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uq.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ez.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fn.lnxyls.cn

[J03] 字符串解析为日期
来源：http://bw.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zl.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fp.colortex.cn

JS:   new Date("2024-01-02")
来源：http://id.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://dg.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zo.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mt.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://up.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zl.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://py.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://db.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ti.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zr.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tz.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gf.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jm.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yc.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jw.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://kg.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://zz.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qv.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sg.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hp.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://yi.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ks.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://yz.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qb.newstarts.cn

[J06] 计算两时间之差
来源：http://sq.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://hm.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://qo.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zo.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eb.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ey.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://jd.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://lx.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://fe.huanxung.cn

[J07] 比较两个日期
来源：http://fv.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://am.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xn.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zi.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yc.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sw.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pw.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zm.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://mu.521024.cn

[J08] 提取年月日与星期
来源：http://yr.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://js.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rc.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xh.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vz.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fs.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ih.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cr.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kz.hnjuh.cn

[J09] 时区处理
来源：http://ec.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lk.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hu.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kb.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://es.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lc.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xg.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qy.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://se.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://dq.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dx.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xc.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kl.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ru.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ri.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ev.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://du.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vq.yuntaijiaju.cn

================================================================================
来源：http://ci.shxzskj.cn

K. JSON 与序列化
来源：http://ob.yuntaijiaju.cn

================================================================================
来源：http://fh.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://wf.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ic.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bd.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ed.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://dh.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lg.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://la.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cl.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wb.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ap.huixiangedu.cn

Py:   json.loads(s)
来源：http://be.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://af.asd995.cn

JS:   JSON.parse(s)
来源：http://co.shxzukj.cn

TS:   JSON.parse(s)
来源：http://or.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tf.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://zt.521024.cn

Ruby: JSON.parse(s)
来源：http://uj.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://em.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://gu.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oj.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://as.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eg.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lp.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kr.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cl.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://an.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dc.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://hk.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cq.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wx.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ca.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oi.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hj.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lf.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qe.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oi.9csxet.cn

[K05] 深拷贝对象
来源：http://zs.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://ze.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://st.521024.cn

JS:   structuredClone(obj)
来源：http://sl.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://fx.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qw.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mi.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://od.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hy.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://fk.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qk.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://re.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jh.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uv.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wg.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fp.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gj.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xr.chemitech.net.cn

[K07] 进制转换
来源：http://ab.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://td.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gn.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ry.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hh.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tb.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bs.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ud.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ck.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sc.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://wy.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ty.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://bp.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://jf.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nr.yuntaijiaju.cn

Go:   encoding/gob
来源：http://nc.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://lz.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ld.nszjky.cn

================================================================================
来源：http://ml.huixinmuqiang.cn

L. 网络请求
来源：http://ev.nszjky.cn

================================================================================
来源：http://ge.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://pw.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qo.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qu.shxzukj.cn

JS:   await fetch(url)
来源：http://no.panjiajie.cn

TS:   await fetch(url)
来源：http://il.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://un.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://nv.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lb.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qv.521024.cn

[L02] 发送 POST JSON
来源：http://kz.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dn.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nb.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ti.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ur.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nt.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dp.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ii.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ff.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://lh.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kc.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nb.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yc.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://op.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gm.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pa.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://np.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ov.nszjky.cn

[L04] 设置超时
来源：http://er.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://iv.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qt.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qz.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cl.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oj.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kb.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vm.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sb.huanxung.cn

[L05] 上传文件（multipart）
来源：http://bq.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://va.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jn.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zy.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yn.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bd.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vw.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pg.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zu.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://zc.jianghongdianzi.cn

Py:   resp.json()
来源：http://ia.asd995.cn

PHP:  json_decode($body, true);
来源：http://pa.panjiajie.cn

JS:   await resp.json()
来源：http://ug.newstarts.cn

TS:   await resp.json()
来源：http://sg.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://co.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bv.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://zz.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ro.huixiangedu.cn


<!-- 参考信息 -->