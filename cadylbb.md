代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fe.szsharing.cn

[I03] 提取捕获分组
来源：http://ra.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://we.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qn.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://io.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vb.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hb.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pn.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qx.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hy.huixiangedu.cn

[I04] 正则替换
来源：http://oh.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://im.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ln.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wf.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ld.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oo.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ik.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kd.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://od.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://vl.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lm.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://do.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ta.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nm.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://oe.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sn.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xi.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wz.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ki.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wv.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://df.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cd.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dg.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xv.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tl.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oj.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://qh.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nf.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ca.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kd.shtwfgs.cn

TS:   /error/gim
来源：http://sv.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nk.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vt.colortex.cn

Ruby: s.scan(/error/i)
来源：http://wo.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jf.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://ph.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ea.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dd.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bu.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ct.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wx.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kl.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lt.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mi.shxzukj.cn

================================================================================
来源：http://xi.huixiangedu.cn

J. 日期与时间
来源：http://so.nszjky.cn

================================================================================
来源：http://ge.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://zi.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bq.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aj.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://rc.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ge.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kv.lnxyls.cn

Go:   time.Now()
来源：http://mp.hahajie.cn

Ruby: Time.now
来源：http://xc.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dm.nicolike.cn

[J02] 格式化输出
来源：http://vn.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mz.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rf.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gm.gzmigu.cn

TS:   d.toISOString()
来源：http://dd.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fo.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bi.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xc.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lj.shxzskj.cn

[J03] 字符串解析为日期
来源：http://wb.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xd.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cx.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://wr.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://op.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ef.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dk.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://xy.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vq.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://rs.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cc.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://md.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cv.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wf.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ay.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hq.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rc.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zc.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://wt.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://ii.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rp.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nl.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xm.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://eq.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yv.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://er.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vv.wgjwhj.cn

[J06] 计算两时间之差
来源：http://kw.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://ez.521024.cn

PHP:  $end->diff($start)->days;
来源：http://sn.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://am.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cv.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mi.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://dm.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://fd.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://mz.521024.cn

[J07] 比较两个日期
来源：http://ew.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://un.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sf.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vt.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hs.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ay.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tt.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bt.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ov.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ny.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nr.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yb.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xx.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bz.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jc.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lc.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gy.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pz.shxzskj.cn

[J09] 时区处理
来源：http://rh.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kt.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zi.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pk.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yh.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rf.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jp.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://du.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://km.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://iu.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gi.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ax.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rv.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://or.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aj.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oz.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://my.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ok.hnjuh.cn

================================================================================
来源：http://qu.szsharing.cn

K. JSON 与序列化
来源：http://xs.yuntaijiaju.cn

================================================================================
来源：http://tu.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://tr.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ov.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ek.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://gu.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://ss.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ou.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ck.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://un.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yw.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://ar.huixiangedu.cn

Py:   json.loads(s)
来源：http://mh.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://wd.panjiajie.cn

TS:   JSON.parse(s)
来源：http://cr.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ku.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://bw.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://oe.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bo.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://gx.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fn.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rj.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hx.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mn.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fa.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kk.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ow.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qz.huanxung.cn

[K04] 读取 JSON 文件
来源：http://dp.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kp.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wp.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ng.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kf.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vt.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ck.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fz.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gn.huanxung.cn

[K05] 深拷贝对象
来源：http://vi.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://qr.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://wf.newstarts.cn

JS:   structuredClone(obj)
来源：http://ar.nszjky.cn

TS:   structuredClone(obj)
来源：http://xq.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hk.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ck.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vk.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dv.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://hi.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jy.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nd.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uf.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iv.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ju.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://je.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ot.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cw.shxzukj.cn

[K07] 进制转换
来源：http://dz.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wz.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ys.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yz.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://in.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://up.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cs.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rv.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sd.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://ax.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://fh.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qu.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://em.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://yb.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hj.panjiajie.cn

Go:   encoding/gob
来源：http://ra.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ey.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uq.wgjwhj.cn

================================================================================
来源：http://xl.yuexingan06.cn

L. 网络请求
来源：http://ks.jianghongdianzi.cn

================================================================================
来源：http://cc.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://hw.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nz.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zg.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://fv.shxzukj.cn

TS:   await fetch(url)
来源：http://kp.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dj.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://gt.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tp.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hp.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://vd.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bc.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qh.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kb.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sv.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oj.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xl.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pb.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fl.shxzukj.cn

[L03] 设置自定义请求头
来源：http://xd.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sw.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ig.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ps.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jn.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ia.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://by.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gt.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yv.huanxung.cn

[L04] 设置超时
来源：http://oq.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://nn.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bc.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://di.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pw.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vb.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fj.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mp.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://df.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://vo.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bf.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nk.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mo.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zh.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://am.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uo.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ny.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lu.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://gl.bjjhwx.cn

Py:   resp.json()
来源：http://ut.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://nw.yuntaijiaju.cn

JS:   await resp.json()
来源：http://fe.huanxung.cn

TS:   await resp.json()
来源：http://bm.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nx.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ha.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://va.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wb.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://wr.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ct.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jh.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://al.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://bt.hnjuh.cn

Java: resp.statusCode()
来源：http://if.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://qw.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://df.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://sn.gzmigu.cn

[L08] 并发请求多个地址
来源：http://wx.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ay.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://do.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ke.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://if.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yr.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bk.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ex.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aw.nszjky.cn

================================================================================
来源：http://jq.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://ya.haigaiapp.cn


<!-- 参考信息 -->