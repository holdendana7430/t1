代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://uf.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zq.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://su.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lw.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qn.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ug.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://um.newstarts.cn

[H10] 资源自动释放
来源：http://mj.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rx.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yi.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pa.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xl.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://di.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://up.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yw.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ra.wgjwhj.cn

================================================================================
来源：http://ob.yuexingan06.cn

I. 正则表达式
来源：http://dp.9csxet.cn

================================================================================
来源：http://up.nicolike.cn

[I01] 判断是否匹配
来源：http://yy.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hy.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ye.hahajie.cn

JS:   /\d+/.test(s)
来源：http://lg.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://xw.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bb.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://er.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://hh.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sy.shxzukj.cn

[I02] 提取所有匹配
来源：http://ty.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://dt.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yv.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lh.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://su.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lg.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pr.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://rk.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://io.asd995.cn

[I03] 提取捕获分组
来源：http://hy.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rv.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ln.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://on.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fw.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mz.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mf.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hx.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nx.hahajie.cn

[I04] 正则替换
来源：http://ae.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xq.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ot.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mt.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ys.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://as.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yh.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bl.hahajie.cn

[I05] 按正则拆分
来源：http://ai.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uu.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yw.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://vf.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://hz.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://qn.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jz.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gu.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uf.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kt.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nf.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kl.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://po.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ua.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sj.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cu.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://er.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://og.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wv.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wx.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rm.shtwfgs.cn

TS:   /error/gim
来源：http://qu.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zw.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ay.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://cu.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bg.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ce.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vj.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wo.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oj.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sn.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rm.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://of.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://up.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tu.yuexingan06.cn

================================================================================
来源：http://pu.newstarts.cn

J. 日期与时间
来源：http://la.lnxyls.cn

================================================================================
来源：http://cr.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ky.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lv.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ye.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://xe.9csxet.cn

TS:   new Date();  Date.now()
来源：http://zp.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vh.9csxet.cn

Go:   time.Now()
来源：http://zk.szxytkj.cn

Ruby: Time.now
来源：http://vg.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rz.asd995.cn

[J02] 格式化输出
来源：http://vg.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kc.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fs.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iy.szxytkj.cn

TS:   d.toISOString()
来源：http://pp.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bf.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ks.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ki.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dm.colortex.cn

[J03] 字符串解析为日期
来源：http://lu.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://is.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hi.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://pk.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://qz.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cy.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mg.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://lf.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lw.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://ca.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yv.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rb.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hk.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cx.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jm.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fv.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cz.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nf.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ie.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://iz.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bw.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yk.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nq.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://lb.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gq.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://vt.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kq.bjjhwx.cn

[J06] 计算两时间之差
来源：http://mr.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://ux.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://xs.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uh.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dr.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kw.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://fy.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://mn.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://nj.asd995.cn

[J07] 比较两个日期
来源：http://tu.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://db.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ez.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kj.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qp.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sd.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lr.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kk.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://cp.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://on.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lg.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ah.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jy.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sh.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://um.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mm.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nv.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wc.szxytkj.cn

[J09] 时区处理
来源：http://yg.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dg.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://me.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ad.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kt.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vv.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yo.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gd.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zl.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://gp.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ll.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rh.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wf.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oe.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ah.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uj.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vr.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://of.9csxet.cn

================================================================================
来源：http://bb.bookmarksfly.cn

K. JSON 与序列化
来源：http://la.yuntaijiaju.cn

================================================================================
来源：http://cg.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ls.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tz.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yd.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://jk.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://fp.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qv.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://yd.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gr.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yx.colortex.cn

[K02] JSON 字符串转对象
来源：http://ou.9csxet.cn

Py:   json.loads(s)
来源：http://ux.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gi.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://zt.colortex.cn

TS:   JSON.parse(s)
来源：http://qi.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fx.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://wq.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://bv.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ev.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://xs.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nm.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ti.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zo.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mh.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sb.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vz.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wq.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xx.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://sb.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://on.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://df.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vj.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uu.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nt.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yb.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bk.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sg.nszjky.cn

[K05] 深拷贝对象
来源：http://hv.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://kl.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://ic.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://ar.colortex.cn

TS:   structuredClone(obj)
来源：http://zu.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eq.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pp.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ee.9csxet.cn

[K06] 解析 URL 查询串
来源：http://zj.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pi.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hx.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gr.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ma.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yc.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ew.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fc.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vp.panjiajie.cn

[K07] 进制转换
来源：http://sk.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qn.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bw.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://or.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://md.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://br.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jg.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://li.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xl.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://tt.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zk.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://mn.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://qh.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iv.jianghongdianzi.cn

Go:   encoding/gob
来源：http://ao.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://gc.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ld.9csxet.cn

================================================================================
来源：http://al.hahajie.cn

L. 网络请求
来源：http://pi.jctech888.com.cn

================================================================================
来源：http://pi.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://dj.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://po.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fh.muxihuayi.cn

JS:   await fetch(url)
来源：http://ch.gzmigu.cn

TS:   await fetch(url)
来源：http://fx.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aa.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://se.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gb.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eb.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://ta.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ac.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ef.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://js.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://se.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mn.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xm.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nu.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://qs.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ob.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nq.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tr.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ad.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uz.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hc.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iz.chemitech.net.cn

[L04] 设置超时
来源：http://nb.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://fy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xz.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wd.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tf.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oy.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xr.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mz.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eb.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://au.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pa.hnjuh.cn


<!-- 参考信息 -->