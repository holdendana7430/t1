代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://bf.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bm.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sq.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ho.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tw.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://su.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cs.chemitech.net.cn

[H10] 资源自动释放
来源：http://fs.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cw.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mw.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nr.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xa.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dm.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://wk.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yb.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kp.bjjhwx.cn

================================================================================
来源：http://ni.asd995.cn

I. 正则表达式
来源：http://np.colortex.cn

================================================================================
来源：http://av.szsharing.cn

[I01] 判断是否匹配
来源：http://et.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kh.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cj.huanxung.cn

JS:   /\d+/.test(s)
来源：http://av.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://iv.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fa.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://do.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://qv.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zv.wgjwhj.cn

[I02] 提取所有匹配
来源：http://hu.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ff.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fc.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ju.colortex.cn

TS:   s.match(/\d+/g)
来源：http://xm.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kp.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zt.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://dd.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://be.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://ja.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ex.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hc.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gn.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nm.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ka.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tc.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vo.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pi.newstarts.cn

[I04] 正则替换
来源：http://jz.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yk.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ge.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bq.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vw.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bt.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ob.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nu.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cj.haigaiapp.cn

[I05] 按正则拆分
来源：http://ow.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tl.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yq.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://lu.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://yl.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://xy.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bb.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qr.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xr.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ic.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lz.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qr.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ac.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gr.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ny.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qh.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dt.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dl.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://te.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zt.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nd.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ey.szxytkj.cn

TS:   /error/gim
来源：http://dq.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wq.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cz.colortex.cn

Ruby: s.scan(/error/i)
来源：http://fv.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://le.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://vw.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://he.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rp.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wj.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ry.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xe.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ti.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ns.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gw.9csxet.cn

================================================================================
来源：http://ki.nicolike.cn

J. 日期与时间
来源：http://pj.nicolike.cn

================================================================================
来源：http://da.huixiangedu.cn

[J01] 获取当前时间
来源：http://op.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qn.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dd.521024.cn

JS:   new Date();  Date.now()
来源：http://en.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://qm.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vy.jianghongdianzi.cn

Go:   time.Now()
来源：http://xx.yuexingan06.cn

Ruby: Time.now
来源：http://xh.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sl.muxihuayi.cn

[J02] 格式化输出
来源：http://rp.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nz.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xd.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rv.gzmigu.cn

TS:   d.toISOString()
来源：http://xm.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nb.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hk.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.9csxet.cn

[J03] 字符串解析为日期
来源：http://ou.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pe.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sg.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://hv.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://oc.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jv.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hf.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://sl.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wj.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://kt.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ux.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zo.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://li.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cp.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lr.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hy.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://du.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zy.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://eq.521024.cn

Py:   now + timedelta(days=7)
来源：http://bf.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dw.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bq.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ox.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://ck.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ra.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://bg.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xw.yuexingan06.cn

[J06] 计算两时间之差
来源：http://ro.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://gc.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://jw.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aj.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uv.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jb.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://nb.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://nl.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://wr.521024.cn

[J07] 比较两个日期
来源：http://bf.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://it.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wk.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rp.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xj.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ps.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pj.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://td.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://vx.shxzukj.cn

[J08] 提取年月日与星期
来源：http://kn.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yg.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ft.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vi.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vh.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://go.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kd.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ck.panjiajie.cn

[J09] 时区处理
来源：http://hm.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gu.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pt.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gt.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ti.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mm.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mp.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ep.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vq.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://kn.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lo.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sa.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zr.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://us.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rj.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pi.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://av.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iz.bookmarksfly.cn

================================================================================
来源：http://oq.gzmigu.cn

K. JSON 与序列化
来源：http://md.newstarts.cn

================================================================================
来源：http://ds.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://wl.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ea.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xy.asd995.cn

JS:   JSON.stringify(obj)
来源：http://bp.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ni.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ho.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://bf.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dm.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xi.newstarts.cn

[K02] JSON 字符串转对象
来源：http://vg.bookmarksfly.cn

Py:   json.loads(s)
来源：http://xc.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lc.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://my.newstarts.cn

TS:   JSON.parse(s)
来源：http://bh.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wz.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ax.9csxet.cn

Ruby: JSON.parse(s)
来源：http://cb.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ba.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://fm.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cl.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nz.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rx.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bw.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wk.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://am.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ou.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fd.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://xs.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jl.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eu.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ei.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ki.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yv.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fz.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wg.szxytkj.cn

[K05] 深拷贝对象
来源：http://tg.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://tk.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://dx.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ci.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://wd.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lx.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sm.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://de.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yo.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ax.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xx.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zn.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xj.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yn.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rh.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pz.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uh.shxzskj.cn

[K07] 进制转换
来源：http://ss.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ce.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jb.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://si.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uw.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ry.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uy.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bn.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hx.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://wv.colortex.cn

Py:   pickle.dumps(obj)
来源：http://lz.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nm.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://pf.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://fp.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qk.shxzukj.cn

Go:   encoding/gob
来源：http://ny.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://vn.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kn.szxytkj.cn

================================================================================
来源：http://lt.chemitech.net.cn

L. 网络请求
来源：http://kq.yuntaijiaju.cn

================================================================================
来源：http://ww.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://wz.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nk.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://re.shxzukj.cn

JS:   await fetch(url)
来源：http://fz.jctech888.com.cn

TS:   await fetch(url)
来源：http://nn.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ku.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://hf.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://en.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ae.hnjuh.cn

[L02] 发送 POST JSON
来源：http://mc.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vb.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hl.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ea.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ng.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rc.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lk.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ge.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dd.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://wp.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dj.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hl.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kt.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ou.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fw.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nn.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xs.huanxung.cn

[L04] 设置超时
来源：http://yk.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://jf.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://li.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://er.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hb.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wa.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://il.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eo.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uk.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://tm.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rm.nicolike.cn


<!-- 参考信息 -->