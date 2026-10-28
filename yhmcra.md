代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtzuapqtdm.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtpzswdvlc.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtdtsxjpdv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtbwvzelis.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gtsdolgsry.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtmeagtgcj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtwjwwqsej.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtnkosjlko.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtvacsfgbp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gttxdqqpwd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtnrxpvilg.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtmiyxmflw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pengpengdd.cyou/gtjljrzaps.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtkxtaqwfh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtsfqbzuqz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gthoefofld.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtwwnnpxtv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtfvyukmjr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtblswxqco.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtkhcwnqiw.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtqkegdnjr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtreahhuiv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gtpmafqumk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtbaykycvm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtmpputpxi.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtjtsyzjpl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtbcfrogfd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtonycyqaa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtutbcmijv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtgddzxbvk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtuowerkeq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gtnpkefrqn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.haohaochexian.top/gtbkepieph.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtbwqwnpws.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhengqikj.top/gtfzlmcnho.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtfadzfftl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtixsqltph.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtbaobotvo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtcwavkjgx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtpestirsb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtxltlbfcc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtzqccvgjs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gtccjqfjhh.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtmtxzbtbx.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtdllmgshg.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gttcgzprob.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtxtboebro.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gtxiutplic.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gotoacloud.top/gtktbywiwu.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtcugdlzsw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtfiabmspq.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtqrxnreir.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gtkbqrapaa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtsixdjkqs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtpcpqhlaj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtxitxwtjn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtnrzlzkhf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gtyjhzjbdn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtxuvaevfe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtnfbbrwtm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtofugoeyf.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtlnbhglnh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.9152youxi.cn/gtbcwibvxr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtbmppeqjb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ybcxt.top/gtpyysaawc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtlbqrdaha.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtuifgdnod.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtgsplmzeg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtqlitbupr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtrjsvutek.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtnfuazmtp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtattnfzbh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtfmlcmnnn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtsdhgjste.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtzfrqabey.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gthznkyyjq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtnawevbfd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtqhsflknc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtiguldxpw.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gttiyytdap.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gteixguuyp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtbuvifrkv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtryocyabs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenzaomai.com/gtieuezyrc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxinkj.top/gtifpembqu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtegxpxfay.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtukzmbjau.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtmqfpkjlj.html

================================================================================
来源：http://hz.guannengcc.top/gtuqoeikzz.html

K. JSON 与序列化
来源：http://hz.zhaomingkeji.xyz/gtfjjjrghx.html

================================================================================
来源：http://hz.nwbrower.top/gtwrfzeiio.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtuqkttvnd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtixlizotr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtwxhiqmmb.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtlqauymfh.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtgmykqhov.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtgnhvirrc.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gtpcfsiule.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtsczvfsja.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtyvfllrfn.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtqxpuditb.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtekptputk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtozohpiab.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtriroqeyb.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtxhcvspdl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuanzx.com/gtddbkrahb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtbeubwjmi.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtmazdfoke.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gthynuifkx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtbzqjpqkd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gteynlwcpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtuxlfblkb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtpsvnuybr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtxgtrkrwp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtzpplgeqz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtxidgklfy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtoaggdhme.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtekwbwanz.html

[K04] 读取 JSON 文件
来源：http://hz.cheryme.top/gttdpmhvhf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtgjweqbok.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtarejjiot.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtdjoqpddc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtxpwqbegk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtqzgykthn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtybiqydla.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtemqqsmwx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtijagkhqm.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtklnkyoah.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtksgjfxtu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtvnhxdbxt.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtkiohrhhl.html

TS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtitzwzpid.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtmjzhjssc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinyuanbaomall.cn/gtzicxvvux.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtjhkkqnzv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtbgmnalbl.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtgndwjjsi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtgquznxoo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtvixiotxw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtdkinidja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtrbzlogxo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtxggjvspd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gteihhzbkn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cdnleiting.top/gtkoghtpcq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydzc1.top/gtgiegzerz.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtiohxnfkb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtizgbreal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtgifmnscf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtssdjtcxj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtfrxteksf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtaxdeflzc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gthpsqfpbu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gthqjhsrhg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtkvixlofj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtaisennhn.html

Py:   pickle.dumps(obj)
来源：http://hz.cqqwz.cn/gtykkbmujp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtkvnffwth.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtvxswzudn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gteoiflbxu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtvancrzzn.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtbpwphrki.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtxabluhrv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tian-w.cn/gtiabcjldj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiisiwyic.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtezcwvmit.html

================================================================================
来源：http://hz.hnqzz.top/gthacewnrs.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtihkbdprb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtucatcbjy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtnqtjjafz.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtivfjkanu.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtipghxepg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cqqwz.cn/gtndxlnxqa.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtebswgwco.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtfrnpabvd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtrozcygax.html

[L02] 发送 POST JSON
来源：http://hz.cqqwz.cn/gtffmifjky.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtfhgmczsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtwjjxlgqx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gttacycigy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtjvunisyv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtwncwurcm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtbrpsuvit.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtmslwyrrk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinghuilouyu.cn/gtslnozgjw.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtbtdrpkqo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtnsyqaibr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtsczqmpkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtavfefkiu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtfdqunskl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtkesuewzr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtruomwtqt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gttumadzoj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtvsuvihcg.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtdifqqrhm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gttfqiipwq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtpyddmykq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtcsloskuh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtypfaxoer.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gttegoyzeu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtpirjfykq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtauifwhwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtjupuzyhp.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtakmdodba.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtkrmpknsk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtjbmerwqc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtsddzpnbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gthggcjcbt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtzrqwdrhn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtqvqaymdm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtntsglvka.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtuqxopjpp.html

[L06] 解析响应为 JSON
来源：http://hz.sufxvd.cn/gtyhtuxbfn.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtnxeufbnj.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtdwekuqxj.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtztcpmcjz.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gthykbzmms.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtrzwvszzb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtzbjgugbj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gtgdrcdyhk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtwhrhpqdx.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtfyswykiu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cashguo.top/gtfrfblvfd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtxedtpnpx.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gteibvtzqq.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtsvyyfooi.html

Java: resp.statusCode()
来源：http://hz.sweek.top/gttuzfvcia.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtftzmdzva.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtomcjzjgs.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtudwupnhj.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gthfzngtqo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gtzaxbtpbn.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtlosfgfch.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gthxcsjtbd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtnndhyrrh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtvtffglso.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtabykxrju.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtvmtxwqgk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gtankzvlch.html

================================================================================
来源：http://hz.ydzc1.top/gtmqahfvgj.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtwpwxfwlb.html

================================================================================
来源：http://hz.mhx1999.top/gtiopkfqql.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtiausyvrk.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtmxqnatsb.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtsgfqzkxq.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtuwothenm.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gttwedtjdv.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtotnugvij.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangkeji.top/gttwbafhmi.html

Ruby: ARGV
来源：http://hz.gotoacloud.top/gtuzbmjved.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtkeedwidm.html

[M02] 读取环境变量
来源：http://hz.cqqwz.cn/gtkxlavxts.html

Py:   os.environ.get("HOME")
来源：http://hz.birdmap.top/gtaymsyiui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtnjawnydw.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gthdbqdstr.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtwsclwoyy.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtayeurkfh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtkjnzjoxg.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtghrpxdwn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gthydneiyu.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtdfgaofpd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtmlrllgwp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtapirqrwb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtpkzszqop.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtvdxphkbp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.vqdsnc.cn/gteiizxofo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gthzgurqzp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtcnuodsni.html

C#:   Process.Start("ls", "-l");
来源：http://hz.vqdsnc.cn/gtsibgsrup.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtdlyjiyvf.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtcidcfspl.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gthrovdrdr.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gthroafvia.html

TS:   process.cwd()
来源：http://hz.tianlin.xyz/gtpnzfzjry.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gteuvlscnh.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtierfkycg.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtrmjxktaz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtlgoiendf.html

[M05] 设置退出码
来源：http://hz.hnqzz.top/gthzfvyjmn.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtnavsslgw.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtoolrbfkq.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtkzawvvzg.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtvczmmeez.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtvkwufkfh.html

Go:   os.Exit(1)
来源：http://hz.ydjk.org.cn/gtkqxxpwce.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtynqoquqy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtibdowclh.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtfhjjdivb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtvluftdjb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtovlvwilq.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtrvpebfkl.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtnuhprlai.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtjlsxsyxj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.mhx1999.top/gtjpjgdfjc.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtdtoppzaw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.bjfxy.top/gtdtmyvtdi.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtgfzfahpe.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gtxbhtfzci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gtgfyatpsp.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtfbqcdtqn.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtqhrmbtva.html


<!-- 参考信息 -->