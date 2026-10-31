代发 wailian999

================================================================================
来源：http://zb.newstarts.cn

I. 正则表达式
来源：http://ok.panjiajie.cn

================================================================================
来源：http://fn.gzmigu.cn

[I01] 判断是否匹配
来源：http://me.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ls.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xw.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://th.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://iz.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bw.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fc.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://dr.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tc.shxzukj.cn

[I02] 提取所有匹配
来源：http://bs.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://it.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hh.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gj.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://rs.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ln.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pb.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://cz.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ns.szsharing.cn

[I03] 提取捕获分组
来源：http://jo.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xr.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ua.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sd.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uf.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hq.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gl.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pv.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rs.jianghongdianzi.cn

[I04] 正则替换
来源：http://ar.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ue.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ca.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dn.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ku.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bi.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://et.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pt.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ic.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://jp.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dj.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nk.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ob.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://kj.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://tj.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iu.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pm.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vm.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nb.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xu.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xx.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wd.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vd.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qf.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zy.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ar.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zq.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://bl.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vn.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tg.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uh.lnxyls.cn

TS:   /error/gim
来源：http://vn.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://se.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hn.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://au.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://in.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://hv.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fr.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ey.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jr.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bq.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ia.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hy.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eo.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nh.huixiangedu.cn

================================================================================
来源：http://jl.nszjky.cn

J. 日期与时间
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://re.9csxet.cn

[J01] 获取当前时间
来源：http://nv.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yb.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ln.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://da.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://ah.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yq.wgjwhj.cn

Go:   time.Now()
来源：http://bh.jianghongdianzi.cn

Ruby: Time.now
来源：http://co.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qk.jctech888.com.cn

[J02] 格式化输出
来源：http://zz.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fh.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ab.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fs.chemitech.net.cn

TS:   d.toISOString()
来源：http://mq.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yk.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rm.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fm.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pe.panjiajie.cn

[J03] 字符串解析为日期
来源：http://jp.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fk.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tc.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://is.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ko.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bz.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wi.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://kt.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xw.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://lx.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mr.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rh.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jw.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bd.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ea.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ne.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pe.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lj.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://rq.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://rf.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cf.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://df.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://su.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ar.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yy.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://uv.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://le.huixiangedu.cn

[J06] 计算两时间之差
来源：http://aq.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://rt.521024.cn

PHP:  $end->diff($start)->days;
来源：http://gd.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lr.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://av.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://al.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://gq.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://os.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://bv.gzmigu.cn

[J07] 比较两个日期
来源：http://mk.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://he.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://np.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ee.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zm.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tv.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pg.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sa.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://it.newstarts.cn

[J08] 提取年月日与星期
来源：http://qu.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hi.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rb.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sv.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pp.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cp.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oc.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yb.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.shxzskj.cn

[J09] 时区处理
来源：http://bk.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hh.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ty.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hk.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ic.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bd.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pf.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cw.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gl.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://tc.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lw.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ov.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gf.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://la.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yy.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oe.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://km.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pc.gzmigu.cn

================================================================================
来源：http://up.shxzskj.cn

K. JSON 与序列化
来源：http://te.521024.cn

================================================================================
来源：http://wt.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://ei.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://or.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kt.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://sb.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://tt.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nj.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://rq.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kz.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://un.newstarts.cn

[K02] JSON 字符串转对象
来源：http://td.muxihuayi.cn

Py:   json.loads(s)
来源：http://ct.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ac.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://gb.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://xd.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bh.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ht.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://ix.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cw.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xs.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xq.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wf.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pq.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cw.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wq.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kg.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://zu.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pz.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ub.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tu.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tb.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jd.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rq.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nf.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lf.bjjhwx.cn

[K05] 深拷贝对象
来源：http://oe.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://zm.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ru.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://rc.panjiajie.cn

TS:   structuredClone(obj)
来源：http://rz.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://py.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bn.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://or.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tk.521024.cn

[K06] 解析 URL 查询串
来源：http://zf.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ox.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ba.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kq.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jz.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gd.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nj.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oh.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dx.nicolike.cn

[K07] 进制转换
来源：http://kh.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ew.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wx.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zc.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fh.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vv.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wl.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ak.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sy.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://wz.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://iy.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xd.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://xk.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://zr.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uo.gzmigu.cn

Go:   encoding/gob
来源：http://vp.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://gp.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qd.huixiangedu.cn

================================================================================
来源：http://gt.shxzukj.cn

L. 网络请求
来源：http://xk.wgjwhj.cn

================================================================================
来源：http://pv.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://bf.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kg.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mm.hahajie.cn

JS:   await fetch(url)
来源：http://tz.shxzskj.cn

TS:   await fetch(url)
来源：http://wx.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xz.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://zu.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ro.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xd.asd995.cn

[L02] 发送 POST JSON
来源：http://cl.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yt.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ql.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gp.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aa.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iq.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oe.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://al.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ny.newstarts.cn

[L03] 设置自定义请求头
来源：http://xi.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ar.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://me.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rp.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://id.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://il.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mk.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fc.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nk.shxzskj.cn

[L04] 设置超时
来源：http://fy.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://kv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://na.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ho.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nl.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tq.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ys.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ax.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ix.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://rs.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tj.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hc.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yz.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ng.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jd.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zf.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ve.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jf.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://dx.nszjky.cn

Py:   resp.json()
来源：http://sg.asd995.cn

PHP:  json_decode($body, true);
来源：http://qf.shxzskj.cn

JS:   await resp.json()
来源：http://yv.szxytkj.cn

TS:   await resp.json()
来源：http://mj.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nn.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kv.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://tl.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qb.szxytkj.cn


<!-- 参考信息 -->