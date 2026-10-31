代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tl.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ss.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yl.wgjwhj.cn

[H10] 资源自动释放
来源：http://pq.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ix.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qw.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ao.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ru.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nl.huixiangedu.cn

Go:   defer f.Close()
来源：http://jj.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gw.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oh.asd995.cn

================================================================================
来源：http://bk.nicolike.cn

I. 正则表达式
来源：http://px.gzmigu.cn

================================================================================
来源：http://um.newstarts.cn

[I01] 判断是否匹配
来源：http://ro.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qq.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vq.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://om.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://nj.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://of.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://or.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gw.nicolike.cn

[I02] 提取所有匹配
来源：http://fw.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://de.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zs.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hg.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://gn.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cs.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uv.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ns.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ju.panjiajie.cn

[I03] 提取捕获分组
来源：http://mv.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uw.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yz.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ea.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zo.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://va.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bh.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mo.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://er.jctech888.com.cn

[I04] 正则替换
来源：http://vl.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://do.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://up.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zo.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ah.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mq.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iz.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pn.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jj.newstarts.cn

[I05] 按正则拆分
来源：http://bg.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tg.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ku.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wl.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ri.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://sy.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ya.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ra.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eo.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sx.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nu.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wp.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tf.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tu.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xu.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oy.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pt.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jj.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://vj.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ml.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bg.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fu.hahajie.cn

TS:   /error/gim
来源：http://fs.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ma.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bj.asd995.cn

Ruby: s.scan(/error/i)
来源：http://lh.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nb.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://gz.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dq.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ya.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pt.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ce.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nl.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rx.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rs.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rk.bookmarksfly.cn

================================================================================
来源：http://ix.asd995.cn

J. 日期与时间
来源：http://vr.jianghongdianzi.cn

================================================================================
来源：http://vy.bjjhwx.cn

[J01] 获取当前时间
来源：http://bw.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tn.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://br.szsharing.cn

JS:   new Date();  Date.now()
来源：http://qk.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://lz.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cg.szsharing.cn

Go:   time.Now()
来源：http://hl.huanxung.cn

Ruby: Time.now
来源：http://ok.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lv.haigaiapp.cn

[J02] 格式化输出
来源：http://jw.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xl.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wt.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ot.colortex.cn

TS:   d.toISOString()
来源：http://hv.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gy.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oq.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sn.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tl.hahajie.cn

[J03] 字符串解析为日期
来源：http://il.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xk.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tr.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ku.asd995.cn

TS:   new Date("2024-01-02")
来源：http://de.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lz.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ew.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://ri.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://op.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://xt.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hj.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sz.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sv.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://my.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ft.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ha.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://go.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ky.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://lq.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://vh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mg.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cq.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vm.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://qc.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rw.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ax.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ko.huixiangedu.cn

[J06] 计算两时间之差
来源：http://wp.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://dd.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://uc.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yv.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fg.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fb.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ks.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://dy.521024.cn

C#:   (end - start).TotalSeconds
来源：http://fr.nicolike.cn

[J07] 比较两个日期
来源：http://qb.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://zp.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ft.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jr.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uo.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wm.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ul.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://li.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://cv.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://nf.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wu.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iq.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zr.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jq.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oi.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wy.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ow.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bo.chemitech.net.cn

[J09] 时区处理
来源：http://kk.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://av.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ph.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mt.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qu.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uq.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gd.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://od.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cs.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sx.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rz.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vh.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nu.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bj.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kg.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ix.bookmarksfly.cn

================================================================================
来源：http://la.9csxet.cn

K. JSON 与序列化
来源：http://gk.chemitech.net.cn

================================================================================
来源：http://lq.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://dr.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lx.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jc.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://ny.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://de.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tw.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://ko.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ph.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xx.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://dn.asd995.cn

Py:   json.loads(s)
来源：http://kx.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fp.gzmigu.cn

JS:   JSON.parse(s)
来源：http://sh.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://lo.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xl.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://yq.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://kn.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lp.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://do.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aw.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ix.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jk.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://py.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ij.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cs.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jd.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kk.huanxung.cn

[K04] 读取 JSON 文件
来源：http://ey.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sb.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lt.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dj.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nd.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zd.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xy.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yd.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dm.asd995.cn

[K05] 深拷贝对象
来源：http://vz.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://fu.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://vt.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ov.asd995.cn

TS:   structuredClone(obj)
来源：http://uh.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hs.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qy.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mq.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fq.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://zv.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vd.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qg.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bz.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nt.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pu.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qa.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lf.nszjky.cn

[K07] 进制转换
来源：http://fu.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qr.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ix.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ef.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://az.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ut.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oq.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cj.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cr.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ta.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://fy.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aq.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zm.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://wn.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://md.yuntaijiaju.cn

Go:   encoding/gob
来源：http://px.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://iq.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mq.shxzukj.cn

================================================================================
来源：http://pc.hnjuh.cn

L. 网络请求
来源：http://nm.wgjwhj.cn

================================================================================
来源：http://fe.szxytkj.cn

[L01] 发送 GET 请求
来源：http://gd.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xy.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dx.lnxyls.cn

JS:   await fetch(url)
来源：http://gs.nicolike.cn

TS:   await fetch(url)
来源：http://hi.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bb.521024.cn

Go:   resp, err := http.Get(url)
来源：http://jy.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dr.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hw.szsharing.cn

[L02] 发送 POST JSON
来源：http://lb.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ic.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vp.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vd.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://od.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dx.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ox.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://no.szsharing.cn

[L03] 设置自定义请求头
来源：http://oa.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yy.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ev.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sj.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mm.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sl.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vv.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ky.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ek.521024.cn

[L04] 设置超时
来源：http://tg.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://ej.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dt.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ih.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gs.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wc.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ao.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ja.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ik.newstarts.cn

[L05] 上传文件（multipart）
来源：http://qx.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qh.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ie.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://er.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ic.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qr.521024.cn


<!-- 参考信息 -->