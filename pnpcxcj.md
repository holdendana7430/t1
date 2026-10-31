代发 wailian999

================================================================================
来源：http://xk.jctech888.com.cn

I. 正则表达式
来源：http://di.shtwfgs.cn

================================================================================
来源：http://ut.asd995.cn

[I01] 判断是否匹配
来源：http://rs.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fq.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hq.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ly.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://ca.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ya.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nu.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://tq.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jj.shtwfgs.cn

[I02] 提取所有匹配
来源：http://jj.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://rd.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ke.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://of.colortex.cn

TS:   s.match(/\d+/g)
来源：http://jc.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qi.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fi.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://nc.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mg.colortex.cn

[I03] 提取捕获分组
来源：http://hp.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pz.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xk.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tr.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kx.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://at.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ds.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ky.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gl.lnxyls.cn

[I04] 正则替换
来源：http://my.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://um.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kt.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gk.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ah.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bm.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ux.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hs.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://at.lnxyls.cn

[I05] 按正则拆分
来源：http://tk.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ep.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ml.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://vq.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://bm.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://aj.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qw.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://du.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mn.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kf.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ek.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rc.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cy.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ko.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://va.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://le.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zk.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://bi.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://od.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jc.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ey.yuexingan06.cn

TS:   /error/gim
来源：http://vt.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ef.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yy.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://hg.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wd.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://lu.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pm.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ix.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pz.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zi.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ok.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ps.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cu.yuntaijiaju.cn

================================================================================
来源：http://hh.asd995.cn

J. 日期与时间
来源：http://zs.chemitech.net.cn

================================================================================
来源：http://zd.yuexingan06.cn

[J01] 获取当前时间
来源：http://bc.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sr.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ou.huanxung.cn

JS:   new Date();  Date.now()
来源：http://jr.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://nz.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ud.521024.cn

Go:   time.Now()
来源：http://sb.asd995.cn

Ruby: Time.now
来源：http://bc.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lq.yuntaijiaju.cn

[J02] 格式化输出
来源：http://xb.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ey.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://co.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yd.muxihuayi.cn

TS:   d.toISOString()
来源：http://da.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gd.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://va.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jf.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yk.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://pr.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sy.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kk.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://vb.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://gh.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gg.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qw.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ok.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tw.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://du.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rl.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wz.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ta.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uu.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bq.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xr.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vf.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nx.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://en.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://pp.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://we.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gj.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cn.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://wq.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jp.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://mc.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zy.9csxet.cn

[J06] 计算两时间之差
来源：http://on.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ax.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://oe.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pa.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jj.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rq.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://qx.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://zs.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://mp.yuexingan06.cn

[J07] 比较两个日期
来源：http://vl.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ng.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ql.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dt.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gz.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lx.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fn.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lc.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://wj.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://yf.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ke.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yc.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ou.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pg.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tb.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ii.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://im.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gr.panjiajie.cn

[J09] 时区处理
来源：http://jc.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://il.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tc.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qd.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wa.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lb.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bw.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ia.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ue.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ol.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vc.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lu.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gl.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dz.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ql.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fn.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fn.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kn.chemitech.net.cn

================================================================================
来源：http://dc.hnjuh.cn

K. JSON 与序列化
来源：http://bb.huanxung.cn

================================================================================
来源：http://cl.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://fl.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gt.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mg.asd995.cn

JS:   JSON.stringify(obj)
来源：http://vw.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://tr.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uj.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://ae.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rp.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ob.521024.cn

[K02] JSON 字符串转对象
来源：http://no.9csxet.cn

Py:   json.loads(s)
来源：http://qe.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ws.gzmigu.cn

JS:   JSON.parse(s)
来源：http://tt.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://yl.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zs.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://lf.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://mj.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hf.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://dd.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sp.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sz.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wn.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hv.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yz.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jl.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zr.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mn.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://qr.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://su.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jp.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jx.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vc.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zq.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dj.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zm.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ix.haigaiapp.cn

[K05] 深拷贝对象
来源：http://fv.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://kc.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://hf.newstarts.cn

JS:   structuredClone(obj)
来源：http://rt.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://ng.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ij.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xb.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xq.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://db.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://rd.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ns.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zi.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kh.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mc.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fx.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://td.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lt.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://we.hahajie.cn

[K07] 进制转换
来源：http://kx.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sv.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ir.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ux.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eh.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tr.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ah.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mo.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sf.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ti.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://ys.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gw.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yn.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://uj.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sn.szsharing.cn

Go:   encoding/gob
来源：http://qk.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://ry.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kh.nicolike.cn

================================================================================
来源：http://ot.nszjky.cn

L. 网络请求
来源：http://ty.nszjky.cn

================================================================================
来源：http://xx.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://jj.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ki.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zy.nicolike.cn

JS:   await fetch(url)
来源：http://jj.szxytkj.cn

TS:   await fetch(url)
来源：http://bh.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ui.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://wk.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ar.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ms.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://pb.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uc.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dk.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rb.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://we.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yt.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xn.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://to.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mg.lnxyls.cn

[L03] 设置自定义请求头
来源：http://fm.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gf.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ty.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fv.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uv.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nd.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mg.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uj.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gu.hnjuh.cn

[L04] 设置超时
来源：http://sn.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://qt.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jv.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jb.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yz.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yy.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bn.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://el.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qa.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://zj.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ej.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://di.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kr.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tx.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rf.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://st.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wr.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://yi.bookmarksfly.cn

Py:   resp.json()
来源：http://yu.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://en.wgjwhj.cn

JS:   await resp.json()
来源：http://ln.huixiangedu.cn

TS:   await resp.json()
来源：http://ja.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fr.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mv.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://xa.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zc.bjjhwx.cn


<!-- 参考信息 -->