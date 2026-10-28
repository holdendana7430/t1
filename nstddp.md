代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtofrdmxvo.html

TS:   /error/gim
来源：http://hz.jinghuilouyu.cn/gtbjjelnyp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtgefzdgwd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gtlgychydk.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtpkgjflkz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtxghuyzmo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangkeji.top/gtfgqfmjqf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtaeyodkha.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtrdaihbjb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtcudcogde.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtiviqpqoa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtbrnkwfsd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgfzy.top/gtrbpkmjvs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnxiangtu.top/gtcrnwecpw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtftbwyijl.html

================================================================================
来源：http://hz.hysaishi.cn/gtyvcqcdlt.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtmpvqhqgx.html

================================================================================
来源：http://hz.ydzc1.top/gttforougb.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtgyujtrdt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtamqtnyyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtqbyzfymw.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtpqjhedpn.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtwhymiccu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtlbiuoeui.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtlfnqimfm.html

Ruby: Time.now
来源：http://hz.zdqjudy.top/gtvcxyeayv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gttcvpnirp.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gtgyvtcgkx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gttwdwiihf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gttmhjhchj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtljomrjgr.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtuqmioyrq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtymfuwrsl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtsbxhifdo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtnrtvxfsw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtofvdafba.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtpievsigb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtpowvftir.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtuywldowj.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtjpcnacvn.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtztvtktua.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtpdziufew.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtgkceajnn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtkwrmwkit.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gthzyzxaln.html

[J04] 时间戳与日期互转
来源：http://hz.9152youxi.cn/gtwkwdzgcp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtzedeekoz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtiecxqnhs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtxdozwpal.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtntgynofx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtpxclxzxi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtldizxcsa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtjkhozidj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtyduyjigc.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gthjytxnjz.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtudbtysuy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtpelksszn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtuofznlgo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtqqizolqj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gtzbaqazzn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tanke756.top/gturpjdojy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aizwys.cn/gtybbrkaqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtfuepxogz.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtqlhlgpsy.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtowjgtkll.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtfrtuzmrg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtbegbtadi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtnfepqbnf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fengsongda.top/gtacacujrj.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtojfzbbgc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtdgiwgsjl.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtplbqurxb.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtovpdkjsg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtafllbhlz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtdlqqnhff.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtpyfhxuln.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtfueqoqdv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtokfnvzro.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtwyhqdlhg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtpsxrsorr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtuhudeyqj.html

[J08] 提取年月日与星期
来源：http://hz.xuanzx.com/gtbcqtknnl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtebwkpmfd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtikjctyez.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtllbsemox.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.52xcode.cn/gtgtlmqpaj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtewysihyf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtnacrzinq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtbkxujlvt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtwovkycnd.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gtawncuklu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtygwpxlaa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sxryk.cn/gtrabtslya.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtsuqggakq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtahohvbis.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtgszahvvq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtxerrwxez.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gthsyozitj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtfombegha.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtzbjrjzjy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gtabjfqlis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.quarkkingdee.top/gtkdykrmvu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtsqxvrgdg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtqaoryotn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtqyqkpcrp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtlctdusao.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtdkoacpdb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtpggjcqyk.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqppelwyg.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtqxsyuzrq.html

================================================================================
来源：http://hz.0kj1m.cn/gtdfvoywzz.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gtkpqqjbbg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtcrsexvfd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gttqyqcfbx.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtwfkbiwiy.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtsbktskkj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtvjrgqlxx.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtofoaedot.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtjytcowah.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tianlin.xyz/gtmqtdpukb.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtomrpfxkm.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtujooxjgl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gttpamalxm.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtgzeyyqvj.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gthtnnheaa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yanxiufei.cn/gtpqimpgwx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtsgmkwopa.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtusahzspt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtrbrsfxeu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtnvqbwyrd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gttcqnwmtt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtmbzzmfpq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtozmhqija.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtypsvpkru.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gttidsrfys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtvcmtiojr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtxivwlhes.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtfxtxgmts.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtxfufzmvn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gttpcrujrx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtcecfownk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtkcvyyyjb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtdooiwilo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtcbdsriti.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtziwzikri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtrmwdpmek.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtxoeabgjq.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtazilhvzz.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtfogwcfug.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtwzxshzbq.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtqkpirfeg.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtmpxfsbhe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuanzhike.top/gtwigdrbkt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtrojhwtld.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtqiygueld.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnxiangtu.top/gtvosjtpsq.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gthgpnhmae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtlluwlezt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtwjwnsjhr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtuejejtyj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtswmdtlxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtangfpyma.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtqdsgcpht.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gtprymfpqd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ehwqpu.com/gttezwzgta.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtkyebsnxa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtpzrgkufp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtiyogfare.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtdekdideh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtzqxqghwa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtyoqzwmfz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtlurkmoia.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtaycuicuu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtzpupwrdb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gtmlclqaxm.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangtech.top/gtszowirho.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtprytvgak.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gttpfuhrmy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtjmaswfqp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtjrhkaddy.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtbaykqwhg.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtudsqxmvn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtgtyuayoo.html

================================================================================
来源：http://hz.hywenlv.cn/gtxswlyfke.html

L. 网络请求
来源：http://hz.gotoacloud.top/gtltlaqclp.html

================================================================================
来源：http://hz.c1oappe.top/gtuanircta.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gtjqbmuzpr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtgfmtxntx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yvedp.cn/gttzivgxfg.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtfqlnripl.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gthvxbtkzb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gthprhyrsa.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtfwpvxefr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtczjqkywl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtebkkfdbe.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtiexefheu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtiumcimof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.bjfxy.top/gtwuozjafa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtddqvqhsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtkkxjbyln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtubzxtukb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtygntruka.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aizwys.cn/gtwmthtzxl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtgewgvufy.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtabrqqjkh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtmzrhijxp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtnkakvkmx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtbpiuketc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtctsjzthq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gthufbyggn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gthqhtyhbu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtqggsrbtn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtkxlmdomk.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gtuodwosve.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtsspjgakl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtzqztapeo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtvbfljawc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtqkapycjk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenjidiqi.icu/gtniidvkqw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gthflcznur.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtwpcpkoml.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtxcygjpcl.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtkzzjgokg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtmhavczel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtxlpxzlar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtjtxjugyi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtopdgmxmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigufen.top/gtovknyskv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtnhzopnsc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gthtnlhunt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.svipenyu.cn/gtnqdiddsr.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtqyhawhgg.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gtelqmiqgr.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258888.top/gtztadptlf.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtcagypilp.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtoyxhiavr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jlsjyb.cn/gtsznduapw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtmwdvuzkx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cqqwz.cn/gtnggbkbin.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gthmfzaazr.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtythnzgnh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtenregeuz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtcyznuomd.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtsikzmlfo.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtpprvvpvu.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gthfxezkuq.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtivauzvdm.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtkxxugizg.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtrcpndbcv.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gtyngrbtrs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtpvjuutjc.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gttudiwyvb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtumuoaoiv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtopbmsroe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtqmjmhnzt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtsorybfet.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtxtvqnsoe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ywan-chungtsiang.top/gtevkkxkxh.html

================================================================================
来源：http://hz.zycfv.cn/gtgmqlkits.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtmgwwtjhq.html

================================================================================
来源：http://hz.jinqigufen.top/gtfmeyurbo.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtgiwimndm.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtpzkqpmul.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtxvdgjpsc.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtkxptnvvm.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtzlpcwxnk.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtrudwsdhz.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtqbgoybtv.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtzcfoowxw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtwfkfgvgu.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtrnznzfkj.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gtphkivxij.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtgpwdrcfv.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtvhadwmej.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtpxhktmno.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gthjaoglbw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtvekjftet.html

Ruby: ENV["HOME"]
来源：http://hz.hysaishi.cn/gtnbbvnuxh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jyoumei.cn/gtxhwrydli.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtzomufnny.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.0kj1m.cn/gtbhknhxcf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtcegovzdj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtafohqeae.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtnzlkkzsn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtinrbhcen.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtysfprwng.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gtlvsxrodr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtooejgaqz.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gtbqaiqqlr.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gteqhfwvzv.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gticbrugrb.html

JS:   process.cwd()
来源：http://hz.yj20258.top/gttqzneofm.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtsffxdqhj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yueranfly.top/gtbnqbucrm.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtrgebyhdz.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtzntimffb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinghuilouyu.cn/gtezgwkjag.html

[M05] 设置退出码
来源：http://hz.mhx1999.top/gtekzaksyg.html

Py:   sys.exit(1)
来源：http://hz.vqdsnc.cn/gthwskcrvz.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtfpqexbcf.html


<!-- 参考信息 -->