代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hh.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pu.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wr.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://fw.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gs.shxzskj.cn

[I03] 提取捕获分组
来源：http://ls.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rm.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zz.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://is.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jz.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gr.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xv.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tt.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jf.yuexingan06.cn

[I04] 正则替换
来源：http://tl.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qk.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mj.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yd.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cn.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cp.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hj.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bn.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.szsharing.cn

[I05] 按正则拆分
来源：http://ti.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wf.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ih.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://vd.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://up.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://gv.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dl.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://om.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://du.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ww.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sl.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vo.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sq.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://id.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qp.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kx.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oh.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://gc.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zn.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lx.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lk.hahajie.cn

TS:   /error/gim
来源：http://ta.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://li.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ic.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://px.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dz.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://oa.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ui.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ue.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gg.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pi.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ms.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://io.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ma.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zo.szxytkj.cn

================================================================================
来源：http://en.nicolike.cn

J. 日期与时间
来源：http://ir.asd995.cn

================================================================================
来源：http://vb.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://aq.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ue.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://da.asd995.cn

JS:   new Date();  Date.now()
来源：http://bz.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://hv.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://me.yuexingan06.cn

Go:   time.Now()
来源：http://yg.yuntaijiaju.cn

Ruby: Time.now
来源：http://xf.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oo.9csxet.cn

[J02] 格式化输出
来源：http://qb.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://od.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fk.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rt.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://kv.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zb.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ct.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vh.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ah.szsharing.cn

[J03] 字符串解析为日期
来源：http://ii.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gt.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ul.colortex.cn

JS:   new Date("2024-01-02")
来源：http://lj.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://by.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wk.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aw.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ga.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dr.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://an.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ei.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://no.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dw.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xq.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cn.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ri.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mb.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nm.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://ed.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://en.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://er.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mj.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wi.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://kn.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vq.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://uc.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fz.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ed.asd995.cn

Py:   (end - start).total_seconds()
来源：http://vs.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://tr.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cl.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ak.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wm.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://nh.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://ul.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://kg.huixiangedu.cn

[J07] 比较两个日期
来源：http://rd.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://sf.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wb.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qm.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ry.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sh.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://th.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wy.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://vn.huanxung.cn

[J08] 提取年月日与星期
来源：http://be.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kf.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ms.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://je.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ev.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ja.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gz.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vu.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vl.panjiajie.cn

[J09] 时区处理
来源：http://aq.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://la.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lh.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lu.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bn.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fs.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cf.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ta.521024.cn

[J10] 取今天 / 本月第一天
来源：http://kn.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://md.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uw.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kw.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ym.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hm.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zq.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jf.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xr.panjiajie.cn

================================================================================
来源：http://xi.nszjky.cn

K. JSON 与序列化
来源：http://cb.shxzukj.cn

================================================================================
来源：http://rr.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://ji.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qr.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://md.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://yh.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://lv.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yl.newstarts.cn

Go:   json.Marshal(obj)
来源：http://dt.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vi.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gj.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://rj.jctech888.com.cn

Py:   json.loads(s)
来源：http://pv.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oy.nszjky.cn

JS:   JSON.parse(s)
来源：http://ah.nszjky.cn

TS:   JSON.parse(s)
来源：http://do.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bz.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://sq.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://bo.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fz.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://iy.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qb.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ar.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zb.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jk.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mh.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hs.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ul.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rj.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://hc.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tx.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://st.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cg.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hh.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mr.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pi.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yx.hahajie.cn

[K05] 深拷贝对象
来源：http://ik.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://yn.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://yi.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://to.szsharing.cn

TS:   structuredClone(obj)
来源：http://je.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sp.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kg.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wx.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wr.9csxet.cn

[K06] 解析 URL 查询串
来源：http://ej.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fh.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cx.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tc.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nn.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iy.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sl.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hg.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ec.asd995.cn

[K07] 进制转换
来源：http://lw.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fa.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cc.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fg.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ek.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uh.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tg.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://so.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nb.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://lu.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://tv.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hi.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://as.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ho.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ja.jianghongdianzi.cn

Go:   encoding/gob
来源：http://vm.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://ai.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yf.jctech888.com.cn

================================================================================
来源：http://na.szsharing.cn

L. 网络请求
来源：http://cc.chemitech.net.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://ga.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ic.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bx.bjjhwx.cn

JS:   await fetch(url)
来源：http://wf.wgjwhj.cn

TS:   await fetch(url)
来源：http://xo.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ic.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://hd.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xx.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yj.521024.cn

[L02] 发送 POST JSON
来源：http://up.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oh.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://am.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gp.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sp.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://po.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bm.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mq.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://za.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ie.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://um.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fh.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sz.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://it.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iq.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://db.muxihuayi.cn

[L04] 设置超时
来源：http://ho.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://us.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bt.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xw.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mt.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sh.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wk.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bt.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://fs.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yt.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zb.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pf.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://al.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gs.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://io.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rf.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://go.wgjwhj.cn

Py:   resp.json()
来源：http://tn.szsharing.cn

PHP:  json_decode($body, true);
来源：http://hs.szsharing.cn

JS:   await resp.json()
来源：http://tu.haigaiapp.cn

TS:   await resp.json()
来源：http://di.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ks.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vv.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://im.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iz.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://ka.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://og.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ea.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://oo.asd995.cn

TS:   resp.ok;  resp.status
来源：http://fe.521024.cn

Java: resp.statusCode()
来源：http://gf.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://wd.shxzskj.cn

Ruby: resp.code.to_i
来源：http://eb.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://yn.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ji.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yd.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://ld.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xo.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jj.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jv.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kg.nicolike.cn


<!-- 参考信息 -->