代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dy.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jq.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cb.szsharing.cn

[H10] 资源自动释放
来源：http://bk.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://er.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xf.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fb.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yx.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jh.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://vj.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mk.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ji.hnjuh.cn

================================================================================
来源：http://oh.shxzskj.cn

I. 正则表达式
来源：http://eg.szsharing.cn

================================================================================
来源：http://bw.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://lk.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hh.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vs.colortex.cn

JS:   /\d+/.test(s)
来源：http://nj.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://gq.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://st.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mw.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://lv.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sr.jctech888.com.cn

[I02] 提取所有匹配
来源：http://zx.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://vc.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://px.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fr.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://cc.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ow.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mx.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://bq.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ry.huixiangedu.cn

[I03] 提取捕获分组
来源：http://sp.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sn.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zp.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fy.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bn.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ax.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://as.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zv.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fa.nszjky.cn

[I04] 正则替换
来源：http://fs.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hs.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fz.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fu.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vz.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ci.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zd.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tf.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tk.muxihuayi.cn

[I05] 按正则拆分
来源：http://vo.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yd.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nh.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://xp.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://ll.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://jf.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ts.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vn.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nz.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://po.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ji.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wy.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mh.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eb.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zc.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lg.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://km.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://tj.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dj.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ud.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bo.chemitech.net.cn

TS:   /error/gim
来源：http://ac.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sb.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ca.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://wx.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ip.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rk.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://le.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xr.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jc.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yd.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://as.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ux.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://go.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://br.nicolike.cn

================================================================================
来源：http://fw.huanxung.cn

J. 日期与时间
来源：http://el.szsharing.cn

================================================================================
来源：http://gl.521024.cn

[J01] 获取当前时间
来源：http://in.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ce.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jh.nszjky.cn

JS:   new Date();  Date.now()
来源：http://bj.9csxet.cn

TS:   new Date();  Date.now()
来源：http://jw.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ho.szsharing.cn

Go:   time.Now()
来源：http://fh.haigaiapp.cn

Ruby: Time.now
来源：http://ue.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://by.bookmarksfly.cn

[J02] 格式化输出
来源：http://iv.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mk.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nd.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nd.bjjhwx.cn

TS:   d.toISOString()
来源：http://te.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vy.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fn.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qd.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vn.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ax.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gi.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tx.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ia.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://wr.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ad.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ku.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://an.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://my.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://sb.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://td.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uc.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sx.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fj.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hu.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cw.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qv.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zd.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://dw.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://hj.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qa.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fu.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nc.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://mm.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yw.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ev.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pk.asd995.cn

[J06] 计算两时间之差
来源：http://je.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://wm.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://td.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://si.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hx.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://je.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://co.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://gl.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://fs.szsharing.cn

[J07] 比较两个日期
来源：http://aj.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ca.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ma.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://of.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dp.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xb.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ym.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lr.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://cp.asd995.cn

[J08] 提取年月日与星期
来源：http://wd.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cr.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sf.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cc.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yy.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uj.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nd.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bs.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.jctech888.com.cn

[J09] 时区处理
来源：http://yo.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kv.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lx.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tb.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mu.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ms.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ee.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zz.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hy.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://qy.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vc.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rl.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eu.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ag.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sh.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mr.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pd.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jq.gzmigu.cn

================================================================================
来源：http://pe.bookmarksfly.cn

K. JSON 与序列化
来源：http://cs.9csxet.cn

================================================================================
来源：http://uz.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://it.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zr.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://be.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://yt.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://fm.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uq.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://mh.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rz.huanxung.cn

[K02] JSON 字符串转对象
来源：http://gz.nicolike.cn

Py:   json.loads(s)
来源：http://ik.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pr.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://em.gzmigu.cn

TS:   JSON.parse(s)
来源：http://yj.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jm.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://tn.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://wf.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pf.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://xs.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vs.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bj.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mm.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fm.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ig.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iu.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eh.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://py.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://tu.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qf.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vp.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uh.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kv.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gw.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nr.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ym.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fh.huixiangedu.cn

[K05] 深拷贝对象
来源：http://wr.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://yg.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://qh.newstarts.cn

JS:   structuredClone(obj)
来源：http://yo.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://jn.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nf.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ov.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://op.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zn.colortex.cn

[K06] 解析 URL 查询串
来源：http://jw.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dk.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zj.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wu.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pp.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dw.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vt.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iq.chemitech.net.cn

[K07] 进制转换
来源：http://wu.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ig.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sl.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tq.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pu.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ll.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ia.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rr.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://sb.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://zr.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bq.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://yp.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://mk.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qg.lnxyls.cn

Go:   encoding/gob
来源：http://rr.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://rg.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cb.9csxet.cn

================================================================================
来源：http://oc.bookmarksfly.cn

L. 网络请求
来源：http://bc.521024.cn

================================================================================
来源：http://dj.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://my.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iu.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qk.bjjhwx.cn

JS:   await fetch(url)
来源：http://zn.newstarts.cn

TS:   await fetch(url)
来源：http://qp.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ni.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://zx.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dx.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ql.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ml.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pn.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ub.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kl.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rq.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sh.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vk.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xi.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dt.szxytkj.cn

[L03] 设置自定义请求头
来源：http://iq.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dq.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fg.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ug.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ah.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yv.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ok.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sn.wgjwhj.cn

[L04] 设置超时
来源：http://hz.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://qv.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nl.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ll.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ff.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qy.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lq.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://so.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hs.9csxet.cn

[L05] 上传文件（multipart）
来源：http://vq.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hg.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vg.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ed.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pg.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xx.9csxet.cn


<!-- 参考信息 -->