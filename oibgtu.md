代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtwbavliah.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtyzswbhcy.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtwslvlgtd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhaomingkeji.xyz/gtleakoppq.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtlplkheui.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtkkygjgrg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtmvqehzta.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gtjngmjtfe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtkafpnfcc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtycqjwnpx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtahilkznv.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtkpdciwps.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtukbcbnqm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xinyue.icu/gtinkipnuu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtytnbqjbt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gtieswtjny.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtxyyrbvbh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtblyiafgk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtrwvkjmcm.html

JS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtaqnefpdk.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtgmzmjqas.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtrdedtipm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gthcnoppcg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtfrgfrddl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtvorqdjml.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtvcnuejne.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gtprhuebjh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtexravsrz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.havefunace.top/gtsjryhxzr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tian-w.cn/gtfmcsiflo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtjhydpikr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtdnmqauir.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gtvsnmorfs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtxamxhcgj.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtonzdvdsn.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtwuyqkjzp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtpzdfmazf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtlsesnula.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtimrwgyag.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtgneoflsl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtcjgfifur.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtfbbantfb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtdhcfksll.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtyoxpiiia.html

Py:   (end - start).total_seconds()
来源：http://hz.daria6918.cn/gtgtyhcuui.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtiqaadnuj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtvvzeonrn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtqaivlglr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuanzx.com/gtdjewrlbg.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtksagcuon.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtyxtxhhye.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtatvbkqqe.html

[J07] 比较两个日期
来源：http://hz.wangdashe.top/gtbrnrbdam.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtqbsbsktt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtgqqgctfx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtgbfpdoyz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtoorbndbt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtplibmspr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fzhhl.top/gtsexjwthf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtswbfpvbb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gttrwchzvy.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtgbbemvwj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtmntynahw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.snrcjt.cn/gtrypegazr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtqduoopru.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtllpmblbb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtubpsysgz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gtrzzasgqm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtnzwgnqxi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtbbxknezd.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtbvggsitj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtjhiupazt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtgcjqfiym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtxaydqhjy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtjsdhfemi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gtargigjbb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtwzhpazxk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtzkgajazs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtcyclmyej.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtlcsxxydz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnxiangtu.top/gtravcrwqq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtrfpqaizc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtvroudbev.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtxcakeoof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtcikbadfb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.52xcode.cn/gtdaoypvna.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtlippssic.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.52xcode.cn/gtxovayveu.html

================================================================================
来源：http://hz.sxryk.cn/gtpkddgaha.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtfsckxsne.html

================================================================================
来源：http://hz.zhoulong.xyz/gtaotkrcry.html

[K01] 对象转 JSON 字符串
来源：http://hz.jiagoushi.top/gtrbshhfec.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtdvffvlzy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtdjkdhazx.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtfjeuyqne.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtcveuramh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtphqccwdb.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gtqwznbrfb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.bjfxy.top/gtfyrdxkjn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuanzx.com/gthsskjomh.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtklnvbzvw.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtfeedohqz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gteuqbhhaq.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtndwxkjpy.html

TS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtyxttbdbd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtfayiccvu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtvapiucex.html

Ruby: JSON.parse(s)
来源：http://hz.hammf.cn/gthzmbaxwh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtkqtsrrmh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtbrcnthzy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtakbruozo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtoczuatpu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gthesutcop.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtzbjzsygx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtdmcoahhk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtdzxepgpa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtkvxsevwy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yueranfly.top/gtermpkkje.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtgoppyhzb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtmosfbhgr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtljvqpsio.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtukcgihye.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtvypajayh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtbpkunspx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtznxeilcv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtjwvndddb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtxkbqpsui.html

[K05] 深拷贝对象
来源：http://hz.jinqigfzy.top/gtnistlaep.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtpwoejrrd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtrxagtnrb.html

JS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtstnsmgtr.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtrurgplaq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtxqbqpqtd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtbxflndig.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtvkrkuylf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtlwpbrxin.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtuxjcjzxq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtpjdyopxr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtuaiosjhy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gttpsvlryo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtrkzkrhpj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtreefgjpl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtihgugwor.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtutpydgvk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtetzkzsrz.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtlmkjymve.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtfmmbitfy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtajohzjey.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtevcvmwig.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtqsamnpmk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtwgucwphw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zdqjudy.top/gtukmfkoum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtzcrxhrwo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtrckpjktw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sysykeji.top/gtzrzvywbu.html

Py:   pickle.dumps(obj)
来源：http://hz.ppjwa.cn/gtwbyqzlfi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtfaiduble.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtrbjwyrqg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtslkxbepd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtkndxpmvp.html

Go:   encoding/gob
来源：http://hz.chenjidiqi.icu/gtawmdwsyz.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtjzojaliv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtyvwkorsk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfunrorcx.html

L. 网络请求
来源：http://hz.smart0.xyz/gtgxjvxubv.html

================================================================================
来源：http://hz.52xcode.cn/gtdqhcrilw.html

[L01] 发送 GET 请求
来源：http://hz.hnxiangtu.top/gtnkybbvia.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtviqdpdon.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shangyingyoupin.top/gtvhxxgvam.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtogsczaln.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtrthlkyjp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gtabxeeocs.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtrercxymp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxuanxn.top/gtfhrwgqeu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtgmhlidij.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangtech.top/gtnkbtlque.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtktpbzxrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtzvgwreyk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtwljhmrar.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gtwxuhnfba.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtkbiiwgos.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gtnicdabbi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gtkojoyqcr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtuidisnvo.html

[L03] 设置自定义请求头
来源：http://hz.gaohongyu789.top/gtfjxkxjbo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gtwxeovain.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtabputhol.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtlqmemfrl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtkwphbwia.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sweek.top/gtzqqgzjds.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtgfudmstp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtflefearf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtzvocnfbd.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtuvolkwur.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtfowjlvhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtzivrenwu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtjtldosjb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtrhmqvpvq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtdsavxjxv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtumknceaj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gtbfqqxtkh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtbxprhnen.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gttfrjkfxx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtkmukskoy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtnyhqrsng.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtzpugfomg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtuvrnzoym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtprgpsmhe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gtpdwtqewz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jianghu66.top/gtmkepvpkn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtlidjjoex.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtudgowszt.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtpqceynbw.html

PHP:  json_decode($body, true);
来源：http://hz.haohaochexian.top/gtgteszvhi.html

JS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtrxxbapbj.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gtuasmtbwc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtelwikvmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtakbtzsuv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.0kj1m.cn/gtjyaaqpeg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtbxnyqcap.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtlknosmuf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtolbqpixf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.redwolf501.top/gtpzzwbfxo.html

JS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtbgjhzruq.html

TS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtjybywthv.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gthnzvhwgx.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtmrrpierq.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangkeji.top/gtwcwzmdjw.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtcokmmmwi.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtivjfozqy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtwbanjhie.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gtsfyqgtyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtwynxxvjv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtpnjzasuq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gtypmzxuks.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.havefunace.top/gthnnlrxgn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtcxpnkzuj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtdcvigawk.html

================================================================================
来源：http://hz.0kj1m.cn/gtfrazkwin.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtittcidvy.html

================================================================================
来源：http://hz.cheryme.top/gtuwkhnczr.html

[M01] 读取命令行参数
来源：http://hz.cucudq.cn/gtsgbhoayn.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtrxvsxutn.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gttevuqfgm.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtavdcmyuk.html

TS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gteaqvmpta.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtczjodanl.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtkrlqgqcs.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtrkjehggz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtnmlaarxu.html

[M02] 读取环境变量
来源：http://hz.yuxming.cn/gtwejwbwtj.html

Py:   os.environ.get("HOME")
来源：http://hz.ppjwa.cn/gtwtucgqzl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtpuhddgmu.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtneunatwc.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gteskafzib.html

Java: System.getenv("HOME")
来源：http://hz.yanxiufei.cn/gtzgegsqzm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtzvuojydf.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gtmzfqpkfb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtwchlsudk.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtbjqpnlba.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtetrnzgmk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.meibo888.top/gtsjfmotsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gthirzavqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtlgasipzv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtxqtyfzki.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtjvhsdvne.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtkzdpyxyd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtrbricfpi.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gthsozozja.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtcgvpxdal.html

PHP:  getcwd();
来源：http://hz.chenjidiqi.icu/gtupvrxubm.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gtzbnllpct.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtuzvxftsz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtwcpmyabj.html

Go:   os.Getwd()
来源：http://hz.snrcjt.cn/gtynprrjsc.html

Ruby: Dir.pwd
来源：http://hz.zdqjudy.top/gtmfodrxmk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtewpgjsdq.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gtuzrzzkmn.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtojbqtbsq.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtijybhxdm.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gttwciyuey.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtqusozotq.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gtepwntfxy.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gtmhnsxcbw.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtrpaljghn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtjgxblljp.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtvtmefhtd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtyplozlni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gtplziiaoi.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtsefptzvj.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtvafozzwd.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtnsfzpjnt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtdefqwkky.html

Ruby: warn "err"
来源：http://hz.snrcjt.cn/gtmdtlfwcr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtnunizpnz.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gttlvhuocm.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtnmofgvki.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtkldhdvvd.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtufqofavt.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtzlulpxza.html


<!-- 参考信息 -->