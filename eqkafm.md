代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtzatsxayh.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtlwxrtckm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtpxvycrjc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtkwkedziu.html

Ruby: s.scan(/error/i)
来源：http://hz.gaohongyu789.top/gtmvndbxfv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cashguo.top/gtkzykceho.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtwktcgygw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gtbdfyqpza.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtxhjkucpn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtyibocvsm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtulqsglxd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gzhubu.top/gtbpidgumh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtoqgxibeh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gthuyeexui.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtchwxtabm.html

================================================================================
来源：http://hz.vqdsnc.cn/gttixwtzhq.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gttckqfzwt.html

================================================================================
来源：http://hz.yuxming.cn/gtjztskxqy.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtjduonvwi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtmvrntqjy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtmbwnsfsf.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gttwvsyeej.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtwoligppz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtkjapftgr.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtfxnlvjfq.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtujcarjop.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gthtxtbcud.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtnixoelgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtbogdmeqa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtdjextxxx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtmlvvmzex.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtxmtxqojd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sufxvd.cn/gtaflaoqij.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtwnrrzitj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtpsamjeng.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtftkhieih.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gtblqwudgh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gthadbopvz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtpjswetyo.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtzmvcmekr.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gthagrxvoh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtmkzipjrk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtwczwafhr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtstfqaopj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtuuzcyxrj.html

[J04] 时间戳与日期互转
来源：http://hz.dashuyun.cn/gtqcizjxgw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtyrefrvdg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gthijvcopl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gtlwfgjodk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtjllfaifb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtsyjdhtez.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtoltyluwi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtwclrpsgx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtnjjksyha.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtubrrelku.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtnfdaibdj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tianlin.xyz/gtpmzqikya.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtqnuqcmfw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtzuqrkmxs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtpavtebuh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtpyfrhlwd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtargoakfm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dianchejie.cn/gtpejffqps.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gttzrehtyz.html

Py:   (end - start).total_seconds()
来源：http://hz.0kj1m.cn/gtannlpkht.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtywmmqmpg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtbhgbugns.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtlwkswavd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigfzy.top/gtghtcjeez.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtrbtsiqsp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtzesponku.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258.top/gttaoqmxwa.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtwwvrlbbo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtmyozaini.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtwelubqnp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtsbtjlfqm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtaptktrbf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtihbcnyat.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gthimdxlmr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtfmucgqyc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtcuzvpmzd.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtqeendpbr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtijaqrpwf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtjpwxpwgs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtktnfgcdn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gtzqyecmgo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xziqi.cn/gtckddygks.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gtemsnvgla.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtigtxcqfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtdqiewqyu.html

[J09] 时区处理
来源：http://hz.shangyingyoupin.top/gtloojvgmf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gthshrbulx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sufxvd.cn/gtzmwbfzrq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtashzggga.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtgdpmxxgk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jianghu66.top/gtksmgxdqm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtdbishfgj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gaohongyu789.top/gtvehswtpj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gtskkazcbb.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtclhevpia.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xylfe.cn/gtxnenqsaz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hongshengwenyu.top/gtdhhaxryi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtadtxccqd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hnqzz.top/gtboajzgaj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtdvhqjmlm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gtpkdkatdr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.haohaochexian.top/gtcshgtcmy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yangfankeji.com/gtmclqohqy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrhhgoada.html

K. JSON 与序列化
来源：http://hz.ydzc1.top/gtakrikjto.html

================================================================================
来源：http://hz.andypj.xyz/gtrcislsdj.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gtppzfsntn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtnxyubanl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtiuirftfd.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtsnyqqpof.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gttetdwheb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtnkpmabdp.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtyowrireh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtfjgintsx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtvmavbley.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtzwaimvmv.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtldintmyb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtugehqcim.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtjdclelpb.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtdizwcplu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtjqoasmxk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtutjiabfu.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258888.top/gteeicbvpl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtcbhyffwi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtsjpzxehb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtdojitgqq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtkuiacmce.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtjdzfvcll.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtotieiviu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gtimkdyrvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtjuyzhpgr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cheryme.top/gttvaqlclc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtdwmcdltc.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtevzxsvpo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtrdgtpnbl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gthohujhfw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtntykzaxr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gticoyrlgx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtmphqaedu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtukmkfdjd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtdcleitlk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtyxsdvfhh.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtkscipssl.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtnzfxxtkd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtlmagslds.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gteegokmjj.html

TS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtdeyftjph.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtphvnwunu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtrfcppdib.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtckueqewe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtgfpfafqd.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gttdcenybg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtgxatbapd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gtyvxwtstk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtdtruqmgu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gturghkvdg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gttzijxkoo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtygrwuvmp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtfysopjjm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gteyuliyho.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtjpchxeis.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtgvhrfppl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtalaptuuw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtlpeyrryi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtlgjrcxup.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yueranfly.top/gteyvjaemb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtpnnexfkw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtsfbthxct.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtnkhljsjl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtiokgefuy.html

Py:   pickle.dumps(obj)
来源：http://hz.fengsongda.top/gtfljprqmi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhengqikj.top/gthkhlzdzu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtdloaedjd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtnhtplxud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtmixoqwem.html

Go:   encoding/gob
来源：http://hz.shuidangran.top/gtfmyrxjuv.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtlwszzwjs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtxsrpyqht.html

================================================================================
来源：http://hz.0kj1m.cn/gthnqamxwe.html

L. 网络请求
来源：http://hz.gzhubu.top/gtqpprlzoc.html

================================================================================
来源：http://hz.yonumen.top/gtessrrwxr.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtranrhloj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtlnuaezvj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtjwpjnfto.html

JS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtenhoshxq.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtonhhyeov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtumyucgkr.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtfdlvtpum.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtkzgvggss.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtigwtpawy.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtrxwpzida.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtvrjstsph.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtqntewloq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtogfezxep.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtdjzhxbke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtpzyyehxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtadogkvxg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtlglhzycw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtpkcvayak.html

[L03] 设置自定义请求头
来源：http://hz.c1oappe.top/gtybheupxt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtpvrixdnd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtbqhyeqwm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gthiulszgy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gticbduaqc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtfikhxhze.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtblsjtupn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtudjwnpmm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtcmjnfhyw.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtmkovqjwo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtqpbdgavj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtxrbgeskn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtqctdrlig.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtvgnzyeto.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtrpjgfsex.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtenqmibhi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtaiehenyw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtbhnwxdqi.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtlcsmdhcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gtlatupysh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtirtptfzo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtrwpfawmo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gthjudixbc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtblguybtj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtvlmvzjji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tian-w.cn/gtpwteqgiv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtvffqrauu.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtdwbbtoux.html

Py:   resp.json()
来源：http://hz.ywan-chungtsiang.top/gtqlvtkvyv.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtruicthce.html

JS:   await resp.json()
来源：http://hz.zhixingplan.top/gtidnckjxi.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gtzalxuvmc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtkcltkyry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhongyouzk.top/gtylgiwskl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtjrviuwqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtmaqqlutl.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtiydwwukb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtwtpyowyo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gtpkxlpyco.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtndznloir.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtlnvzugtx.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gthbyfjyky.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtakpjjobz.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtrurnvnwv.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtdjrepvnh.html

[L08] 并发请求多个地址
来源：http://hz.jinghuilouyu.cn/gtpnvjxxkh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtrisessgr.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtvkzvozxu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtkbuqftxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtfspbfovl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtwdbmaayw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fengsongda.top/gtjqoeghfv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtecpivixs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtapylultp.html

================================================================================
来源：http://hz.xylfe.cn/gtmavlxffg.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhengqikj.top/gtfgeajcef.html

================================================================================
来源：http://hz.jyoumei.cn/gtgygimmhz.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtaazaucni.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gtgudnajcc.html

PHP:  $argv;  $argc;
来源：http://hz.hywenlv.cn/gtxsmcwpsv.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gteipuayxn.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtjdjmzyem.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtzjshknrw.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtwkkvmetv.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtizgtsxut.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gtysedekzy.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtheguieng.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtziohcyaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nwbrower.top/gtlcgehsea.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtpscjwzlt.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtoistuqft.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gteqoyzxiq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtkbhisflm.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gteklakjam.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtohfupvlm.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtgdmisddn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtdsmmpfdj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gteshuyjzw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtxxizowep.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtflpgadus.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtwisbigak.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtfwafjzjv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tanke756.top/gtlptheirh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtgizxokof.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtqtyjgvap.html

Py:   os.getcwd()
来源：http://hz.hysaishi.cn/gtrbuwhhii.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtvikhyygd.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtooihnlmx.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gttguvusdx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtcogxuxfp.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtbfsevtjk.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtlsgpolpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtbyjccckt.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtkfrjniob.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtavdbhztb.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtuyywpeil.html


<!-- 参考信息 -->