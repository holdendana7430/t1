代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gteebdexby.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtkqavsxnh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhengqikj.top/gtchrkqbye.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gteucmdfvj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtxzqwfcdm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenjidiqi.icu/gtotfblerp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtcabmhnip.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtdqkznltj.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtzheauqia.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gtljbnodum.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.meibo888.top/gtzwtmxxeq.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtncmrjppb.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtyyzzgqxs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtuwrcumdi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gtmptvknoi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtzqpitmht.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtsweprnrz.html

[J04] 时间戳与日期互转
来源：http://hz.hnxiangtu.top/gttjidkibl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenjidiqi.icu/gtelfoyehl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtlvqtsdep.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtoulhlmqw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtrwdcyxhv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtazegnqgg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtpfwlqegs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtqoossnvz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtwiibmndv.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtonbvwgld.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtohuqbqto.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtvbsdrqmu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtjdpgtyth.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtgaarfigl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtxykezjhk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtqxmbghja.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj202588.top/gtcyabrtia.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gttgnkuwes.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtigmqtidi.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtsqmhtooe.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gthctgnjxh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gttpdmiwmq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gotoacloud.top/gtxscufyys.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.9152youxi.cn/gtgykwflss.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtsalxggad.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtploflfut.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gttucjvzsz.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtbihudamy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gttinuracf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuanzhike.top/gtmtdcytnt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtypyneffe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtibnjkkij.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aizwys.cn/gtvmlcmcrj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtddxdihrm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtnfguxhvv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtqlrnobca.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gteuynpapo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gtiyqeyjdt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtcdxvgpna.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenzaomai.com/gtbnyhuqab.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtynammrau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtjjdxbrsi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtezlllqtw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shuidangran.top/gtvkxjzzfr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtsplascgu.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtrnuslfia.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtaxtxdvre.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtuquuujrq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtnhkxdmhv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtlxqwgkms.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gteioomwlh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtqkykpdce.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gtgulttkjq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtjsznnjga.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydjk.org.cn/gtjkzazxbr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gtqrovxuqw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtrjwuikwn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtmqenbtnv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gotoacloud.top/gtnseakdqa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtfputjcor.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtofvdfbhv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.kuanghao11.cn/gtrjjcgqol.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtsgtsayva.html

================================================================================
来源：http://hz.xinyue.icu/gtjwynshfm.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtvyrtgoll.html

================================================================================
来源：http://hz.xuanzx.com/gtpqzyliqn.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtonydnqmk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtitndgimg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtphhjasdo.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtvkfgkdwj.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtnkwscmqj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtadxmlgwf.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtkbvanhdx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtzpgnhzvs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnxiangtu.top/gtdtllkgac.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtitistwwd.html

Py:   json.loads(s)
来源：http://hz.tanke756.top/gttorncwnr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gtizfsjeqd.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtnfgkmvyq.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtuiiogaop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtxpueuqap.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtgavjyjsa.html

Ruby: JSON.parse(s)
来源：http://hz.zycfv.cn/gtnszdfdvb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gthnhkcvae.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtvmyjlqrf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtsggirplo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtrcldfbip.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtzkaqemmm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtfwmocryq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtirsepxxp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtwqbizkva.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtupettxjs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtdlqqalki.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtvjopauil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtwjwnsgon.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtruzsgqfn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gthrmpctxo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtepujgpcw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtgfmlsrkq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gthitszmna.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtjigpyxqp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtsvbnslni.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtpwjpjqmc.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtpgubvjch.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtyviifjrl.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtmwumrdfx.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtgkllkrhq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtxjdwsojg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtslbvmhpb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gthupbdhxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtaenetidt.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtnswbhkiv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtuclipyzy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gthzhgczcy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtwyvjjhvi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtexupsfwu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhixingplan.top/gtmuiyhhmo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtjxhxgkvs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtlpewzkbc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yueranfly.top/gtxeqbaoex.html

[K07] 进制转换
来源：http://hz.0kj1m.cn/gtaoavwgpp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gttdxpiqod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtopwbryid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtqvfnqzit.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtlqcnvsfe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtqthnbkom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtmgkgpcpk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gtjntszdyk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ybcxt.top/gtbuvzvibf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gtdxeqacky.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtmjtwheid.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtmumafnmf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtqzowbdlx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtpldzdgjp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258888.top/gtnwuuswuq.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gtfwjiupvh.html

Ruby: Marshal.dump(obj)
来源：http://hz.nwbrower.top/gtdupeehcz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtjcilyzdb.html

================================================================================
来源：http://hz.aibaodan.cn/gtndldidef.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtifypjyva.html

================================================================================
来源：http://hz.dashuyun.cn/gtpnrzpyat.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtoeahjinm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtymqmfeqp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtzpdomdlr.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtaptqyqvt.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtrtkynfkh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtazvzvbac.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtbbrftiyv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtcqhgmdeb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtzsnbndkd.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gthbexkcfy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtbmzxxjpi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gtzfenbfkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtktpjroxo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtdccmuefz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydjk.org.cn/gthqfkorjx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtlkqsnslu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtnndlnpya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gttjtdqsns.html

[L03] 设置自定义请求头
来源：http://hz.pengpengdd.cyou/gtezwjxwdw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gthrrxqfxs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hywenlv.cn/gtclbfacqp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtsvimcqkj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtxtuqjvhi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxuanxn.top/gtbcjuyxaq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sufxvd.cn/gteajgaffy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtjrxiwsbb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtacxnfdit.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtxbfpxelg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtpmlrpnaw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtpkbpjhik.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtntzagfft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtqywnsdyl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtxbcewhlp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fengsongda.top/gtpofhshqp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gttqnbamgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtbdzwdvxs.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gthbazralv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtkxqziugf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtwjjihniz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtzceqvtbp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtiryvofru.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gtnsrznser.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtfrakyuen.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtaoswiwiy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pengpengdd.cyou/gtvmknvkjf.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtciullgoo.html

Py:   resp.json()
来源：http://hz.ydzc1.top/gtpdpqhkwq.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtdcammguz.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtfravrxln.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtbckaesrp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtifpbpzco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtzitstdit.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtlyvtvpzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtysjvjltv.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtrlfyydrw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtnsbdtkby.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pengpengdd.cyou/gtsaqicdgk.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtinrrhohc.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gttmiktidg.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtdtnszgcv.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtwmrbhnjg.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangkeji.top/gtjookoguj.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtfywqmqat.html

[L08] 并发请求多个地址
来源：http://hz.xylfe.cn/gtwgiemwvs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtcwsyevaf.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtvslemjue.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtwtsxwmlg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtpzjspszc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gttaezaeqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtleukzqbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daria6918.cn/gtrytrenkf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtwbihyqja.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmemgdgwn.html

M. 命令行 / 进程 / 环境
来源：http://hz.cdnleiting.top/gtjiryiqwl.html

================================================================================
来源：http://hz.sweek.top/gtsqqukcyw.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtpsfrriyv.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtbvficoyk.html

PHP:  $argv;  $argc;
来源：http://hz.cashguo.top/gtcsbhdlsp.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtrtlachjg.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gthswjhaep.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtmrowdoag.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtlgihfgjn.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtliwtfiyb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gthcvarnje.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtqwbaynym.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtpjxusnjv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtwwbjtjhh.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gtwnywyepe.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtdcpybcsd.html

Java: System.getenv("HOME")
来源：http://hz.jinghuilouyu.cn/gtyuiwbunt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtikyhpwqp.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gthfpudlro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtrmyoafuk.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtvuvjethm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtalzcqqsw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtbynioiib.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtiusosskl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtwfuyctnv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtcjnhpqsk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtwhhjgjna.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtrrnidgcp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtotktdcgz.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtfimztfjl.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtapzkuuft.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtvhvcorly.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtsxfcifwz.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gtpdyypvsq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtnrbokrzo.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtgxftmwny.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtsyfpgpod.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuanzx.com/gtyacnifvv.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtyfcoulqj.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtofiysxxs.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtificzpab.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtkumlzovj.html

TS:   process.exit(1)
来源：http://hz.yj20258.top/gtunprxumd.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtmfcnmwop.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtsbygrumf.html

Ruby: exit 1
来源：http://hz.pycfn.com/gttsojsnlq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtazpilags.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtdtgaliop.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtczynquit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnxiangtu.top/gtkztrlmnr.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gthwwvmiqy.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtvwblviie.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtnmethnmg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtoegnniui.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtuvbrkofh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtrreivlay.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtnidctmuj.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtnnompqwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtteiiyovn.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gthgswudjz.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtomqujery.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtjohbvpms.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtenhuqmwu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtxqrphhkx.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtbwzrkyjn.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtjwdvxjln.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gttbqqboia.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinyuanbaomall.cn/gtqsksgpwe.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtvrrwqcle.html


<!-- 参考信息 -->