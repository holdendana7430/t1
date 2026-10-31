代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hn.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ru.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vh.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pm.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sh.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sg.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nt.muxihuayi.cn

[H10] 资源自动释放
来源：http://di.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ao.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bb.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oe.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fy.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pq.nszjky.cn

Go:   defer f.Close()
来源：http://yy.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zy.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ta.bjjhwx.cn

================================================================================
来源：http://dw.jctech888.com.cn

I. 正则表达式
来源：http://xz.shxzskj.cn

================================================================================
来源：http://og.chemitech.net.cn

[I01] 判断是否匹配
来源：http://tx.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ap.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zd.nszjky.cn

JS:   /\d+/.test(s)
来源：http://fa.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://fu.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lb.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://le.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://hc.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bf.bjjhwx.cn

[I02] 提取所有匹配
来源：http://qv.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://vn.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bt.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yp.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://vz.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ff.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rb.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://fu.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ww.521024.cn

[I03] 提取捕获分组
来源：http://au.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://st.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dx.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zz.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ee.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://va.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qz.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zp.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ut.shxzukj.cn

[I04] 正则替换
来源：http://wn.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://az.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yi.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kp.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yi.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qr.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lt.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tx.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://th.hahajie.cn

[I05] 按正则拆分
来源：http://cn.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dg.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://so.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://yl.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://eq.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://gl.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nn.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ut.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vm.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yp.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rj.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yk.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lo.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bi.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hp.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pa.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lu.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wf.521024.cn

[I07] 忽略大小写与多行模式
来源：http://xq.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kn.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bf.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ss.nszjky.cn

TS:   /error/gim
来源：http://qr.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://np.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qj.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://bv.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yu.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ie.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ra.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mo.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rp.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oy.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kf.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://id.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pn.huanxung.cn

================================================================================
来源：http://tb.szxytkj.cn

J. 日期与时间
来源：http://ya.szxytkj.cn

================================================================================
来源：http://qz.9csxet.cn

[J01] 获取当前时间
来源：http://nx.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vv.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rx.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://pr.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://vz.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ol.nszjky.cn

Go:   time.Now()
来源：http://rx.jctech888.com.cn

Ruby: Time.now
来源：http://nc.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zg.lnxyls.cn

[J02] 格式化输出
来源：http://jv.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nm.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ue.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xg.lnxyls.cn

TS:   d.toISOString()
来源：http://vr.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tm.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fo.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qk.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cz.9csxet.cn

[J03] 字符串解析为日期
来源：http://rw.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bn.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://js.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://rj.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://ow.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ea.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://za.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://tz.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ep.huanxung.cn

[J04] 时间戳与日期互转
来源：http://qm.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yw.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wf.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iv.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hs.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sv.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qw.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fi.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ci.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://ag.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://zy.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tk.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gr.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://or.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://sb.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bn.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://nj.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mn.gzmigu.cn

[J06] 计算两时间之差
来源：http://cn.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://dk.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://ly.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gt.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uf.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yk.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://lb.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://gf.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://pu.panjiajie.cn

[J07] 比较两个日期
来源：http://lt.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://cq.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://no.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://do.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fq.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cd.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rs.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gx.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ed.colortex.cn

[J08] 提取年月日与星期
来源：http://uf.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lw.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lp.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dg.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ox.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sc.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ww.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hn.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fi.newstarts.cn

[J09] 时区处理
来源：http://es.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iy.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cm.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bq.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jt.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pu.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qk.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ma.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gh.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://ct.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://un.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nd.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dt.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nm.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ci.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yz.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://px.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ml.muxihuayi.cn

================================================================================
来源：http://zw.jctech888.com.cn

K. JSON 与序列化
来源：http://kx.nszjky.cn

================================================================================
来源：http://ti.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://hn.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vp.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cy.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://in.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://fo.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ww.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://lv.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qu.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hx.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://wg.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://ro.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fq.asd995.cn

JS:   JSON.parse(s)
来源：http://cg.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://ai.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://si.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://el.colortex.cn

Ruby: JSON.parse(s)
来源：http://br.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://be.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://wy.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nc.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ir.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jr.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kg.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cf.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://on.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hy.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vf.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://dy.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hj.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jn.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ci.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xu.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ma.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lb.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mn.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qv.haigaiapp.cn

[K05] 深拷贝对象
来源：http://xc.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://xz.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://hn.hahajie.cn

JS:   structuredClone(obj)
来源：http://fu.hnjuh.cn

TS:   structuredClone(obj)
来源：http://tz.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vj.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sv.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kh.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ph.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ee.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zp.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://un.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hk.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ma.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vz.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://le.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rp.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nb.haigaiapp.cn

[K07] 进制转换
来源：http://ha.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://na.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vf.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fb.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pi.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zk.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cf.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://go.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qr.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://rs.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ar.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pv.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ga.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://gn.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nr.shxzukj.cn

Go:   encoding/gob
来源：http://gp.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://we.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://br.jianghongdianzi.cn

================================================================================
来源：http://ja.bjjhwx.cn

L. 网络请求
来源：http://lx.huixinmuqiang.cn

================================================================================
来源：http://bp.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://sy.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pj.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kd.muxihuayi.cn

JS:   await fetch(url)
来源：http://yc.huixiangedu.cn

TS:   await fetch(url)
来源：http://zw.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gy.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://nb.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ih.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vd.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://sa.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uk.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nv.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pi.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://af.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jp.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yj.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qq.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://jk.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zo.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://at.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vd.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jj.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jx.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xq.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ye.bjjhwx.cn

[L04] 设置超时
来源：http://dx.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://vn.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ss.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fe.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ng.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ez.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zx.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qd.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ia.colortex.cn

[L05] 上传文件（multipart）
来源：http://vx.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ok.haigaiapp.cn


<!-- 参考信息 -->