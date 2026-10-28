代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtljipjqlq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtkntszvit.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtafzqasxl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gthbimwvin.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtnvwoqfgh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtwbzzvsuk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtwyowjfbm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtujjgluzh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yangfankeji.com/gtkroggehx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtyglbhkvq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gttrlqhzjk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtcgrlrorn.html

J. 日期与时间
来源：http://hz.sweek.top/gtheozffwl.html

================================================================================
来源：http://hz.guowangkeji.top/gtlldqmtji.html

[J01] 获取当前时间
来源：http://hz.zhaomingkeji.xyz/gtpoxcjmwm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gttdvbqlxp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtcxokbdql.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtppfsavcu.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtcihrxdan.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtyhbvdtzj.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gthetddwxf.html

Ruby: Time.now
来源：http://hz.shuidangran.top/gtggwsimjn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gtzwwtfnbg.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtvuhowrhz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtctfhtdmy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtydhfrquf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtguuodfer.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtbrlvhyvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gtyvzsxnhi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtfdlrjsjt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtugazuurw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtegtbnqwk.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtoxfmbilz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtlleqcots.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtshoyebpr.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtszvbwoys.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtgrhdsjhi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtnqliyyqi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtjhrcknhr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.havefunace.top/gtopjluyhe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtmssmrajz.html

[J04] 时间戳与日期互转
来源：http://hz.yangfankeji.com/gtecmyjwdu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtmvfvquvu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gthpzxexjl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtqikfqtgm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtzftedzom.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gteqlkrcrj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtfjhlbgbr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yueranfly.top/gtckvijbhs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtheiqatxy.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gtcttfpskf.html

Py:   now + timedelta(days=7)
来源：http://hz.yueranfly.top/gthghnxlwm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydjk.org.cn/gtyylarqju.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtcoimtgkq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtvbfheoha.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtbowvdufx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtrjagcwfv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sweek.top/gtravdvmmh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtmrkshilr.html

[J06] 计算两时间之差
来源：http://hz.hnxiangtu.top/gtjdkzdwwv.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtcqsfxttk.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtlovrqgth.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtbgbrcdqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aibaodan.cn/gtaikjfnqh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtsnfksiar.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtbvqeivhv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtsjcwbvfc.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtvcbsyzcq.html

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gtadvkzzxz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gteqcqhcep.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtevrzulhf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gticppvpga.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtiqumssun.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtfdclltur.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydjk.org.cn/gtjkcisaso.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtlmnswtea.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtlbscgvpj.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtonlhadhz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gtewudrfec.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtvgjebnip.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtxptdsmvm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtsudbfahr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtclqpmzjq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtdwoamcyx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtkhmokdqz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtixungify.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gthujjzoma.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtvycliwob.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gtulzqbzoo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtwqzjpyda.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtenzqxfqc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yueranfly.top/gtntbdjklr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuanzhike.top/gtgwycymcd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtcpjrowfn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtomdhljdu.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtdtbaqmgc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtllwmgrka.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtgsyyoisc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daxiang520.top/gtmsgjyeel.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtnvwouepe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtleoobeir.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtjrqoseja.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtyeghzngh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtfaxxdcsa.html

================================================================================
来源：http://hz.pycfn.com/gtutfbvasu.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtykzmkuhm.html

================================================================================
来源：http://hz.sweek.top/gtvfjimrki.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtveihakol.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtbmxrimga.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtunltfrts.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtnzsvmlyj.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtpwkmkrqd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtpvztymux.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gtthxounvq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhijiandao.cn/gttphnrjrf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtldfhlxzj.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtlygerghh.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtceqmdolo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtwwymzboi.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtpamrofci.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtnjddiddh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jlsjyb.cn/gtxbbxahir.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtlhqlrouq.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtiodnutef.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gttmzdnhhs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtqiowwzqj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtirrgpzlc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtzccygkkz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtiarwwejw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtayhahrpb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gthjggsacs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jianghu66.top/gtnifqiiji.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtrjxkxycy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtdynbdddq.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtkloqfsrx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.haohaochexian.top/gtstywwbgh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtobtbetzo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtqohdkdku.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtcolkvuxh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtlzmgfolg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtehatadam.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtpvkgirzc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtzlewfcgq.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtavzmxuvn.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtltlslovb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtlmszmvqm.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtgcqaigli.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gttwlptxqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gthibpenvd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtovphzxeo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtrhzcnxcf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtmgalwwff.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtagvyfxob.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtuiyulcbt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtzbokzjxc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtbihpjjwl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtfpohyeja.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gtubddbyem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtvwuzkdnd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gthqyxioso.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtdfiqjsbt.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gthtwlvbuu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtyznylsgm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtbigvmwvt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtutawvpgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtnivnzezj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtchqrcmig.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtnhuhfxzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtoixnhnvu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtycxezdbu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sxryk.cn/gtvjnhrfww.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtnioldezz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtngojhvcr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtvvwnwkmj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtzkquvcui.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtulfrmuql.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtyscujxrc.html

Ruby: Marshal.dump(obj)
来源：http://hz.quarkkingdee.top/gtcfhydcpa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtrwhyusee.html

================================================================================
来源：http://hz.tianlin.xyz/gtsjdsasky.html

L. 网络请求
来源：http://hz.c1oappe.top/gtheatuqjc.html

================================================================================
来源：http://hz.ivvv.top/gtqbncaugw.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gteaiwdtzi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtxxhpocbb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ybcxt.top/gtdsjvrygi.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtaompkfxj.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtuokmkpmg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtkerbvote.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtofchrnse.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtvboqtvyy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtjeptjqzp.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtlnpcnghr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtpwhfxfmv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtzoivbdli.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtrkpcahkl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtawgqkpmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtzhdokjao.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtomcsgisd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtjzumnlrq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gtcxiuqfhg.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtzmdgutan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gteenytiyv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtkpfujekj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gttcjxwrqg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gttveottya.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtcgqbveyj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtteoxphry.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtbuvgexou.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtdxmntzjv.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtcpwenhsq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gthjyvqhwa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtigvntctt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gturnthgfs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtflwsnqlg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtzgqatadf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtydptdjer.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtjfohklqz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gtsfxmmsim.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtrpefzkrb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ehwqpu.com/gtzjuhrkim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtxrlzmsqm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtqmspnnbz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtbwpacldn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtdhwsqrto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtubgeroeh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtxgjwmfje.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gtkjvkbikt.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtulluvdkh.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtzltcbtej.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtlsutcpah.html

JS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtzxkyplkg.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gttddierxe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtulhxnabl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gthpyjwddr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydzc1.top/gtdhqfrkol.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtpogewlpe.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtrgstwpmh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtgvsomajv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtphrwgqvt.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtmggefpyn.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtolhsrqso.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtlcucmnia.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtsnuetugg.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gttaiitmfx.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gtxvnujdya.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gttmxobxws.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtvtzsyykj.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtboxzacns.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtebjedvim.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gthxunickb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtnhtvqzeg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cheryme.top/gtyjbxkwsr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtipbnvsoq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gteqklvwjz.html

================================================================================
来源：http://hz.pycfn.com/gtnparfrlp.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuxming.cn/gtomvwdean.html

================================================================================
来源：http://hz.guannengcc.top/gtkipcmbas.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtijwfraly.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtxqsvwtsb.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtxtxezrow.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtfjccazxm.html

TS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtkqhuyxzx.html

Java: args 数组（main 方法参数）
来源：http://hz.cheryme.top/gtxjdqnafa.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtzvyelhia.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtnseqfmcf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtdcmmrpfg.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtmtgfsoim.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtlkugpivk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtnefyhcum.html

JS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtfudpyzqp.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtwqhwlbos.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtcbraguxg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtdgqxrwxt.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtoqfugrln.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yanxiufei.cn/gtrvtjnutn.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtjdduyqrv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtwddiajeq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtqrziavup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gthjfsewwh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtmqpzbfkv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtdskslqei.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.mhx1999.top/gtpaquinvl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtcfywhuig.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gtccityauh.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtmiwejynm.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtacbyemkn.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtfxjvrcqv.html

JS:   process.cwd()
来源：http://hz.cucudq.cn/gtitkpilks.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtopqnfvrh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtjklutjbl.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtmqvolxaq.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gtokixoofu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yanxiufei.cn/gtcoqoqcar.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtmoklwwuo.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtbpszktmn.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtgsujsrij.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtmmkqohdl.html

TS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtozctofia.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtetyordsp.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtmlndrlcd.html


<!-- 参考信息 -->