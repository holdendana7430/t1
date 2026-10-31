代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ov.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wf.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ju.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ke.szsharing.cn

[I02] 提取所有匹配
来源：http://jw.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://gl.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nz.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mu.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://nr.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hr.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xx.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://rd.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ti.9csxet.cn

[I03] 提取捕获分组
来源：http://fx.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mc.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ja.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ky.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ia.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uz.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jf.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fx.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zf.huanxung.cn

[I04] 正则替换
来源：http://hy.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pk.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lx.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nf.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nc.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rw.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qj.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ac.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ja.colortex.cn

[I05] 按正则拆分
来源：http://oc.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yp.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eb.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://xp.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://sr.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://tc.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wx.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hv.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tk.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ah.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nk.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bs.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rb.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zt.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bv.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://za.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jq.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ay.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://ou.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vf.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ao.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ps.shxzukj.cn

TS:   /error/gim
来源：http://qe.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gj.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ra.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://fx.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fe.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://op.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://su.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rs.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fh.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hy.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pf.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wu.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kl.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wt.huixiangedu.cn

================================================================================
来源：http://nd.huixinmuqiang.cn

J. 日期与时间
来源：http://eh.muxihuayi.cn

================================================================================
来源：http://zx.nszjky.cn

[J01] 获取当前时间
来源：http://kd.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gr.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eo.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://bf.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ou.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://og.asd995.cn

Go:   time.Now()
来源：http://po.huanxung.cn

Ruby: Time.now
来源：http://ov.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://em.jianghongdianzi.cn

[J02] 格式化输出
来源：http://lq.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wk.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qt.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gu.shxzskj.cn

TS:   d.toISOString()
来源：http://ni.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pt.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lp.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jx.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jz.shxzskj.cn

[J03] 字符串解析为日期
来源：http://ok.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zl.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oa.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://qq.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://le.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jp.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nd.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://cd.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tv.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://aa.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lu.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ib.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yv.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xl.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zq.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://al.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lo.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://su.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://oz.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://wj.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://id.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qd.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://wu.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://al.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://qt.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kg.bjjhwx.cn

[J06] 计算两时间之差
来源：http://fc.asd995.cn

Py:   (end - start).total_seconds()
来源：http://cu.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://xd.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gz.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hn.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zf.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://mo.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://av.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ug.bookmarksfly.cn

[J07] 比较两个日期
来源：http://eb.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://nk.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://re.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vm.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rt.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zl.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nv.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tl.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://dr.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://hd.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ri.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qp.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gs.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mz.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://et.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rw.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ca.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wl.haigaiapp.cn

[J09] 时区处理
来源：http://gn.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sc.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ze.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vl.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uk.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ux.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://be.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xn.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vm.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://sj.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uf.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fz.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hx.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zc.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tg.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wm.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qg.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ht.bookmarksfly.cn

================================================================================
来源：http://ed.shxzukj.cn

K. JSON 与序列化
来源：http://ib.shxzukj.cn

================================================================================
来源：http://ka.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://rf.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gc.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eb.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://vo.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://jw.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sm.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://gt.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mf.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://rh.wgjwhj.cn

Py:   json.loads(s)
来源：http://pt.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xp.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://fq.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://zr.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ci.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://zs.szsharing.cn

Ruby: JSON.parse(s)
来源：http://ap.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gl.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://oa.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rf.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ea.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kn.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ot.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uf.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vu.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sv.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://ho.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cv.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qp.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kh.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pr.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vo.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fl.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ud.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qn.wgjwhj.cn

[K05] 深拷贝对象
来源：http://sh.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://fw.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://go.hnjuh.cn

JS:   structuredClone(obj)
来源：http://fw.gzmigu.cn

TS:   structuredClone(obj)
来源：http://sg.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://or.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zt.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ja.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jm.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://zy.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zu.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ph.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pd.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tq.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ok.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sl.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pw.jctech888.com.cn

[K07] 进制转换
来源：http://xe.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cb.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pv.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yd.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ey.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ss.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jw.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aa.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://nq.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://ea.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gg.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hk.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://rt.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pi.asd995.cn

Go:   encoding/gob
来源：http://ul.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://yj.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://if.huixiangedu.cn

================================================================================
来源：http://ip.yuntaijiaju.cn

L. 网络请求
来源：http://ff.yuntaijiaju.cn

================================================================================
来源：http://wd.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ei.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ww.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gs.hahajie.cn

JS:   await fetch(url)
来源：http://ox.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://wd.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ky.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://pb.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://et.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ov.nicolike.cn

[L02] 发送 POST JSON
来源：http://qt.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lh.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pl.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zz.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yv.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ad.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qx.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mu.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://rn.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dd.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ua.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rv.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nr.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bt.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dp.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sj.lnxyls.cn

[L04] 设置超时
来源：http://bb.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://fg.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vk.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bt.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ze.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://db.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jc.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yi.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ns.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://dn.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jn.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mc.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zm.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nc.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gk.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://df.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tz.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ak.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://vo.521024.cn

Py:   resp.json()
来源：http://kz.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://gg.nicolike.cn

JS:   await resp.json()
来源：http://hl.521024.cn

TS:   await resp.json()
来源：http://gv.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wt.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ba.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://on.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xd.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://cj.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ek.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bm.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://et.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://pe.yuexingan06.cn

Java: resp.statusCode()
来源：http://nm.colortex.cn

Go:   resp.StatusCode
来源：http://im.nszjky.cn

Ruby: resp.code.to_i
来源：http://vx.asd995.cn


<!-- 参考信息 -->