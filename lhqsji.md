代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtsolzlcoo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtaddnkffj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtdcrezzqb.html

JS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtqsfvyrmj.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtluxfphpm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtsphozfpr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtlwxwmsqs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtmtpikbic.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtckrapydz.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtzezzmcxv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gttcaawitr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtcwvhlxld.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgfzy.top/gtxnehaeku.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtensoukbt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtugxbrwuh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gtaxjbkxml.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtivyplmbf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.feifeiyinyue.top/gtxcvvcxqb.html

[J05] 时间加减（加 7 天）
来源：http://hz.gzhubu.top/gtmzyfigmg.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gtvaktfrtn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtuvlgbafy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtyxgklakv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtxrrpiemc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtrmxkjgew.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gtuxnazsnn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtufgbniri.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtrjhrusse.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtasjkintt.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtspkrppmp.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtxwbzjyot.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigufen.top/gttwspzuyt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtnkyojpww.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtnafqxydg.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtntaadtbn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtbmlvfhpd.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtietdlzoh.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtfziynjeg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtfeafzbqm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtieogylru.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtvsovxygh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtdalcjpqh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtlwhledos.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtufacnndc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtlernnivd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtqcwmzyxz.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtvjhguxjz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fengsongda.top/gtlruuzllv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtfingtaiw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hammf.cn/gtpgqwrzqg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtbemmenua.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtalylubra.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtbbmptpwc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtqqoymalt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.9152youxi.cn/gtylkykojd.html

[J09] 时区处理
来源：http://hz.bjfxy.top/gtzjeilnnh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtmnjciwoo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtrvbvdoxs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtpblawqza.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtwkyxbtbi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtefqlwnpk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gttcwsngdk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtskkpqknr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtezxpvetw.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtervtbeoy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtfwbatixf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtjcgmcrkt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtfptvzgki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangkeji.top/gtusifsgrr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gtvodopjkh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtddkfrvti.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.haohaochexian.top/gtfojhbgdo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtegkmfwzv.html

================================================================================
来源：http://hz.xuanzx.com/gtyjwgbdui.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtqgugsdqn.html

================================================================================
来源：http://hz.svipenyu.cn/gtnblafdyp.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtqpubsumk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtzivradak.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtjcyaxwqe.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtbyjyyuih.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtmsjcdsil.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtcbyjmeox.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtlkwvjqtz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtgnmsmset.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtebmuijfh.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangtech.top/gtqbbsmyii.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gteszepmkx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gthhaefqlk.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gteehnqbey.html

TS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtoxefwubp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtpmmwdjlq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtqozghjkv.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtljyotjqm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnqzz.top/gtbmatxkqr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.feifeiyinyue.top/gtkokmpkbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtrmrppdit.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtoqusoeof.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtaevudmfq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtepztbsye.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtmeimrihw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtwquukpor.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtforouzpq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtscgkokxa.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtxbjbwwvo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtdpsqbdnr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtitfokzvh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtrnlnhbbo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtkaoczmfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtcxozycra.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtbghmirho.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtyxibdvdw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtnpmzrjvu.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtchmtprmh.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtcuaotmmb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangtech.top/gtinhebafn.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtkvtcaocl.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtznauyytf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ehwqpu.com/gtdiqqgsqa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtnxlvwlnv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtsxodgtxb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtlnlbieum.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtmuhmpdxv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtpvoiikuf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtlnyornhy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtordbovng.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtkeicwupk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtimpwwkdw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtfltyrxda.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtxbqjelee.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtrmrjfezn.html

[K07] 进制转换
来源：http://hz.cqqwz.cn/gtfeqidmbf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ehwqpu.com/gtjpedsxsc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtgqqwmefa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtdqpedfeu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtpuefylnm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtfpkreuro.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtjufztezk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtdcopmyjb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtexsdbndk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtdwvzwvyh.html

Py:   pickle.dumps(obj)
来源：http://hz.ehwqpu.com/gtldkcgqjq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gtwiiezzgh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtwndnfgrz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtvchpgmaf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtjlsasecs.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtfffjdule.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtkrqcoili.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtftwueebu.html

================================================================================
来源：http://hz.jianghu66.top/gtgnikuozt.html

L. 网络请求
来源：http://hz.hammf.cn/gtysdesbhj.html

================================================================================
来源：http://hz.mhx1999.top/gtzuqyaall.html

[L01] 发送 GET 请求
来源：http://hz.jinqigfzy.top/gtytkbccvf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtejbapwtd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtuaztdofk.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtkogckraa.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtsjxfixve.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhiwuduotai.top/gtgakbaasc.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtsketnzbz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtygbwltwc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtnnhqntpm.html

[L02] 发送 POST JSON
来源：http://hz.yonumen.top/gtdmlmuvbr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtfpetvavw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258888.top/gtttbqshdi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gturtrwjxs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtkryxkelu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtyipjrpyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.vqdsnc.cn/gtwvlnbtoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gtmzwkkadm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtzxivzbku.html

[L03] 设置自定义请求头
来源：http://hz.wangdashe.top/gtnpnxpqby.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtlmatalcy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtpsiuvvro.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtopvuapug.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtjyutbyfh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gtvyqimotz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtynzngksq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gttmddkxfh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtjtboutoc.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gtlasqqqwk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtscxpfbxn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtbkcxwrdp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtgcghstxf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtmtnynxtr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258888.top/gtbrzucyqz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtmhjldemw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtyyjtkhxo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtqwupvvma.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gtjmjexzbh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtujnaneyq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtyownfmkp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtmxjxwxed.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtciarkiwj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtdafutjll.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtqoypggde.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtvcvfjngz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtcbukzaea.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtrohniexa.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtgkwipwjf.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtbqtglogm.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gthrafznwt.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtrpfanqdr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtgiznudji.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ybcxt.top/gtpojjhlfc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtdzvexrna.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtftzmuzwu.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtprnwogkw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtmwpmgfoe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtgdterdkv.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtvapkjynt.html

TS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtrzpxaqeb.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtlxtyzamn.html

Go:   resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtnukzadcg.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtxzeyvnni.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gttmdfnruc.html

[L08] 并发请求多个地址
来源：http://hz.dianchejie.cn/gtvihhndvz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtvruhcuuw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtngvhebgh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtpliverqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtabvjvaym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtitnhlzym.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.havefunace.top/gtjwjmnsbd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtswlufmxs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtoicbasdl.html

================================================================================
来源：http://hz.zhixingplan.top/gtypqhmebi.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtghngfqqr.html

================================================================================
来源：http://hz.yuxming.cn/gtkhusexrl.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gtlnoiteam.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtvenafkvl.html

PHP:  $argv;  $argc;
来源：http://hz.9152youxi.cn/gtwfekpldf.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtpflksouq.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtyuxzirww.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gttgnhggqb.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtyxkfowei.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtmjrymwvv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtcnpgdosu.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtfwpywijd.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gttenknubc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtmamkdpkr.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtzclrmoma.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtwhkcreih.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtaygwrarr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtvwgrcxha.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gthahfsaqh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gaohongyu789.top/gtppxikubi.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtehgamibt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtaohnryre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gtkgqgcobf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtpheeurzd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtortscrgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtwabdsbkj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtwrhzeycd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtliuduzdn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtydzpudvw.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtvgfpieyf.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtvkgcroce.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtxmascxve.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtbryznaen.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gtfwsuqmtn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtihehvmti.html

Go:   os.Getwd()
来源：http://hz.cashguo.top/gtcnmrwfpi.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtsrrovacr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gtormvhhqj.html

[M05] 设置退出码
来源：http://hz.dashuyun.cn/gtqhyfbkrt.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtjmsgfcrw.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtqxlnqtya.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gthtkfqaig.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtccvenbgd.html

Java: System.exit(1)
来源：http://hz.tanke756.top/gtdyukzloj.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtyhonubyf.html

Ruby: exit 1
来源：http://hz.sweek.top/gtnxrabyvt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.c1oappe.top/gtsiilaero.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtnmnywdcl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtrlgrzamk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtwwlvcomv.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtfedqmczd.html

TS:   console.error("err")
来源：http://hz.havefunace.top/gtehnevqhr.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtoavpespt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtpsvjlowm.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtcbmxmevp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.meibo888.top/gtocjbjdja.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtzzfnuxfl.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtmhcqlmmw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtafcizrzo.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtvepaluwk.html

TS:   require.main === module
来源：http://hz.xuanzx.com/gtnqjlkfoc.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtkcgvrfmn.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtqsmsmxhl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtpwhteehs.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gtaxgremgo.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtdfqxifqn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtsmxegbrm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtaelcumec.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtexwbcsdw.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtnfbmsdfa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtdcdqtzij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gzhubu.top/gtmkuxtbcr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtsfrsgajg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fzhhl.top/gtogqpjysw.html

================================================================================
来源：http://hz.dashuyun.cn/gtjdewnhsw.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtjkdzhnew.html

================================================================================
来源：http://hz.xziqi.cn/gtazekrfol.html


<!-- 参考信息 -->