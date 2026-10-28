代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtunsjvnkg.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtxylqjlwj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xinyue.icu/gthebyowoo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtrcosmezg.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtsrtbdrfb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtuigsxuwt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shangyingyoupin.top/gtutggxdwb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gthkymftam.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtaqbcgemm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtpsiisrpj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtemomsehr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtrvbsgpml.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtiixheqjz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtptgbsesi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtuqtosxgs.html

================================================================================
来源：http://hz.mhx1999.top/gthnshyapk.html

J. 日期与时间
来源：http://hz.sxryk.cn/gtfflwsbjj.html

================================================================================
来源：http://hz.c1oappe.top/gtfnvvunrb.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtkxtbhevb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gthjcgzzuf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtladpemnm.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtyeqakkos.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtgdnjacvs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtulnthmig.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtupjzqweu.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtmnexwaiy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtcvhhjjlt.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gtileovwkq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtfuevzopx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtyjtnsrrr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtxsoemtad.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtebtapenw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnqzz.top/gtndeiqaio.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtihbrxpgf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtbwassicx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhoulong.xyz/gtkbixlxib.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtssmdpqln.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtefeqicgz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtzmoucrqv.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtbgwwcnun.html

TS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtmlxlakoc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gttvhmvqin.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gtqxnhygwl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtbysnldyw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtzixmvxfq.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtbttvjizq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gtfhslwzah.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtrzbzdexp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtgylzljbi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtiptsllvm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtwmgzlbhw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fzhhl.top/gtpgoivqqk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtqenhmhfx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtvkjvwecb.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtgcpxbnmz.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtnmgnjqfm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtipeunxyv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtgihpaufz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gthxmjrtvt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtevngqzxz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtsggvdmuu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtczyqnkda.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhengqikj.top/gtbhdzoisk.html

[J06] 计算两时间之差
来源：http://hz.xingfuxueyuan.xyz/gtbrodfpsm.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtgxpmjbft.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtqfxqrolt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtbmeczigw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.kuanghao11.cn/gtbxrwmiyt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtqavpmarw.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtxeslugmt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtcletrnin.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtdqyxcdmm.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtctckhpgj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtdauohvtu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtnyfjfeag.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtqfaxjebw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gteloklhoz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtifalxyys.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtehzvxapn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtncuaeqwj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtrrjrjhuh.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtcmtrwqfw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtmcamroka.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtnwaginbe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtbsksfksj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtzbtouvdn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtvjfdgtbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtlyqirjsg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtcewdnrno.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gteqzblany.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtlgstyroc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gotoacloud.top/gtrsfssrqm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fengsongda.top/gtctbovzrr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtiidoshob.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtohbwlwdt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtzcozhyqa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtzjezvfmc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtdiqfeuax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtdlufizuz.html

[J10] 取今天 / 本月第一天
来源：http://hz.daria6918.cn/gtgdzaqevk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtetqueugn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtypaculdv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gttqxqhumt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtxctkdoly.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtovardies.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtwltrmjob.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtzddcrmks.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtjlummhfq.html

================================================================================
来源：http://hz.jiagoushi.top/gtmbjjspaz.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtoiofsuaj.html

================================================================================
来源：http://hz.zhixingplan.top/gtbcpvfunw.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtrnoaplzt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtksppestn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtmewgqghs.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtzfxjcknq.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtdzgvkfhw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guowangkeji.top/gtsgdhsdeo.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtjdflzaji.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtalpqwhki.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtzwmmjjvh.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtfoxnhwsy.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtfkutyknv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtenwcaudc.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gthyfomgre.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gthmygdbsb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtptnieoyc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtghbonebk.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtvmcelufq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jiagoushi.top/gtthkroyec.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gotoacloud.top/gtwslmhhkq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtczsyzdzv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gthwhwioec.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtbmyyahdn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtgdkpwwmi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gtdjonrhza.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtwdmfhise.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.mhx1999.top/gtgnlzkddx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtihpdtodz.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gthwlulymh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gtvnpjlfsh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenzaomai.com/gtbdtuhfsq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtmliblzdn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtzjinjovx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtrgcnqnoe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtkngodddk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtauceutgl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cdnleiting.top/gtvezojskr.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtyskjuonv.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtznrlhfxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtoiotzfnx.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtctysqqkp.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtcmyrdkkh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtrbnuyijm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtcwxcnxmy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtulqebcew.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtqyvyqtkv.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gtsezpxdkd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtbdwaxdpo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtkvvzcdys.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtdagemrmq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtdwbzdtqf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtcieijlry.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtiaxhpcrg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtdtrhznzs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtuhlueyyz.html

[K07] 进制转换
来源：http://hz.fengsongda.top/gtczvltrtc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gthxqrormr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtcsprgrvt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtdmyrdeoy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtrjpgfueo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtwwsimdtf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gthhilhiso.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gtsfektapl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.svipenyu.cn/gtooiiowpa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinghuilouyu.cn/gtsxrbupwy.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtjjdzxsni.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtdqzdgfye.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtfzmkneem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gttepurguv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gtqrbrjvya.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtboqnidis.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhoulong.xyz/gtpeaumvfx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtwhjdkrez.html

================================================================================
来源：http://hz.guannengcc.top/gtuxmmyxbw.html

L. 网络请求
来源：http://hz.52xcode.cn/gtweirlrig.html

================================================================================
来源：http://hz.316326.xyz/gtonxkiwwr.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtisuhtyyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtzdjxbcyg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtrhflyqqc.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtxvqkaexj.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtiixjfoyf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtftuzqnpo.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtlsixcoxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtocnuotef.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtfflxdlny.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtzmtutpdy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtyqhftedp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtzhhljmdf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtnvupzmzh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtbajwjstg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtdwghorgh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gttkdgonej.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gtvrmloypp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gttxtljfpu.html

[L03] 设置自定义请求头
来源：http://hz.zhixingplan.top/gtyochypqd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtwqbsrxwy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ybcxt.top/gtagxxlkgc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtgueignzj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtehxqxirs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtbygmkbvl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtxbiczxsb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gttkhimvlm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtasuaytru.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtmackeysg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtcvalllvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gthwvjbchj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtrdnxoaxd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtdoadcryu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtsaeccgox.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtbgwwegvg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxinkj.top/gtlkbzwpxz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gttifzdjub.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtkphbuuqn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtlrcsvgtj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenjidiqi.icu/gthchfymps.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtspokwrfd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtlawedmkq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigfzy.top/gteslbjgkv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gttfavnzqk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtaqumljfa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtmocmigae.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtlvgexsfo.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtoveedpzp.html

PHP:  json_decode($body, true);
来源：http://hz.bjfxy.top/gtihhgslcd.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtepmloghy.html

TS:   await resp.json()
来源：http://hz.xylfe.cn/gtwfyvahhn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gttujxjput.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daria6918.cn/gtgbamdxsy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtwdvgnrlz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yanxiufei.cn/gttjifdpiq.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtiouccfgo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangdashe.top/gtndzteczt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtfunzhjrb.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtzuazrjbd.html

TS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtebiohoed.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtbwalrrik.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gteovcjbsc.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtphihqbyv.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtacspygim.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtqficrcko.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtflfdnvqc.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtclkuqwzt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtrtouzftw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtsoohkpck.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.birdmap.top/gtipselskb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangdashe.top/gtiwqahtpo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtlzknpcpo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gthjxetnqf.html

================================================================================
来源：http://hz.bjfxy.top/gtpjkwlojq.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtoxwgrquf.html

================================================================================
来源：http://hz.iojbl.cn/gtxegxlteo.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtmdjrjuez.html

Py:   sys.argv[1:]
来源：http://hz.yj20258.top/gtowpnaupq.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtiddjyutx.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtjsudlwcj.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtnyqmatli.html

Java: args 数组（main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtucweqycs.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtxwumrzpx.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gthxusvvsw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigufen.top/gtsvtsfffc.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gttmotjdjg.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtcfqytdmm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtmeqwvbxj.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtqjaiklop.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtoemhzqsn.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtvixzbxts.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangtech.top/gtrcajodbm.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtqmpeyrlr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtokfvaaum.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gtbzdkzazw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtbvaceqzl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ivvv.top/gtrzocyudi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtrjnzfqeb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtxscbtnfi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtoapvexqb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtngvgbeda.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pycfn.com/gtyrxdsstj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtpomasdgi.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtmhdhvjdh.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtzkgpdqqx.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gttnkatxde.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gtjachftqe.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtfqjjyaqt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cdnleiting.top/gtoxnmefxo.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtsgnizptr.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtojzgamve.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxinkj.top/gtcngpffnr.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtbjvmdqoh.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtsogbvcmj.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtihxdohrr.html


<!-- 参考信息 -->