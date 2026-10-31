代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fy.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mg.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oh.shxzukj.cn

[H10] 资源自动释放
来源：http://ar.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rx.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cv.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ah.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cb.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://we.hnjuh.cn

Go:   defer f.Close()
来源：http://tt.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rt.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ed.9csxet.cn

================================================================================
来源：http://zw.shxzskj.cn

I. 正则表达式
来源：http://rm.huanxung.cn

================================================================================
来源：http://ov.shtwfgs.cn

[I01] 判断是否匹配
来源：http://vm.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lo.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cd.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://la.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://hl.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xu.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cj.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://cr.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fn.shxzskj.cn

[I02] 提取所有匹配
来源：http://px.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ft.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uf.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yi.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://oa.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zx.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rn.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://sg.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mk.gzmigu.cn

[I03] 提取捕获分组
来源：http://nd.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xn.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zt.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xj.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ou.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ly.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dk.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://na.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zc.521024.cn

[I04] 正则替换
来源：http://ps.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://af.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bz.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xm.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://si.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kb.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uy.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wq.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fo.szsharing.cn

[I05] 按正则拆分
来源：http://op.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xk.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ny.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://tm.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://cw.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://qo.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qm.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ih.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kt.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nx.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xz.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://po.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wr.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kl.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://de.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gq.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bm.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ye.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ud.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ka.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ij.shxzskj.cn

TS:   /error/gim
来源：http://jm.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fs.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eq.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://gj.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yh.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://jp.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vz.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ht.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xr.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xr.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qi.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wp.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ry.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sj.huixiangedu.cn

================================================================================
来源：http://ce.chemitech.net.cn

J. 日期与时间
来源：http://py.wgjwhj.cn

================================================================================
来源：http://qa.hahajie.cn

[J01] 获取当前时间
来源：http://jn.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eh.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hv.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://cx.521024.cn

TS:   new Date();  Date.now()
来源：http://ou.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ei.yuntaijiaju.cn

Go:   time.Now()
来源：http://sg.colortex.cn

Ruby: Time.now
来源：http://ya.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cz.jctech888.com.cn

[J02] 格式化输出
来源：http://tg.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iq.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kn.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dl.chemitech.net.cn

TS:   d.toISOString()
来源：http://pa.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sb.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eq.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dj.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://va.hnjuh.cn

[J03] 字符串解析为日期
来源：http://cl.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://li.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kh.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://dr.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://os.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mn.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hq.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ay.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wf.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://qw.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jw.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wb.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ki.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sp.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pi.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ab.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pa.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://di.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://mx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://hd.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ik.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://me.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qv.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://lr.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dj.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://vz.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ik.nicolike.cn

[J06] 计算两时间之差
来源：http://du.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://ap.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://kf.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iz.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qp.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://co.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://bq.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://di.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://wb.muxihuayi.cn

[J07] 比较两个日期
来源：http://rz.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://ny.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rd.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hc.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zt.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://if.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ji.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://df.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://vp.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://rw.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ye.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nu.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xy.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sr.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jd.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jd.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qa.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ap.jianghongdianzi.cn

[J09] 时区处理
来源：http://su.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kc.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bb.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ko.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jx.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hy.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qb.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sb.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sv.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://za.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yi.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ry.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vy.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://te.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://th.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xs.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://km.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ef.hahajie.cn

================================================================================
来源：http://no.shxzskj.cn

K. JSON 与序列化
来源：http://vq.huanxung.cn

================================================================================
来源：http://zv.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://wv.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ta.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oy.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://dz.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://bt.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tu.newstarts.cn

Go:   json.Marshal(obj)
来源：http://xj.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gz.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bs.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://rz.nicolike.cn

Py:   json.loads(s)
来源：http://pj.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kk.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ow.szsharing.cn

TS:   JSON.parse(s)
来源：http://vs.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cr.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://yx.szsharing.cn

Ruby: JSON.parse(s)
来源：http://to.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tc.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ku.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://we.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yc.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lw.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ej.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iw.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://um.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pc.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ca.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://go.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://my.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rx.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hv.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zy.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://of.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://le.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vj.muxihuayi.cn

[K05] 深拷贝对象
来源：http://sn.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://yw.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://fr.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://dv.panjiajie.cn

TS:   structuredClone(obj)
来源：http://mz.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vt.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://em.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jo.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wx.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://fd.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zr.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tk.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vd.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ib.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.nszjky.cn

[K07] 进制转换
来源：http://am.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qw.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wv.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zf.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vt.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zk.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nt.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gp.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sc.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://lh.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://hm.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ua.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ft.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://xo.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xa.bjjhwx.cn

Go:   encoding/gob
来源：http://qe.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://xj.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nr.asd995.cn

================================================================================
来源：http://os.huanxung.cn

L. 网络请求
来源：http://zw.shtwfgs.cn

================================================================================
来源：http://wt.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://em.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cp.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://op.huanxung.cn

JS:   await fetch(url)
来源：http://pe.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ar.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qq.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://pk.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ws.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kh.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://fx.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dn.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ep.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://my.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xb.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gf.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hv.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://is.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ud.colortex.cn

[L03] 设置自定义请求头
来源：http://wd.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gw.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ad.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ne.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qj.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ew.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tl.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iw.nszjky.cn

[L04] 设置超时
来源：http://ts.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://eo.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://go.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://no.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lf.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kn.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cc.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ah.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kv.nicolike.cn

[L05] 上传文件（multipart）
来源：http://fj.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ju.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qb.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xr.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gw.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qb.lnxyls.cn


<!-- 参考信息 -->