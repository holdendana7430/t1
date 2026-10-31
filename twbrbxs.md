代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kx.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ha.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ix.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://gj.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gi.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://do.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oi.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ry.huanxung.cn

Go:   defer f.Close()
来源：http://qn.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gj.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ka.jianghongdianzi.cn

================================================================================
来源：http://je.9csxet.cn

I. 正则表达式
来源：http://vp.haigaiapp.cn

================================================================================
来源：http://zb.gzmigu.cn

[I01] 判断是否匹配
来源：http://go.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cv.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pb.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://xf.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://er.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vi.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nf.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://gd.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sc.bjjhwx.cn

[I02] 提取所有匹配
来源：http://hr.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ro.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ll.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jx.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://xf.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://md.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zp.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://aj.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uu.muxihuayi.cn

[I03] 提取捕获分组
来源：http://nt.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rh.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mr.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cq.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yr.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://di.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rw.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sf.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ot.hnjuh.cn

[I04] 正则替换
来源：http://qa.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://es.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ct.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mw.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://io.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hn.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://go.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zs.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vu.shtwfgs.cn

[I05] 按正则拆分
来源：http://fu.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zc.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ia.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://xi.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://yh.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://ar.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lo.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mr.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://av.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bn.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rk.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nq.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wk.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ek.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cq.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gc.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ig.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://gl.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fd.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xt.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nr.lnxyls.cn

TS:   /error/gim
来源：http://bo.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dz.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uv.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://qq.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ic.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://kn.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wc.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qc.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mq.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tn.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kk.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kq.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qg.nszjky.cn

================================================================================
来源：http://cw.szxytkj.cn

J. 日期与时间
来源：http://jo.yuexingan06.cn

================================================================================
来源：http://hg.nszjky.cn

[J01] 获取当前时间
来源：http://ay.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hd.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lg.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://yv.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://hj.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dq.shxzukj.cn

Go:   time.Now()
来源：http://ka.hnjuh.cn

Ruby: Time.now
来源：http://sq.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wq.panjiajie.cn

[J02] 格式化输出
来源：http://od.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mk.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bd.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tg.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://ia.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lr.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yi.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ed.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uy.panjiajie.cn

[J03] 字符串解析为日期
来源：http://li.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xb.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fp.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://gg.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://sj.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wq.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rn.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://pf.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ac.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://gt.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aj.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://un.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qj.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eo.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://te.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xy.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xh.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ly.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://fq.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://ce.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xq.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pk.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://db.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://vq.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hk.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://ac.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://un.lnxyls.cn

[J06] 计算两时间之差
来源：http://ka.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://rs.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://sa.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wu.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ck.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mk.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://of.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ng.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://uw.shxzukj.cn

[J07] 比较两个日期
来源：http://jw.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://bi.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://of.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uf.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bk.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mh.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ro.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iz.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ry.nicolike.cn

[J08] 提取年月日与星期
来源：http://tu.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uy.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://po.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tv.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yw.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cb.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dx.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qb.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.shxzukj.cn

[J09] 时区处理
来源：http://lc.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gf.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://al.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ra.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ld.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ed.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xr.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://et.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xg.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://qi.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rj.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jz.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jc.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ou.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vz.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nu.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://go.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hm.shxzukj.cn

================================================================================
来源：http://oj.muxihuayi.cn

K. JSON 与序列化
来源：http://is.lnxyls.cn

================================================================================
来源：http://dj.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://lr.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yt.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ev.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://kl.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://xw.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uj.hahajie.cn

Go:   json.Marshal(obj)
来源：http://dv.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ei.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pk.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ml.shxzskj.cn

Py:   json.loads(s)
来源：http://us.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qo.shxzskj.cn

JS:   JSON.parse(s)
来源：http://rf.gzmigu.cn

TS:   JSON.parse(s)
来源：http://jb.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wa.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://ul.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://tp.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bh.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://kd.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dz.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eo.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fc.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zs.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qr.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://px.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yj.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ly.521024.cn

[K04] 读取 JSON 文件
来源：http://wa.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gv.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ln.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zv.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jr.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ii.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yo.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ws.bjjhwx.cn

[K05] 深拷贝对象
来源：http://no.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://cz.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://de.newstarts.cn

JS:   structuredClone(obj)
来源：http://cb.nszjky.cn

TS:   structuredClone(obj)
来源：http://tk.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wb.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cc.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fl.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hr.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://as.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pc.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lg.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wl.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uf.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://in.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tp.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://td.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gw.jianghongdianzi.cn

[K07] 进制转换
来源：http://zj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gh.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ow.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dq.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pg.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sg.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wl.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kt.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kw.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://wb.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://xv.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ca.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ov.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://of.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://av.panjiajie.cn

Go:   encoding/gob
来源：http://jb.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://ly.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rr.wgjwhj.cn

================================================================================
来源：http://tq.chemitech.net.cn

L. 网络请求
来源：http://gr.9csxet.cn

================================================================================
来源：http://zx.9csxet.cn

[L01] 发送 GET 请求
来源：http://sv.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fd.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wc.9csxet.cn

JS:   await fetch(url)
来源：http://zr.huanxung.cn

TS:   await fetch(url)
来源：http://xk.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mb.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://ny.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pz.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sm.asd995.cn

[L02] 发送 POST JSON
来源：http://wk.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cg.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wx.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wv.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sn.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ij.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bw.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pw.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hh.hnjuh.cn

[L03] 设置自定义请求头
来源：http://nl.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ly.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yy.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nz.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tl.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vr.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ju.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fz.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xt.521024.cn

[L04] 设置超时
来源：http://ed.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://ft.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dn.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://un.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xr.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hg.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://us.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iq.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oh.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://hj.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ci.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bk.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://as.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cc.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vi.colortex.cn


<!-- 参考信息 -->