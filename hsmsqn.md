代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gthpwfqpoj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtjnpkqddt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangkeji.top/gtefyzzvyh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shuidangran.top/gtibcfbmel.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.316326.xyz/gtsiohykfn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtmefppvgl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtuxgjuxpo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtatheokkj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guannengcc.top/gtnejoausy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtwpvoygla.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuxming.cn/gtfbqjvrbf.html

================================================================================
来源：http://hz.guannengcc.top/gtypvzqgva.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtsvzdxxoh.html

================================================================================
来源：http://hz.snrcjt.cn/gtfchzlkwr.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gtpokffubv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtacibhrnc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtcsmdbsag.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtblenwdhw.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gttdghlxly.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtgceuvifl.html

Go:   time.Now()
来源：http://hz.9152youxi.cn/gtzrcuhmxu.html

Ruby: Time.now
来源：http://hz.andypj.xyz/gtthviofgo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtwvcdqiof.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtkerywmdc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtluffvzdr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtslpwitfk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtrsnsbkxd.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtfzjcknwf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtmjiqwiry.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gtcrucwdfv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtotadmoez.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtyuwzxnoz.html

[J03] 字符串解析为日期
来源：http://hz.c1oappe.top/gtmgyyvtyq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtzboqctci.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtuxkcdefb.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtjnomhfpr.html

TS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtlfrpkdai.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtalypngnc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtxmtbfzyc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtqlhpanxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.vqdsnc.cn/gtazekevvt.html

[J04] 时间戳与日期互转
来源：http://hz.9152youxi.cn/gtvaauwjbf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtquchkrpr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtfbcvavun.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhixingplan.top/gtdgstnwqg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtdbrlolkb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtlgsdvokh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtegksslvt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtcrclpjdi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtyesumlbp.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gtwoaxeqbh.html

Py:   now + timedelta(days=7)
来源：http://hz.chenjidiqi.icu/gtfpcqqszz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtsbmftmhr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gteqnfnflv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtcpdbvncy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.snrcjt.cn/gttschnhne.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtsljymmda.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtywrphymz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtsxwvxpim.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtefanbgfv.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtonpsrhty.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtrkoagazf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtxiijtxvj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gtmtfrfkjy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtlzofzget.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtnmhooubo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtasarjqsh.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gthzgojkvo.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtvdkpgonr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtsofccjfq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtoonwetgi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtzsihblwy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtdtgwjnym.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtuzybijfi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtsyuvyndu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtqacoofvj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtoaohozip.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtxfufcoon.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtxtnlrrgd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtmemkdqmn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtndiqmvhm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtjtmlieyf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtdodavlro.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.vqdsnc.cn/gtprozvqyc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gteeinjwyz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtirplmdlo.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtoclbolhr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtjlzkonju.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ywan-chungtsiang.top/gtvyvuxdgv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtyfdffjzk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtvddujtrj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gthctsaqcg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtapcbvnpa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydzc1.top/gtzkbzlsqu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtbvqiqpcx.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtbofxqdgj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtfidrsmcn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtuyqtdxyh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtxhwxkkyl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtowmhlyqt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtjxcvpgvg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtlxciygje.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtptagecnz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gthvyuntmt.html

================================================================================
来源：http://hz.meibo888.top/gtykyjiooh.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtopasbodu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgauzikud.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtwtdiugwq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtsymmwgvn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtsxftjwua.html

JS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtctdiqsaa.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtnjkenuwm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtrrsyhjtu.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtkpqhpokk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtupfibozo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtwsxwktsw.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtgqtlttne.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtfavyzrfe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtcfyitkht.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtihjktuli.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtlmrtuecl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtmshdtxtx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtldnztkeu.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtsrdnmjjh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtcdalfueb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtnaorbhqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtwmwmbwes.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtzdwpfnax.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtebkrsptx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtjjbimqrt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtatrvzumj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtsmuuqifd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jiagoushi.top/gtgyxzgqle.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtzmvddpvp.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtqdrukkyu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtumafbxux.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daria6918.cn/gtulbcwdwy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtrwbudtls.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gthahjfmtf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtremrwquc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gteynmyrit.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtpybksdie.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gthmfqownb.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gtsuxrncly.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtialbkyyq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cdnleiting.top/gtvrlkagrj.html

JS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtotosozpg.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtsgthidpe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gthuqsvvzw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtgynwckfh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gthbnxcadj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gtnryfosss.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtvrqvnanu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtzkppwrwq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tian-w.cn/gtjkqieeog.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtwyknfljw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtfnoevnkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtzmbdlynm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtoahsvxzv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xylfe.cn/gtwzlulwqo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtiujyummv.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtivswhlas.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtuegzftou.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtjgmosexi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtnewhtvaj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtsditomla.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtxpbajnnk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shangyingyoupin.top/gtsbkzuymj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtiqbckaso.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cucudq.cn/gtetnogyar.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hysaishi.cn/gtocnuuhfh.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtwjombuul.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtmcimwidz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtmualtvzq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtgwfpttdd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtomfbhpcp.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtofsdvomo.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtkafklbdq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtoezzlaar.html

================================================================================
来源：http://hz.mhx1999.top/gtfuoxfdxf.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtmgfyyhwy.html

================================================================================
来源：http://hz.cucudq.cn/gtzyzktona.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtjacdljum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtkswysozc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtahxlrdmr.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtubzwhvpy.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtnvusvrwd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.smart0.xyz/gtogyvdvsp.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtvzikkbrz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gzhubu.top/gtmfwqghzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtnibruajz.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gttuhhxxio.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtzvlzawqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtcemamaev.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtstkqtzwn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtgadxhsdz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.vqdsnc.cn/gttxnqizus.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtwoejeyqu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtrczqojwu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuanzhike.top/gtsgyzteya.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtjshrwnsk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258.top/gtmeutnyel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dianchejie.cn/gtjyxlvmfm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtqndzjmna.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtqcqqjhqd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gthnlwhsxh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtdmjqwkuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gaohongyu789.top/gtgqbomhiy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtwrwkdata.html

[L04] 设置超时
来源：http://hz.zycfv.cn/gtrgjhvubz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtkghnvqqv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtufsoaxlv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtconfszwg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtxhdykdlk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtovxmxivo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtbsufcopp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gttwmnsxeq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtjxomajec.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtzuzchcai.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtqqhfwxfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtnkroesml.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtgsqkdwwg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtqdpmcxrc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtcyfjttmt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gticyfatzv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtrhpumdwh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtzercaxzu.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangkeji.top/gtmzqpqpnr.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtqaapewpl.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gttnoqgtoo.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtcduvqguh.html

TS:   await resp.json()
来源：http://hz.shzxlz.cn/gtuwsqcikt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtotbdmwrv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtkptqcgya.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gttnexdlml.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj202588.top/gttvjugmyn.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtlyskjfks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtywfwpkgq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guannengcc.top/gtenxxftxz.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtlmzxbxon.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gterbarrzr.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gttjokuctp.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtyustjywx.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtirsyehbo.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gthnkawskb.html

[L08] 并发请求多个地址
来源：http://hz.jqgfzy.top/gtebicxotr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtfaayhrxh.html

PHP:  curl_multi_init() 系列
来源：http://hz.yangfankeji.com/gtmrsrhdun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gteabhvfvt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtncavlvrz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtdpkbqlac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtkkfjlmrv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sysykeji.top/gtqtbransu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fengsongda.top/gtmpvlnshm.html

================================================================================
来源：http://hz.tanke756.top/gtzrpxcrbm.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gttkjekphb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtyailfziw.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtwohyddjn.html

Py:   sys.argv[1:]
来源：http://hz.hnxiangtu.top/gtqfbjrikx.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtztcytmck.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtspmfxxxz.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtvzkdscnx.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gtbbfqvbqy.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtawwwxnev.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtpigsmske.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtelojkfsv.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtrrtdmxrf.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtadmetvvo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gteupzznww.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtmjkhvzgz.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtuisgvnqe.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtfmfhdjco.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtjfdgpgjj.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtonvbyoro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jianghu66.top/gtyosqtukj.html

[M03] 执行外部命令
来源：http://hz.hfpthk.cn/gtzopputwl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gtcgtnhdso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtxfphlipm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtminmiink.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtctvwijdx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gtffwhwbvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtjllwpeex.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cashguo.top/gtlqawujba.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtnklfiojl.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtpvykoyra.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtmwghqdjq.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtdimfftjw.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtdyhqcqeb.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtowqdrzgt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtznmxlrcm.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtppvzkrkg.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangkeji.top/gtjdnrjcfl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtgelijpye.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtymxqeeft.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gttiwurziu.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gtfzqjfijc.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtnfhfjsme.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtllrzucqd.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gthcnexzbl.html

Go:   os.Exit(1)
来源：http://hz.jinqigufen.top/gtomocumwx.html


<!-- 参考信息 -->