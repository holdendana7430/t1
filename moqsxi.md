代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtqdhfsffb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtnxabyfcr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gthgzugcrc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtstjxjlzx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gtshjbypnv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtcetcxuvo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtalyeruhd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtnuemvatp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtjnqrxpbc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtqolsofao.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtxgghkevj.html

================================================================================
来源：http://hz.nwbrower.top/gtdlifxazy.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gterxotehw.html

================================================================================
来源：http://hz.gzhubu.top/gtlqvsbtwt.html

[J01] 获取当前时间
来源：http://hz.fengsongda.top/gtdddntoos.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtyhkvqiyy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtdpudsdtm.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtodgnjqxt.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtmyeftffa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtholktfua.html

Go:   time.Now()
来源：http://hz.zhixingplan.top/gtfacjdtys.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtqqbfqofi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gtuonhjvbn.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtyqxrefge.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtwmmnhjop.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtdujllold.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtorrqitvr.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtattikpex.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtgwgrtmep.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtoxoqygnz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtsmgcekqg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtnfmzyzft.html

[J03] 字符串解析为日期
来源：http://hz.daxiang520.top/gtpvltidws.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtqpxxiuom.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtajcfijyb.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtznecszkp.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtyqkhmzck.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtzmvqvnyz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtfgqhcpwr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtninrdtpv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangshuangyany.cn/gtfetzpgnz.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtceapowqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtaanbvfap.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gtszyqiudp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cashguo.top/gttyhaiqfq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gtejgupbfy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtnxwvlrtf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gaohongyu789.top/gtbmbtwbrd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guowangkeji.top/gtxpdtwkpy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtbthwsnrz.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtqkiqgvro.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gteahaqtnp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtjmrxeyzf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtmkcwtmrc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtinsvmvyx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtmkdmafvz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtfkvqwjqz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtevwidmhq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ivvv.top/gtwxwauqkv.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtljntzgnn.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtodhvtpex.html

PHP:  $end->diff($start)->days;
来源：http://hz.dashuyun.cn/gtlqrrqsyl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtqzomtsis.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtptndegvu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtmtjeswpk.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gttakjawzv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtowopryuk.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtmjyfejcw.html

[J07] 比较两个日期
来源：http://hz.zhiwuduotai.top/gteaxugwov.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtdfhnzsvv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtqlozjaho.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtttixqwnv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtolmtpuqt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtgategdei.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtfykwppch.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtnoebxfiv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtlmwdzqaw.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gttfbhsfwl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtpyxuxisb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtyihjkjgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtjksktfea.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtbdiztgjr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gtyqnycmkh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtasufmsqo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gtmcsmqezg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtxzizlqnf.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtwpyfrlnj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtmbztbldy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtivrqnxpd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtdlxqwzwc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gthqvictpd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtmehxnlbq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtqgaxljag.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtkeqlimbm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtqglqvjhn.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtkpgycxlf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtdzzqqvvj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hongshengwenyu.top/gtivjmruqx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtojgwqsln.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtozrpvlwt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gthupbtqgx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtnahvuqhs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtuqxhirjx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtctmergpy.html

================================================================================
来源：http://hz.hammf.cn/gtsclsvkgf.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtgkpifvgn.html

================================================================================
来源：http://hz.chenlongwang.top/gtowqrtoud.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtgwcwgary.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtqdyxjxdc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtbqbwjair.html

JS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtmnwdmler.html

TS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtigbewdfu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtkbofsmmi.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtjatikfgq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gttcubgbmn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtyzvdszqh.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gtubnnjjod.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtaojfnyeq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtplsfhdpl.html

JS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtwismzhph.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtiutqcsmd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gtgbvoznfm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtiaglcrvk.html

Ruby: JSON.parse(s)
来源：http://hz.smart0.xyz/gtkxqlwsgp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.svipenyu.cn/gtzidjescz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtvkrdfeuq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtjwbslpul.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtsykcjkug.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtwlndudqo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtikcaygam.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtutnplrsl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gtrruocshv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtqmneduaz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtezdqzvjp.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gteiqsqtkc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtqkvwseze.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtavsjkjmr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtutlzqexw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtkcardoiw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtvqtetykt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtmezoavkg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtwgbfhvcc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenzaomai.com/gtgdxgmozj.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gttmbxkfkw.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtulujmyha.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ybcxt.top/gtwzsnrrio.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtshhnbydt.html

TS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtcqwqggrq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtqrwpxtbf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtzgcgnixt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.kuanghao11.cn/gtdvsazwpo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gttmsalyfu.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gttnfviaho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtrgutiboi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtmldrrudt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtxrrimbsv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtsxmloczv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gtipdxhsne.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtvotmgyky.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtqxdphaby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtlzkjnizu.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtosxwqwju.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtebtzmkjs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtisqnptpv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gthmcelzec.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtgypyjbdo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gturlbkyyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtdfowxipq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtojseqppj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtmxraspqt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtwajassoq.html

Py:   pickle.dumps(obj)
来源：http://hz.gzhubu.top/gtlxgkiqgt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtvyksafsy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtbhmzpbvx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gttixtzfnq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gtopzxezzo.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtotsojrym.html

Ruby: Marshal.dump(obj)
来源：http://hz.jianghu66.top/gttxdzdnom.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtgtydbadi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyqbxymkj.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtvaoukrlb.html

================================================================================
来源：http://hz.mhx1999.top/gtgwyqnxib.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gttwpgelim.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shuidangran.top/gtpvqhkbpw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.quarkkingdee.top/gtouefvevk.html

JS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtjuaotdtx.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtsafgnzyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gtzqluqzav.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtzagzmznj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtugjvkwmm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtiyfcbtby.html

[L02] 发送 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtisyqjuln.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangtech.top/gtqvcgntcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtvdoyxdfv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtnxncgumg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtvfoxxklj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtxmbzscxy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtzvtpckuw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gaohongyu789.top/gtkavzrlna.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhengqikj.top/gtmbeyxswd.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gttycphyjn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtgizfmkkd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtbdrmkdzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtuquuqmxo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtheagtxzm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtggvviynm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.iojbl.cn/gtlrgourlj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtazbbunxg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gttjtemekr.html

[L04] 设置超时
来源：http://hz.kuanghao11.cn/gtkklqbazn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhengqikj.top/gtxvlqgbyd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtjkoxqoaa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtnggtfmqn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtkocmgugv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gtkyjmcgat.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtristsari.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtzqodqxzu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtwmsfqelx.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtmxvmqksu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sxryk.cn/gtiogilbde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenlongwang.top/gtdpfvwpri.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtdsiuihxz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtphcgvjei.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtvnxjiovr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtmprmopok.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtyqkmtgyc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtzjpocjzc.html

[L06] 解析响应为 JSON
来源：http://hz.zhengqikj.top/gtomzphhjr.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtdhipdevp.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtjqpyvuvb.html

JS:   await resp.json()
来源：http://hz.shuidangran.top/gtjzellrod.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gttaqseybk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtorixyiuo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xinyue.icu/gtncmhgrlu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gteuvnvyni.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtuoqwsvvi.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtllqcbjja.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtqtpchjzd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtukyvofar.html

JS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtlygparrd.html

TS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtrydukeuc.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gtysxzwmua.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtlrutlyok.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtbzvkxctp.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gtffhweovz.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtsvtdfcko.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.9152youxi.cn/gtrlwglnmq.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtujffysqi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtmrpnpnpl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtcnpvpjey.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gtsltzshvd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtfcvqrbuw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtaxqpizvg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gtialawupe.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgdkvldvb.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtdepppygx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgiwhrraq.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtirqyruhz.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gtsubjaqlh.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtlbedtfdq.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtdxxfivyi.html

TS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtjfgmnbxg.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gttariwrph.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gttjanioux.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtqiwwrhzw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtmjkcffzt.html

[M02] 读取环境变量
来源：http://hz.iojbl.cn/gtmfnsacfd.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtuxkgowzs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gtidgbtorb.html

JS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtmcfzwkxa.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtytzffaou.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gthkxmtysn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shzxlz.cn/gtoirxixjh.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtgtwynmdz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tanke756.top/gtorpldtie.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtgdmkgmzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtngfexqeq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sxryk.cn/gtvhkwfftp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtywnpddmj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtuvbbuglp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtkrsugrrx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gtjctefcgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gtvabkmojz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtgbzfxlej.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtdcvniort.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtkfqvjobn.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtdjvwfsyb.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtlitsxhis.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtshwpnusx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gotoacloud.top/gtmeharxwf.html

Go:   os.Getwd()
来源：http://hz.jqgufenzy.top/gtuglkgdto.html

Ruby: Dir.pwd
来源：http://hz.gzhubu.top/gtcyvmwysb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gttsjnqexy.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtsacsrgir.html

Py:   sys.exit(1)
来源：http://hz.yj20258.top/gtuklexgtt.html

PHP:  exit(1);
来源：http://hz.feifeiyinyue.top/gtdfqtlces.html

JS:   process.exit(1)
来源：http://hz.hnqzz.top/gtknslfopy.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtmvzbxvts.html

Java: System.exit(1)
来源：http://hz.bjfxy.top/gtmmyzqqvr.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtmkkwdcze.html


<!-- 参考信息 -->