代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://xs.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://am.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://se.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lf.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fu.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ce.huanxung.cn

[H10] 资源自动释放
来源：http://am.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lm.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sw.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ew.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lh.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rk.shtwfgs.cn

Go:   defer f.Close()
来源：http://rp.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qw.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ft.huixinmuqiang.cn

================================================================================
来源：http://ku.hahajie.cn

I. 正则表达式
来源：http://pv.panjiajie.cn

================================================================================
来源：http://lj.haigaiapp.cn

[I01] 判断是否匹配
来源：http://um.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wv.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jb.nszjky.cn

JS:   /\d+/.test(s)
来源：http://hj.asd995.cn

TS:   /\d+/.test(s)
来源：http://xc.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://si.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wu.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://zm.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lg.nicolike.cn

[I02] 提取所有匹配
来源：http://am.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://gl.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cr.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rk.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://ny.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xj.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yz.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://or.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cm.hnjuh.cn

[I03] 提取捕获分组
来源：http://kv.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vf.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pk.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://me.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tp.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kx.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://be.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ns.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jq.bookmarksfly.cn

[I04] 正则替换
来源：http://px.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cx.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lv.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wi.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bw.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sq.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ni.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pj.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nx.521024.cn

[I05] 按正则拆分
来源：http://gm.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ck.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jg.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://sy.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://jo.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://jb.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://md.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ba.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wa.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ii.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fz.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xh.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vb.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://li.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jz.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ua.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ko.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://zv.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xu.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cc.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sf.jianghongdianzi.cn

TS:   /error/gim
来源：http://co.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ex.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pa.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://zp.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jx.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://cc.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lr.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wx.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hn.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://um.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vp.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wj.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pj.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ta.yuntaijiaju.cn

================================================================================
来源：http://ml.9csxet.cn

J. 日期与时间
来源：http://no.bookmarksfly.cn

================================================================================
来源：http://mp.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://jl.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ch.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ou.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://xw.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ul.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yx.muxihuayi.cn

Go:   time.Now()
来源：http://hw.yuntaijiaju.cn

Ruby: Time.now
来源：http://ow.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gj.szsharing.cn

[J02] 格式化输出
来源：http://ki.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yr.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ug.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eb.bjjhwx.cn

TS:   d.toISOString()
来源：http://tp.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ik.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kj.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://la.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ox.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://eg.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ek.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://og.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://xj.521024.cn

TS:   new Date("2024-01-02")
来源：http://mu.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fa.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qb.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://lo.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ds.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ij.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vw.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fp.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nv.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gr.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wl.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zy.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jw.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gp.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://sb.colortex.cn

Py:   now + timedelta(days=7)
来源：http://fc.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wo.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sy.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pl.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://hz.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://so.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://jl.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ob.huanxung.cn

[J06] 计算两时间之差
来源：http://jr.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://xg.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://bc.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ua.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vm.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hb.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://cy.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://kw.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://sn.jctech888.com.cn

[J07] 比较两个日期
来源：http://co.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vr.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nl.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bv.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://km.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ex.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rg.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bk.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://wn.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://mb.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ds.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vn.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mg.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rc.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xz.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dm.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jx.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wk.wgjwhj.cn

[J09] 时区处理
来源：http://fu.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hx.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ux.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ug.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mk.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jl.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iu.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wo.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sf.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://cl.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hv.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cu.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://br.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://th.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ux.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ig.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vk.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pg.lnxyls.cn

================================================================================
来源：http://le.szxytkj.cn

K. JSON 与序列化
来源：http://ar.haigaiapp.cn

================================================================================
来源：http://mj.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://uc.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zo.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mz.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ja.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://bj.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mc.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://vp.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ls.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cr.nicolike.cn

[K02] JSON 字符串转对象
来源：http://ch.chemitech.net.cn

Py:   json.loads(s)
来源：http://rd.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oo.asd995.cn

JS:   JSON.parse(s)
来源：http://ba.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://xd.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://km.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://in.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://xz.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ej.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://dg.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wo.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vj.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ym.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cq.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ln.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vn.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ho.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://he.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://nm.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gy.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jn.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zm.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://md.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ql.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://en.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://us.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ft.hnjuh.cn

[K05] 深拷贝对象
来源：http://td.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ie.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://ck.panjiajie.cn

JS:   structuredClone(obj)
来源：http://wg.asd995.cn

TS:   structuredClone(obj)
来源：http://vy.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cf.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://je.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jv.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://os.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://vq.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hx.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zl.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tq.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://df.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ne.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://na.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qr.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nv.szsharing.cn

[K07] 进制转换
来源：http://tq.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uz.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://io.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aa.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qx.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://me.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hw.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fk.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gu.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://uu.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://cd.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fb.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://gl.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://nj.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://if.colortex.cn

Go:   encoding/gob
来源：http://ct.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://zt.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dl.bookmarksfly.cn

================================================================================
来源：http://gr.panjiajie.cn

L. 网络请求
来源：http://tw.wgjwhj.cn

================================================================================
来源：http://vn.hahajie.cn

[L01] 发送 GET 请求
来源：http://pu.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zt.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kr.colortex.cn

JS:   await fetch(url)
来源：http://tr.szxytkj.cn

TS:   await fetch(url)
来源：http://fi.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pb.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://aq.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wq.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ht.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://wz.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ku.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fr.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cw.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hp.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jc.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zu.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://di.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://mh.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iv.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rl.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uz.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zn.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qv.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qs.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mq.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zm.shxzukj.cn

[L04] 设置超时
来源：http://td.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://un.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aj.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zt.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pv.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jr.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rg.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yy.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sa.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://td.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xr.521024.cn


<!-- 参考信息 -->