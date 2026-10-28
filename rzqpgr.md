代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtrioqnetz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtfpclshdh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.smart0.xyz/gtxzhzymvg.html

================================================================================
来源：http://hz.zdqjudy.top/gtvrgjqsxf.html

J. 日期与时间
来源：http://hz.pycfn.com/gtzyahsvts.html

================================================================================
来源：http://hz.yvedp.cn/gtqhoccvak.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtprqjeuex.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtmekouggo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gticzgsxtj.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gthaogtyee.html

TS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtyyorkkav.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.52xcode.cn/gtwpgixhtz.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtmleevsbk.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtfhmpibqy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtkrgijors.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtpjfnxjqu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtmiuoespz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtfgswxelm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtsuonfmyr.html

TS:   d.toISOString()
来源：http://hz.wangdashe.top/gtqdewpeef.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.feifeiyinyue.top/gthwemnwah.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtcebbheva.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtcfzcoevk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtcdferpyy.html

[J03] 字符串解析为日期
来源：http://hz.zdqjudy.top/gtsiycqvdc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtatnrhbug.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtnhovmnyn.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtkfzvhute.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtlrbxetmz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.316326.xyz/gtmqfhhjwq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gthdvkcegx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtpyehofuk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhengqikj.top/gtimvqkisi.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtrxdsbzuy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtgonggnic.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtjhfpzclx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtytakekjp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtzgevkosd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtxgehqzbh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtutsybhaj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtornkvfvb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xinyue.icu/gtqtbatgxr.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtsdcfisnw.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtwbgywtev.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtaxmupkdy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gthubwuzhj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtiwreoort.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtecwtokfh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtmeitmgmy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daxiang520.top/gtedhwbbkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtvwhomlbk.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gthsuzvfsg.html

Py:   (end - start).total_seconds()
来源：http://hz.chenzaomai.com/gtudovqavg.html

PHP:  $end->diff($start)->days;
来源：http://hz.quarkkingdee.top/gtgifqbrch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtyciurnha.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuxming.cn/gtpdjhovqo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtwqrwilrr.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtuavlqypj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtmaerprom.html

C#:   (end - start).TotalSeconds
来源：http://hz.0kj1m.cn/gtubhpfcsq.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtiyritevq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtalbxtyut.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtehgluaxl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtifwsuoub.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtjtjuiqde.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtnvxnxcug.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.vqdsnc.cn/gtmqftrrql.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtiztxzbhs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtkzrucajg.html

[J08] 提取年月日与星期
来源：http://hz.jiagoushi.top/gtbqtkmroj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gthszytbip.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtuuaxigfm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtzzkpoznv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtsoyepgvb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtzfwuvjrr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtpskkrktz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtkowqvrsx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yonumen.top/gttmvsoqie.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtthoxukjy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtotvvrqep.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gtdcgxhsak.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtitmarihh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtqphhxwxn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtzvdjjmfo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtaivvwcjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtvxvfmcpd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtspwclztr.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtvxhaqgon.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhijiandao.cn/gtdkqmiuuk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ywan-chungtsiang.top/gtplbbjqzk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gtphztjxgy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtogxvzrlb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtpehjaalk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtwriilvwj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtptyjmrpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtoxgyptfx.html

================================================================================
来源：http://hz.0kj1m.cn/gtapvaljxt.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtvgmgamet.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtecsfovxa.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtrrswozkb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtlqulecyn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtibwaqrgw.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtatzvdyro.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtwcvoyqpj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtdenxcjmc.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtyzjqnfwf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtkxnkbfcs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenjidiqi.icu/gtneaqalwy.html

[K02] JSON 字符串转对象
来源：http://hz.hfpthk.cn/gtjdbcakyp.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtlheelzfd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtkjjaqoyv.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtcwulesqe.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gttsfjtuee.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtvlbreqyb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtkklpojhv.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtsgehjuvw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.meibo888.top/gtqidfifpz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtezfuzadi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtkrbwzatg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtpwjzxkqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtxnijzebd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtbwjoflik.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtqzyiwlsw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtlscgqpmd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtrsjwbgto.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtsqpjncsj.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gtsdxvmvse.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtinvbxoea.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gtehigbmlg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtwhxekbct.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtacjalqqu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtcjxwzgfu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtrnhfneoz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtwqotdtgl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtpriplwul.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gtmsesrddk.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtbmamzdbv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtjifadzaa.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtmdrjqqlq.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtbjlsyxdz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtfnfckpld.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gtrtgnoykt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtirsobofb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gtaszdgfkb.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtrijavyrv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtlqfdmhdx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtaignrgkq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtstluqcxe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtnczndyxg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtxyveamkm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtozpkffpx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xinyue.icu/gtvqntysfz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtsbalhoqy.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtumzckibh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gthbywhtth.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtewdrqovt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gttqqztqba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtfamlsqze.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gteitopmdj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gtzowahgbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtexhrkkfn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtmpigmchq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtlrzmfuhy.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtbfukwebs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtueilmiuo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gticucjxbf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtbpjmldng.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gtjdfbcqlw.html

Go:   encoding/gob
来源：http://hz.jinqigufen.top/gtoapxsjaz.html

Ruby: Marshal.dump(obj)
来源：http://hz.cashguo.top/gttqnngrno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtaebtuatz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtporlmgod.html

L. 网络请求
来源：http://hz.xziqi.cn/gtasbgbwdn.html

================================================================================
来源：http://hz.guowangkeji.top/gtiwxqyjlr.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtwjviyhre.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtxrqnjvlp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.andypj.xyz/gtrkpkqugd.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtkwjalwmf.html

TS:   await fetch(url)
来源：http://hz.zycfv.cn/gtxkxcijob.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gttoehonzh.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtvjdegjge.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtkyhokurp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtgqhmgokw.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtchuautow.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtuagycsmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtgoymrbsr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtuyzahoba.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gttffpqdum.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtkuhtvpsg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtswzznoan.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtslyygegy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtjeiyipbi.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtrissiinb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtekbpluax.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtpekmimny.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtbeveqeui.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtbuvytedf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtgmdkggwk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtphthecpn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtitrdvfyy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtkvmvanhf.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtlxjhpvyy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtkeehqcsq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtmlojgclb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtpgyefznn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtegcqrpjv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtvowjgefa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenlongwang.top/gtzwxqcreu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.andypj.xyz/gtxwpvpjnh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtkubgxkrl.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtjtkrltjo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gttivzscpm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gttulbtkgt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gttnywgpvr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtpafmxzbf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtxsohftja.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gttpzuzdsb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gthdsooyvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gthocokjcs.html

[L06] 解析响应为 JSON
来源：http://hz.aizwys.cn/gtmaxchfwa.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gtvhzejxog.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtytbcabub.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gthwaoptid.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtgjvapnns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gtzqpdtxgs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtmlwbokwy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtcphkcsgi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtxyrpgbxi.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtobwtwokl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtiqsmrhmu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtiuhrfppp.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtcqvxjekm.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtkvmqztiu.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtrdwipmel.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtlfolfxji.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gtwxfcijmc.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtiyrijjsa.html

[L08] 并发请求多个地址
来源：http://hz.yj202588.top/gtmsbvgicl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtadcccvos.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtkmgupfbq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtzuhwkbsk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gthnsfiuzx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtfjkurzog.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtthmplaex.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtzhuhtplh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxinkj.top/gttfhkvtxa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjanbnxgv.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtnpyvhnft.html

================================================================================
来源：http://hz.tanke756.top/gtpazikrzu.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtqoduanrg.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtlllazubi.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtbnxgmfkv.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtsujtdkgb.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtfbmqhopq.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtejirrefr.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtttxaruvk.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtuaohykoy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtfyhjxcke.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gteaudkusr.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtixcmdgix.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtztumzncu.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtivclwadv.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtnsbhxyns.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtfpkbyhhe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtahcegeph.html

Ruby: ENV["HOME"]
来源：http://hz.zdqjudy.top/gtodkykcof.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtxzdgpbkb.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtujobfytr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtcgqlabug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtjcpsydgb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtzqnjafyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtuwodzzbd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtrppljvrr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtyxpsocrs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtghcvghpj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtbqfkgckk.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gtxjaeegrw.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtogmjgvmd.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtapkujdia.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtkqhrmdqj.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gtwoyhupkq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gteecfgssn.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtkcevnkap.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtoeyrihsp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtmfuvlnth.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtrqkiqyye.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtjyowlqlm.html

PHP:  exit(1);
来源：http://hz.birdmap.top/gtwplqpmex.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gtbyczedup.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gticaqowah.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtmcgmdeop.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtbylgemro.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtxixquqct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtmqkdcris.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtzdosmomg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtnfpkxwzm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pengpengdd.cyou/gtmqcxchbz.html

JS:   console.error("err")
来源：http://hz.birdmap.top/gtkjsbxfpz.html

TS:   console.error("err")
来源：http://hz.sysykeji.top/gtvlenrzso.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtblkvsgix.html


<!-- 参考信息 -->