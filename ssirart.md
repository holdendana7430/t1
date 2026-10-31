代发 wailian999

================================================================================
来源：http://te.nszjky.cn

I. 正则表达式
来源：http://jq.newstarts.cn

================================================================================
来源：http://bj.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://vc.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kf.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gk.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://hh.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://dt.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xs.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ge.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://va.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hb.521024.cn

[I02] 提取所有匹配
来源：http://rm.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://fw.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ot.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rx.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://en.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hc.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yf.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://jd.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zf.yuexingan06.cn

[I03] 提取捕获分组
来源：http://kk.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ri.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kn.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kx.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://le.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://az.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fp.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pm.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gh.bookmarksfly.cn

[I04] 正则替换
来源：http://dt.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cd.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mj.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ty.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rj.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gm.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qo.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zq.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qu.wgjwhj.cn

[I05] 按正则拆分
来源：http://mr.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rf.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mj.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://nq.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://cx.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://ka.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gw.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fm.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xi.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aw.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eh.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eo.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fz.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cv.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kb.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gb.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bv.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://im.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://jo.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xf.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vp.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xq.jctech888.com.cn

TS:   /error/gim
来源：http://nq.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://as.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yx.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://cg.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ur.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://hk.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cw.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cb.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xr.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yr.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ya.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gv.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gg.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ld.chemitech.net.cn

================================================================================
来源：http://zt.hnjuh.cn

J. 日期与时间
来源：http://gj.521024.cn

================================================================================
来源：http://na.haigaiapp.cn

[J01] 获取当前时间
来源：http://vg.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sr.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cr.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://cx.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://ue.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dr.shxzskj.cn

Go:   time.Now()
来源：http://gf.newstarts.cn

Ruby: Time.now
来源：http://qh.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qu.lnxyls.cn

[J02] 格式化输出
来源：http://sa.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gt.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cn.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dt.chemitech.net.cn

TS:   d.toISOString()
来源：http://df.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pk.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vt.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bb.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xz.nszjky.cn

[J03] 字符串解析为日期
来源：http://yi.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://es.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vp.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://rp.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://xb.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sy.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sl.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://ph.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wd.huanxung.cn

[J04] 时间戳与日期互转
来源：http://tb.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lz.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oz.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uq.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ax.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cj.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xo.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://so.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://av.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ni.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://xs.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xk.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jc.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lv.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://jv.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oc.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://oj.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ck.gzmigu.cn

[J06] 计算两时间之差
来源：http://vc.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://um.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://fx.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://la.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wq.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kv.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://nz.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://bp.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://xf.shtwfgs.cn

[J07] 比较两个日期
来源：http://so.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://jv.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dm.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://is.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hm.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fb.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vd.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gk.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://eg.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://ec.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rk.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mt.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mr.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://np.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tq.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fq.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eh.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sy.yuntaijiaju.cn

[J09] 时区处理
来源：http://oe.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ke.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lq.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bl.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zi.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cc.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://is.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gc.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iq.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://od.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yu.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uc.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pc.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mc.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ad.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vk.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bg.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.szxytkj.cn

================================================================================
来源：http://ww.bookmarksfly.cn

K. JSON 与序列化
来源：http://hp.bookmarksfly.cn

================================================================================
来源：http://hp.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://sc.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://by.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ey.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ai.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://fp.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ym.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://fp.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lp.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nq.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://un.huixiangedu.cn

Py:   json.loads(s)
来源：http://oq.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vd.huanxung.cn

JS:   JSON.parse(s)
来源：http://to.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://oc.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cn.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://cr.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ax.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jq.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://xn.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nu.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hd.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zf.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ex.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bj.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ae.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oy.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yp.huanxung.cn

[K04] 读取 JSON 文件
来源：http://ry.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fj.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fj.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ng.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rn.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mp.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xi.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ao.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zw.lnxyls.cn

[K05] 深拷贝对象
来源：http://cy.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://qb.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://jc.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://yr.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://jt.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://as.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zm.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kh.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wl.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ja.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dc.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aj.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xf.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jp.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ww.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uy.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vm.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sg.hnjuh.cn

[K07] 进制转换
来源：http://vd.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://od.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yj.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ko.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mp.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ln.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ty.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ve.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wt.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://bu.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://fw.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lo.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://rm.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ih.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cr.521024.cn

Go:   encoding/gob
来源：http://ue.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://ql.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ke.haigaiapp.cn

================================================================================
来源：http://yf.shxzukj.cn

L. 网络请求
来源：http://qr.panjiajie.cn

================================================================================
来源：http://vd.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://ob.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pp.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hf.huanxung.cn

JS:   await fetch(url)
来源：http://gs.wgjwhj.cn

TS:   await fetch(url)
来源：http://rt.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ys.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://gt.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vl.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zn.asd995.cn

[L02] 发送 POST JSON
来源：http://iw.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xj.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ad.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bj.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kl.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cx.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dg.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dh.lnxyls.cn

[L03] 设置自定义请求头
来源：http://xi.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fg.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rh.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xx.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vn.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rp.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tw.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pv.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wk.jianghongdianzi.cn

[L04] 设置超时
来源：http://kz.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://vy.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jn.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wh.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jm.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qq.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rk.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ay.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ex.szsharing.cn

[L05] 上传文件（multipart）
来源：http://dm.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uw.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rj.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gp.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iz.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sd.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wt.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vh.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://no.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://ot.haigaiapp.cn

Py:   resp.json()
来源：http://sy.huanxung.cn

PHP:  json_decode($body, true);
来源：http://rb.nicolike.cn

JS:   await resp.json()
来源：http://gd.huixinmuqiang.cn

TS:   await resp.json()
来源：http://xf.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://re.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://os.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://bi.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tf.lnxyls.cn


<!-- 参考信息 -->