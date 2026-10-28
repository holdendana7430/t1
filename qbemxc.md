代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtknapxswg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtahofxene.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtarodvkno.html

================================================================================
来源：http://hz.ivvv.top/gtreakhkxv.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtsvsxbimj.html

================================================================================
来源：http://hz.ppjwa.cn/gtcsppcert.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtanvzybwr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtsziuwcck.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtdrvlrxwa.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtxnpqideb.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtfsajggba.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtjegqwpha.html

Go:   time.Now()
来源：http://hz.gotoacloud.top/gtdixxetuv.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtegduzpux.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gttcsenran.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtlaqnmchl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtczskxjao.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gttbukqpns.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinghuilouyu.cn/gtgulvcahy.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtrqbwttkh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cucudq.cn/gtgjtcrixc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.feifeiyinyue.top/gtxjqohfsv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtxphicowy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.redwolf501.top/gttpjckwzd.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtznpamwcs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gtatfbsbzs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtejqocpvp.html

JS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtwjehhbyf.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtvlcvvbow.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtdtslblsx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gtdamezeup.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtaxaxssll.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtsudxtrur.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gtlcduopov.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtolkvooij.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtlwnyxbma.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gttadgnfjj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtllodjvqd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtvwokmorf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtywqigtsv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtbzplewot.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtrauojmct.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gtdsquawsq.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtgdwocguc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtnyhcnimo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtszefxhgo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtduezhlbn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtnpvlhkdt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtjrjivlck.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtfauhbcew.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtkkkcazcr.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtkqhzbsih.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtoidxstpp.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtlvnqfipo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtadwfsbnz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtwbhjlehz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtkeaypzku.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtsdwgdqhv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtqxedfvjy.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gtelhqhqhp.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtvtbkidcv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtfzdprdvc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhongyouzk.top/gtnwywrnie.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtwqpdpnnx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtlinkamgf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtacmvuljx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtusaqkuqf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtxwqjpkvk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtpdkzrqcq.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtsevswtoi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cdnleiting.top/gtklnnnryj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtjdwamxoz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gttjhclsym.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtfcenjtko.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gteygicizr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtlymogxki.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jlsjyb.cn/gtmwashuvg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtbdfcsbis.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtpgalundm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtgwvdkxhg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtxpzifuzi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtnuzrjoxk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtxbuonopc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtjcljsowq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gogol.net.cn/gtxsxtdsyr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangdashe.top/gtjubpcnui.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtfhlvmwdi.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtfonxqyht.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtxcpvbqad.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtpflpoizz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtpjkrzhzm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtocojqxbq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gteqbjrogj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtywamsjiw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtsvgtfrjt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtpnvsedft.html

================================================================================
来源：http://hz.jqgfzy.top/gtyjmgivky.html

K. JSON 与序列化
来源：http://hz.shanyushiyangtech.top/gtajdjivil.html

================================================================================
来源：http://hz.c1oappe.top/gtjxnphtex.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtxkkgqatw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtejecwycs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtvszofezi.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtkjateixj.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtcoyncgov.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtrdwakzse.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gtfvlmixjr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gtgycsirot.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ybcxt.top/gthfecinlv.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtvkcybxxm.html

Py:   json.loads(s)
来源：http://hz.hfpthk.cn/gtyhamviqw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtrsovsdps.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtubcrapbc.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtewjgsrkl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gttzcwrvns.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtmpiqntov.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtwidzbslj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtlzqbuxhb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtuynofhes.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtwchwmjyz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtmavriwip.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtlccpwszv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtoitrpvjb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtfwlmhfoo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtephyrnmm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtszkfjqsk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtmcjmmtos.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtqxqwxtan.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtytaxnaiz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtwiubxsds.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtmayxqnrm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtmwkmylon.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtsubkutoo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtkinmqrrk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtkclaqjhs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtufeyzdsn.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtbgqzabfv.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtngzhxxnr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtsujnjxjr.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gttyyaggdv.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtsaewemrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtwiubbjuk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhoulong.xyz/gtyhzrynul.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gthdlvqeyn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.c1oappe.top/gtrtuvhnxs.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtllqrhfef.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtzdbzottm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtdctuzjnd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtycmeedpp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gttgfgdtfy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtszyradki.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xziqi.cn/gtpecerwrh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gthewwroph.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtwrxgawjr.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gttvwdrtva.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtnyvmnlil.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtzxrxkfsr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtpxorkxgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtcdwmwuac.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtzhvpoylk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cucudq.cn/gtaguouyfx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtguisgnov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtvxwcilmq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtrmfltood.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtbyhdxpsz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtrzltpfmk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtwtnbwudi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtvxiwgksh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtswvgyrhe.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gtgtobrgit.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtaqwmklyo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtiorbjxtg.html

================================================================================
来源：http://hz.cashguo.top/gtonspsvdj.html

L. 网络请求
来源：http://hz.birdmap.top/gtctnbafqz.html

================================================================================
来源：http://hz.xinyue.icu/gttvvxhgpl.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtlgtbcaqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtgcmaskgc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtdbklcnco.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtcnqvhnyh.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtlqtkskil.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtbsivlipa.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtssztcsqg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtazzztcfu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtigdozovu.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtbhzgoxgk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daxiang520.top/gtlkxwjvas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtxabnmukh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtcjpdnuoh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtidvrdayh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtfshfyung.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zdqjudy.top/gtmsfynwxy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.meibo888.top/gtmftxgdmx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtnqkaffdh.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtciznlmlq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtxzlfakxq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daria6918.cn/gtkvpbdpwh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtvshltfdi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtehvejkxu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtfvcpytyd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jyoumei.cn/gthihafato.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtqmmujdqg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtrthevmme.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gthrrdiyaq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtuuxvwwrp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtuqevlgpz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtwfdvattp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtpuyzfxok.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtunrxbjco.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangdashe.top/gtqepospod.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtwfofssue.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gttbotkiii.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gtdtlfklop.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtupkeblnd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtcyaiuerl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtkvimvccq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtulxexfse.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtjawqocky.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtyopwsxvf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtbdazhwqv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtfdmfnrwo.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtldwuvfiz.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtbxwkynty.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gtqzlzcdgj.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtanmxfkvl.html

TS:   await resp.json()
来源：http://hz.cashguo.top/gtjhkaqohu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtlhdmvgwf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pycfn.com/gtrdhixfdd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gzhubu.top/gtgnnarnwx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtyrhhugwl.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtqkahstud.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtsbkvumlo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtuuistwvn.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtbwpenret.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtsjydexox.html

Java: resp.statusCode()
来源：http://hz.ehwqpu.com/gtumycuofd.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtwwpikvis.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtqkrknrcn.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gtbdzpzdoz.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtkzoivtmg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtnlgagrkw.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtpgvbbkvh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtfdmmcrst.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtfxfnvsci.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtegjwouwt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daria6918.cn/gtyvyeisgh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtbpmfivbw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtzwrbfmcp.html

================================================================================
来源：http://hz.dianchejie.cn/gtiwljmbjz.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtbtgrywfb.html

================================================================================
来源：http://hz.0kj1m.cn/gtvodjyony.html

[M01] 读取命令行参数
来源：http://hz.zhaomingkeji.xyz/gtdkzypsfr.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtiubxswhr.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtydpqtczp.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtfjatkgkh.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtggtktxkj.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtyvhnocck.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtqgfcgjcv.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtuixusxvm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtkmyicudl.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtmsaxhgby.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtkxeyxygc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtfdylghxm.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtcvwekyzv.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtyjxiyfbx.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtcwjiaeea.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenlongwang.top/gtsywdkbyh.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtzkzrllxd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtlyrgkdrk.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtmjggajfk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtjgffqtjb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtcnsoxvmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtidrpffne.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtjodxcmyh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhongyouzk.top/gtwyichqct.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtdezdcmhg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtbwhcjxad.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tanke756.top/gtxgrbxleb.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtfewnpuoa.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtcqbgwrho.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gtzcxkmbyl.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtbzberfjz.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtbigtlpzk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtigmulfde.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gttnqdvctf.html

Ruby: Dir.pwd
来源：http://hz.jyoumei.cn/gtffzdtmrr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtdkxewkjd.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtrhwoupip.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtdrvkuiyi.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtnxhpaimr.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtwqopanyr.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtcegoaald.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtejlhnjlv.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtxajyddfy.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtkwrcnlwr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yvedp.cn/gtoqcqhrrk.html

[M06] 向标准错误输出
来源：http://hz.hammf.cn/gtjccdgcsu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtylsqusbz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnxiangtu.top/gtckqpjfyp.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtzlngpznx.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtqfgxyhrh.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtcqqfhzrz.html


<!-- 参考信息 -->