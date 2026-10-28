代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtrabnipak.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtyoneylqf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtzxjdakdm.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtyhhsvevi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtsffivfxi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtchbhrffj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtshgiqoot.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtginzzxlp.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gttljzvxae.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gtjyodfcev.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtmgnpclnc.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtklbsxkkh.html

TS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtfdpklzue.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtuzwklhtk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shangyingyoupin.top/gtznlcycga.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sweek.top/gtcvgxlvbs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.daxiang520.top/gtdgtmxbwg.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtdivkpizb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gtkvdnjypl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtwwwffmez.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtwmeathdc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtyuemzstx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xylfe.cn/gtdwpiphtm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtlypbnmwh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangshuangyany.cn/gtrmujftjt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtpymuuxbc.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gtmdpkogyp.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gttsrikbnb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtypzdtomf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtaluybfrw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtuykbkwoz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtbqhnlxkw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtbcgbfxom.html

Ruby: Time.now + 7 * 86400
来源：http://hz.kuanghao11.cn/gtwafqcamr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtnshaggxn.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtiqoqvsjy.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtmzdbsaaa.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtydhcaamx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yueranfly.top/gtbyjmkzrg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gteeyuxhyo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtgplewkij.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtcfqnrwvn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xylfe.cn/gtuhqexkdn.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtfewotaps.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtkakijqsq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gttoelgoea.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtihxiditd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtvewdeucx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtsmheknto.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtundreuvm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtzanbsmwy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtajcwyolk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtxkiazpkt.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtrznmxzbe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtmaotslbs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhaomingkeji.xyz/gtkkpardef.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtjpvymgsn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtfmmggzaz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtpcjbniub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.smart0.xyz/gtlqmyezkd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtstzcpvrf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtqunoflov.html

[J09] 时区处理
来源：http://hz.wangdashe.top/gtwnhjkvwc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhiwuduotai.top/gtativjcri.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yonumen.top/gtqyxtoobq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtyzhxhnph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtogaqiuwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtecjvzaam.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtvqgvjlno.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yanxiufei.cn/gtcosfeorc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtycyhejtx.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtrujgrzih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xylfe.cn/gtimgkjnam.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtpzvuczcn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtemafvttu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hnxiangtu.top/gtrkjrlwnh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aizwys.cn/gtxcdggylv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtkgldaqzw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtfzzlgmqg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtlaokazmm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtompeznvk.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtwxjttjpu.html

================================================================================
来源：http://hz.ivvv.top/gtuwwfggrk.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtipqhhanr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtnbkyfned.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtbeoyjire.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtojixeldu.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtgqeoooky.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtjzeatmph.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtqsiryore.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gtrsvjyorf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtnbgrinms.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gttqwlhwbr.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtiivxohrz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gthmedzuzm.html

JS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtkqibvurr.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtkhnmvidl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gttzlhrvfq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtsbyjybus.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtpnhxoire.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj202588.top/gtrutrilvu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenlongwang.top/gtirutmucq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hammf.cn/gtgblrdlfo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtwolkxxgr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtbgikoimm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gteyrgodgy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cucudq.cn/gtdpguonmn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtcatinmiy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daxiang520.top/gtpjomlhzb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hongshengwenyu.top/gtthaoibyv.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtrytnifsb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinyuanbaomall.cn/gtpvzzjfuf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gttwwijeuw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtielafavm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtbgwhqhhi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtibmnqjcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtnwbgylji.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sysykeji.top/gtppkiegev.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtvuxnqlpl.html

[K05] 深拷贝对象
来源：http://hz.guannengcc.top/gtkgdnygoc.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtavnguaon.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtkscybopn.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtnxuutqrc.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtuxxvjdjs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtnmsjtbyk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtydagcksp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtkibzxmrg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtjboytglj.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtgektrkfv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nwbrower.top/gtajnmmxsu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtwxysemvo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtswdodvhu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtkfcwuhop.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.vqdsnc.cn/gtwhurgybk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtbeimjbpn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtvoocyflh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gttqlesrjp.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtbpzrgxam.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gthqcupeze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtaymsgqez.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtjrwjbdje.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gthmhbevhg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtgihtcauk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtudfibhlo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtaocezswa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtjccziqny.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtahmaemea.html

Py:   pickle.dumps(obj)
来源：http://hz.tanke756.top/gtzvwbvjkp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtfyxxawpx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtzyrwndlw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtdwghzzgi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtpsenrtlu.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtvjlteznv.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtluiezace.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtwjedghmt.html

================================================================================
来源：http://hz.gotoacloud.top/gtipeqkxgo.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtkzptqrit.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtadagzxwh.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtpgxemntr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtetyqoapz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtwjczmbco.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtwbtugmbs.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtdsdspthb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gtoephphde.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtixdkopya.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxinkj.top/gttxixireo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtfxojqsbw.html

[L02] 发送 POST JSON
来源：http://hz.gaohongyu789.top/gtmnjwikqz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nwbrower.top/gtnhxbewuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gttcbvmgqv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtjaizhbec.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gttmsxgkpl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cdnleiting.top/gtkziwulge.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtfnorerqx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gthjnsfada.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtsgikzbty.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtxrkkyhfn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gtaozewzpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtrfxprpbg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtqvhwsrfz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtupgygsfl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gtdjhuoqqc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtwhjumhma.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhongyouzk.top/gtlhzxdxut.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtwoybdjpp.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtvnnbohfh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtcanifrxl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.feifeiyinyue.top/gtumwkuecx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtgtkyptxm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtazircoaj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtayssqnsu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtdcetobye.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtittukxpy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuxming.cn/gtocpcmzck.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gtikmghryh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtnzoxidox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtmvasmopg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtqvftjwkn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtftuasxlt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gtqdrtydij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtgmvuxeuy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gttqbqjvii.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangdashe.top/gtzbidylny.html

[L06] 解析响应为 JSON
来源：http://hz.xuanzx.com/gtaeqfdzak.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtvvwiejwy.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtfrtpilcq.html

JS:   await resp.json()
来源：http://hz.52xcode.cn/gtpeidxsig.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtsaujhurl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gthcfoffab.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtylfvorif.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtuhnudytu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtffhonjcg.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtramjoxtr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtwkudksvu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtsycbzqcu.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtzucguuvp.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtrchagyyp.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtbpyububb.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gtmazmvjoy.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtzdlqpcqa.html

C#:   (int)resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtcfhvzrcc.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtyishubbp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtqouonbhv.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtwrkihzrp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtwkpossjp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtzdkfmzpu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtnfvibakm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtwysywhke.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnxiangtu.top/gtclwjrfio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtezjzagos.html

================================================================================
来源：http://hz.c1oappe.top/gtxuqwehwt.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtxishyybz.html

================================================================================
来源：http://hz.chenzaomai.com/gthrglbryp.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtfzicirtz.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtzkjupwzo.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtjdcfvoda.html

JS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtbfmeqsyx.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtfgsjwhpw.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtloxzsfrl.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtwawjhpfc.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtxpdlcnfj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtnwgdqlni.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtetjxouui.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgufenzy.top/gtddmgollu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtskilmwuu.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtcawecpqk.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtzznoaaqx.html

Java: System.getenv("HOME")
来源：http://hz.jiagoushi.top/gttctafgga.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtknucsxja.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gtxrxdvped.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtnndxogdb.html

[M03] 执行外部命令
来源：http://hz.xuetiantiany.cn/gtocmasnjl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtebptofrv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtdetrtvxd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtebagkwjl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtpanzbzob.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guowangkeji.top/gtuvzpeqlt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtlzpbiwep.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yangfankeji.com/gtbmtutqep.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtbhdphygd.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtekjwvuxd.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtrveyymrm.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtithyxdxb.html

JS:   process.cwd()
来源：http://hz.fengsongda.top/gtjozjpeyw.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtiwmhxxpa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhongyouzk.top/gtyspmrwlt.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtomojkspp.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtakckinjy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtcojxiszm.html

[M05] 设置退出码
来源：http://hz.zycfv.cn/gtmxbpgdhr.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtzwtcwvgu.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gthafoebkh.html

JS:   process.exit(1)
来源：http://hz.gzhubu.top/gtypdhenuu.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtumryhowr.html

Java: System.exit(1)
来源：http://hz.fzhhl.top/gtuqpoeqyc.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtlrlosiqm.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtqklevzbn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aizwys.cn/gtqggigtgz.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gtuqsbbsyy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cheryme.top/gtiwshhxhu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtdmqbqpnq.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtnjmrmqaq.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtlnlyqgex.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtorrcacvt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dashuyun.cn/gtlntxpgld.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtfuudasir.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtrhpxlubc.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtalmwcqfi.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtirbgvyhv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenjidiqi.icu/gtiismdrno.html

JS:   require.main === module
来源：http://hz.sweek.top/gtkqnujlhy.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtrhtlpyjg.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtdmluwkes.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtucnpotav.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtnmhfyqpe.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtaswpkacs.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtpmtmfwhv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtidvdhdyg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtvijvzyea.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtojfcjpsu.html


<!-- 参考信息 -->