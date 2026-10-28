代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtcnopjtdc.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtsmnkioti.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtryikjjad.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gtpuexcozo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtvclgviek.html

TS:   /error/gim
来源：http://hz.jlsjyb.cn/gtoaoshpqb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtkaxqwtpi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtvjhjsdzs.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtgwefebhf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtakubfxjp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtcsdanvft.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtiedfwhlt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtaauhazoo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtqzzhndrt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtstmexezp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtqshianbx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtxfhyhcxb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtncvneead.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtlktvibng.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnoowjpvb.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtahkioiin.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfdljilzx.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtaeldwiqs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.feifeiyinyue.top/gtxfzhzuqd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtztakmwqq.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtqsioonze.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtwdolibsf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.quarkkingdee.top/gtratbezwk.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtwmtrbzvd.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtlspyotyp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtmmirsdsj.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtgnznvljl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtodgiysau.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gttnwuvofy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtgowtanxs.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtnapzinsf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtihwxqxxf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gtatxdkfxg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtmphrgddi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gthfleycoi.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtwtnulyzk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gteipaschp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtmzesifif.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtgsvfmmge.html

TS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtrinxgkcd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtlvepxnzk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gzhubu.top/gtsiherrec.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtzplkfuog.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtalelsbkx.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtylwfqtoy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtqanegmqn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtzfozaeec.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtbkwdhwsh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guannengcc.top/gtdwloabpj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtzbmoeike.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtizigxatb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtxosdtmpg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtylqnvfrp.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtcneqvhsg.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtyfwizxkb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zycfv.cn/gtrmnfdrah.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtvstvvxau.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtipbruxss.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.birdmap.top/gterwwfciu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtohjkkchz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yongpay.top/gtpvjceraa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtltkfttwh.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtaeunbdje.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtpkkeblxb.html

PHP:  $end->diff($start)->days;
来源：http://hz.quarkkingdee.top/gtmaltrvyn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtfdybczuv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtzghaoqba.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gthaczldcn.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtalfwutah.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtessmeegv.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtwlhretlt.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtqdtafxfb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtyxuseuyu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gttzdytqei.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtiuzwnujk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtzmyjcsjx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtfimjpcnn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtngxkfogb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtvkvnenyx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtsnuykicb.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtmwqfcfkn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pengpengdd.cyou/gtvugknkbp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtxbbbyplq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtpcbwieyd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtazukvczn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hammf.cn/gtnihuoyzm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gteqsmcgym.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtwlersbzh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtvpateqen.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtswlwfpfk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtvprtsmhm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtozvpinvg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtudbhpebs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtxvkuhhcx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dashuyun.cn/gtliufbeej.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtbceryzui.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydzc1.top/gtqdtppapx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtsrkcgreu.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtytyxxnuh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtplwlcntn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gthpekuglf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtctxkucrd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtiiaitmwv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtbostjftj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnqzz.top/gttfnpsxzs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.birdmap.top/gtwkrdybah.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gttluqzkgt.html

================================================================================
来源：http://hz.havefunace.top/gtabvytkiv.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gtkmitswrt.html

================================================================================
来源：http://hz.jianghu66.top/gtlhndaneb.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtokjshuvb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.bjfxy.top/gteozvcixo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtojlrqlhn.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtxggbvkcb.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtrfhbmvzd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtoeimmwib.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtvukzivrl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtcdktguzn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtxtbevgoa.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtiojqyqsy.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtupcggejz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gtdlooibeo.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtmshtcgvt.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtgbevuuuz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtepzchahb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtqlmjqcqx.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtqwtsutxs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtaqyvwubk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtbnmsljdn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtrocjlrza.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtvjsabges.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtkqszvykr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtcvqiqyiz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtldchlbqq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtrkeywfmn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtnbaxfcnu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtturonadq.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtchcthydu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtyhamxftv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtiquxnfav.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtgjhjwckd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtqoudhbqy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sufxvd.cn/gtqumtakol.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtpwkrszuu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jyoumei.cn/gtxiecwaml.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gthhnupnde.html

[K05] 深拷贝对象
来源：http://hz.tian-w.cn/gtmnuaugvu.html

Py:   copy.deepcopy(obj)
来源：http://hz.vqdsnc.cn/gtmchwzlmj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtrisgpcgr.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtmbvheune.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gthcdfcgjn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtmvahkjae.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtcmknsise.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gteowxryfe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gttgmztzwa.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtnwmadinc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtmgdwvatd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtgrvkyyjc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gttkufwjha.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtdkofuinq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gtrxzyznbo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gtcuehtxtt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtputinybp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.c1oappe.top/gtmzdjsvhg.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtoryqfpoj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtuhgiwmuj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtxvmaayqk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtsmcmpjxz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtkarmkjjl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtfxxdpyzh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtttcghban.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtyvwqgmpc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtqutxhduj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtqxgvjenm.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtmiriofwt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtyppznlol.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtmpgdemfu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtbnarrwoi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtnxzxodnu.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtvzycukpr.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtacgbqelk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtxeympbmv.html

================================================================================
来源：http://hz.smart0.xyz/gttkqpftne.html

L. 网络请求
来源：http://hz.hammf.cn/gtiixkbyhd.html

================================================================================
来源：http://hz.shzxlz.cn/gtvsruvads.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtiwzfztot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtbmrswamp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtsuravfeb.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtuuafwqbz.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtcctdorle.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtilkwdlfh.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtepboagxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtxchilegs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.kuanghao11.cn/gtbhsotsle.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gttjbpqamd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gthcfbzyhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gteaitmcea.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtoskzhnfu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtmslcoaii.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtoifizisr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtedwrerfm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtfvqjhdeb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtkakuygpw.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gttiunxiod.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtoiykkqno.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dianchejie.cn/gtisfthhwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtvymkeliv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtrtdvjrdh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtarhfsqpd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtdyhtglqd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtmjgwwntq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtehdcnafa.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtmoohcnfa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gttgumsaff.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtkmdkkxld.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gttcvhtrkv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtpcnwqhvj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtsabhancc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtmxkqvkdp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtgehpynwe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuxming.cn/gtrdukylon.html

[L05] 上传文件（multipart）
来源：http://hz.chenjidiqi.icu/gthgruuoia.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtmvcsizod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtyevkoird.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtegvvsjqa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtkmcbrrjd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtwxawjvuh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtjwgdibwv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtmlwzgdpv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtnequbdtj.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtlalnsvir.html

Py:   resp.json()
来源：http://hz.shzxlz.cn/gtksgyavof.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gttooqlwhc.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtmhhzdhev.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtnhdzahhk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtztvygjii.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xinyue.icu/gtueftvpim.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gtzopmhsfc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtgxadcqxw.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtgzysgnug.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtbqowriqd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xingfuxueyuan.xyz/gtlpytzvft.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtepscbyhe.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtccblxuun.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtteigoxeq.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtoxkcllow.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtsozzuyyd.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtxzuugrbh.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtapezwcun.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pengpengdd.cyou/gtxywppjya.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtvgyhbdqc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtzilcfwfb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtevxiwmzk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtmgesyhbc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuetiantiany.cn/gtcpgpfaiw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtpqehhbbd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtwdiqicuu.html

================================================================================
来源：http://hz.daxiang520.top/gtpgfwzzuk.html

M. 命令行 / 进程 / 环境
来源：http://hz.tianlin.xyz/gtwypxphjx.html

================================================================================
来源：http://hz.yonumen.top/gtpzjpdkbc.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gttbjfmvnf.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtuichtmhz.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtftoqaiyl.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtuovgbpep.html

TS:   process.argv.slice(2)
来源：http://hz.sweek.top/gthzafbkxx.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtymalyssf.html

Go:   os.Args[1:]
来源：http://hz.havefunace.top/gthcymviwj.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtwmtgrsih.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gthdepwktc.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtifhgyvqw.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtdkarpaer.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtfhehanhq.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gttphdhanr.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtwxlopbtq.html

Java: System.getenv("HOME")
来源：http://hz.gzhubu.top/gtmhrdnqod.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gtbytmvwgy.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtunsiluqw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jlsjyb.cn/gtovcgksxx.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtnivnlgag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtmhlxjaln.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtslcrzkxo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtjfutavki.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtzhpcnyyw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gteninyzpd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gttymlfqsc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtknwijxak.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtidezvnfx.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtlaljkyqn.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtsimqipcb.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtqorcxgcb.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtmrdukjse.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtamnivyrr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtvkbotudb.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtvhzevgww.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gtjhoattrk.html


<!-- 参考信息 -->