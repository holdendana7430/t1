代发 wailian999

JS:   e.message;  e.stack
来源：http://fj.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eq.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uf.shxzskj.cn

Go:   err.Error()
来源：http://sf.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://cy.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://wt.hnjuh.cn

[H09] 带错误码的异常
来源：http://zr.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vd.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xi.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ae.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vs.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pu.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gy.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sm.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ec.shxzukj.cn

[H10] 资源自动释放
来源：http://ng.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://re.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ud.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wh.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qh.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ta.szxytkj.cn

Go:   defer f.Close()
来源：http://kz.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tf.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://av.bookmarksfly.cn

================================================================================
来源：http://ne.panjiajie.cn

I. 正则表达式
来源：http://cq.shxzskj.cn

================================================================================
来源：http://hs.shxzskj.cn

[I01] 判断是否匹配
来源：http://dd.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ww.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://px.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://wc.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://gj.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qs.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iw.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://ro.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://db.szxytkj.cn

[I02] 提取所有匹配
来源：http://gu.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://mj.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mj.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hi.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://xp.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ur.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hn.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://sw.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ab.chemitech.net.cn

[I03] 提取捕获分组
来源：http://bc.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sp.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zk.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://su.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kt.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qy.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://da.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://be.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qc.hahajie.cn

[I04] 正则替换
来源：http://uc.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://is.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ix.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rj.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pk.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://my.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mz.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fz.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ui.wgjwhj.cn

[I05] 按正则拆分
来源：http://as.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bs.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://zf.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wv.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://pr.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iu.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qu.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ya.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fq.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fu.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rb.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://py.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wl.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qs.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fk.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bo.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://md.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sl.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dv.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ca.hahajie.cn

TS:   /error/gim
来源：http://tl.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yp.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://np.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://zx.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fb.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://lc.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hc.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ay.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cd.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bg.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fo.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ya.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nu.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wh.nicolike.cn

================================================================================
来源：http://wb.panjiajie.cn

J. 日期与时间
来源：http://pa.shtwfgs.cn

================================================================================
来源：http://cw.nicolike.cn

[J01] 获取当前时间
来源：http://pl.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yb.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zu.nszjky.cn

JS:   new Date();  Date.now()
来源：http://va.colortex.cn

TS:   new Date();  Date.now()
来源：http://jh.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zk.newstarts.cn

Go:   time.Now()
来源：http://sr.hnjuh.cn

Ruby: Time.now
来源：http://rr.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yx.yuntaijiaju.cn

[J02] 格式化输出
来源：http://pu.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nd.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://og.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.szsharing.cn

TS:   d.toISOString()
来源：http://fu.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ep.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ou.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vq.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hm.hnjuh.cn

[J03] 字符串解析为日期
来源：http://pp.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://up.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xd.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://bv.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ny.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zj.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vu.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://fy.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cy.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ao.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://er.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wk.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ac.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pk.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://od.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iw.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ru.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rt.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://hr.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://fm.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xj.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wy.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dt.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://wa.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pp.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://mi.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ov.asd995.cn

[J06] 计算两时间之差
来源：http://dn.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://vm.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://vv.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lu.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qt.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xb.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://xj.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://gj.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://vb.chemitech.net.cn

[J07] 比较两个日期
来源：http://dn.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://ph.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iw.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ec.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tc.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dg.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yx.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ot.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://sh.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://vv.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wn.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dd.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ef.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ev.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ih.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tm.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jk.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ev.gzmigu.cn

[J09] 时区处理
来源：http://bb.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ti.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pt.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bn.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bq.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nw.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mm.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uy.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eo.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://bj.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eq.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kt.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kn.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://af.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bp.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tv.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://db.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cy.szxytkj.cn

================================================================================
来源：http://wp.chemitech.net.cn

K. JSON 与序列化
来源：http://qw.gzmigu.cn

================================================================================
来源：http://ve.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://pb.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pn.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zy.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://dq.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://iq.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nx.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://gh.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zk.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lg.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ql.chemitech.net.cn

Py:   json.loads(s)
来源：http://od.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fs.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://ps.asd995.cn

TS:   JSON.parse(s)
来源：http://bu.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xr.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://sc.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://cj.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fg.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lq.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lt.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://va.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rm.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://br.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pd.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mz.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nr.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://qk.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vj.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hn.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sd.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lg.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://an.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cx.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wj.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tw.jctech888.com.cn

[K05] 深拷贝对象
来源：http://jj.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://qp.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://cb.hahajie.cn

JS:   structuredClone(obj)
来源：http://qs.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://gd.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hf.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dz.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pv.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pg.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ya.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bm.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://di.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fy.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tx.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lx.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ky.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zm.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rq.huixinmuqiang.cn

[K07] 进制转换
来源：http://wi.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hf.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qa.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ft.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dr.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pm.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pg.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qc.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fk.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://bt.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://ek.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kh.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://ml.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://ey.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hu.gzmigu.cn

Go:   encoding/gob
来源：http://zh.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://yv.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://um.shxzskj.cn

================================================================================
来源：http://yz.haigaiapp.cn

L. 网络请求
来源：http://vh.lnxyls.cn

================================================================================
来源：http://vb.newstarts.cn

[L01] 发送 GET 请求
来源：http://sv.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uh.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vw.9csxet.cn

JS:   await fetch(url)
来源：http://gu.szsharing.cn

TS:   await fetch(url)
来源：http://vd.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uw.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://jz.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bp.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mn.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ay.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://je.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jn.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pq.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sn.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ro.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bz.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zl.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://de.gzmigu.cn

[L03] 设置自定义请求头
来源：http://za.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zn.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eg.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fa.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ol.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jo.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jx.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wl.gzmigu.cn

[L04] 设置超时
来源：http://ly.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://sx.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pe.gzmigu.cn


<!-- 参考信息 -->