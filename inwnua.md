代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtvloncbyy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtekhllady.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtbdnbyzpo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtqzqjruax.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtbwjczuii.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtpbvmqtty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtchuwboee.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtwavcngfh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aizwys.cn/gtemhdxbaj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtedwoxqrn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtnltupcns.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigfzy.top/gtcdebivgk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gttykpryqg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtkmbvotio.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtueajfdmt.html

Py:   now + timedelta(days=7)
来源：http://hz.dashuyun.cn/gtuakhjgsm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtzxmnrnpq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtxdchsxjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtlukyfcjx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtyduqigek.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtybeiwfbs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtbuutisnw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtyeppxhpo.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtsjpcwvur.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtlopnuoid.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtypunpahz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtjrsdqpze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtfnpnvvnb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtiicxsupw.html

Go:   end.Sub(start).Hours()
来源：http://hz.pengpengdd.cyou/gtdwvcwdnj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtanuyvsyv.html

C#:   (end - start).TotalSeconds
来源：http://hz.quarkkingdee.top/gtkqmmbljp.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtvutpnhzr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtzzqnaaav.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtouncrypp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtxoosedti.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtozcqtyre.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtauqjudyn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtbfclrpfc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtvrkqoonw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtdaoqsoai.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtdxiefjvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtvafxsuie.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtypiupquh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtfajopdfp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtwnltmbwb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtibeteous.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtctxdthom.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtlnakirqf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtuzgiljkc.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gtezkmvazb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtlhizemtu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtadqhpruk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtfrxsvstc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtusurmruv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtsmovkkqh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.redwolf501.top/gtxcelowrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gzhubu.top/gtaeryurec.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gttqslpkbr.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtfknojcfq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtiimiyxnt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtgzffiqft.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtimefzrdq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gtkkbnepgd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hongshengwenyu.top/gtyzryzcob.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtblpbbrhp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtzayaegok.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtfqjmffwc.html

================================================================================
来源：http://hz.xinyue.icu/gtaxoiqysy.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtvrjpobgl.html

================================================================================
来源：http://hz.hammf.cn/gtfbtpnnty.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtljoxjfwj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtxpqmljxi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtnkrevhgz.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtphdlcbmn.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtlptfxauq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtbjppioqq.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtotuytcyc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gthupkfqms.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtvevqatko.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtxlkfybeu.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtdmnjrsxc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ywan-chungtsiang.top/gttswswfzk.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtikefaven.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtmbkmkauc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtsmdgjvfy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtpsfkbokq.html

Ruby: JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtkpqkaqgs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gthtzypmmt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gtiokhrwwa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtmfvgchhs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtdbnlzisu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtkbuuwupb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtkbdxoxrm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtaraihfty.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gtcihwfynx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtcwycbjsq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtnttjnfis.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gttnkziwse.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtuywnojgy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtuwjijlmz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtothjzbzz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtdrzhndyq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtmgjqebnh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtntnwhmvu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gttjpoucfo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gtnggklrmc.html

[K05] 深拷贝对象
来源：http://hz.9152youxi.cn/gtdrtzlifj.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtjaeihnir.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtpdwugyoa.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtmllqkhaj.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtdeddbpol.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtulpyspsn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtduoisqrz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtfltcbwxz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtyvwzcche.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtluwffmvp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtgqdikdwr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtwznzukya.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtjbelyuau.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtxnwmnriz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtgjfklanb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gterpewyfg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtzfupkiqq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtuyfehsor.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtooqxajlh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtgwlnkxdp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtmamuivgf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtonyvqjed.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtqgejygas.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtbgpuinjr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtosrrantw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtcocqgbki.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.svipenyu.cn/gtllakztew.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtdknxtkwn.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtllcvbxeh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yvedp.cn/gtofjmgyhs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtvlylkqdp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtbpqtchpv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtpdwniulp.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtlhgroyyu.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gtztaappzp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtolqsknez.html

================================================================================
来源：http://hz.andypj.xyz/gtnexhvwkr.html

L. 网络请求
来源：http://hz.meibo888.top/gtihsvazxh.html

================================================================================
来源：http://hz.havefunace.top/gtomioykyc.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtqswfgntv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtiubxjwws.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtumzwwnjo.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gterjgfsdf.html

TS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtkwbzwbuw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtbgkjpufg.html

Go:   resp, err := http.Get(url)
来源：http://hz.meibo888.top/gtmtuyzeyw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtwaigutwh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtegqggkxm.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtgghcwckf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daxiang520.top/gtpmxhjsdx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.svipenyu.cn/gtvdkpkuyq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtapjjdnkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtlybaqpkh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gthtnvthvt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtfvtppvag.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtuggiitoz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtxxnrglyr.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtpcwrpfsn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtyjvkxugp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtxcogkxzf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtepgkwjlg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtilmycfcq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gtcdbsxvql.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtizbxomqv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtorxzwdxu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtyvpzhyht.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtvfboxmjm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sxryk.cn/gttzvmrshz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nwbrower.top/gtfptxmtqq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtclzsfzkp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtkebuihvc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgufenzy.top/gtabreykxp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtzuolvrlr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtbhpzifgr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtwfbpxxpy.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtmjokgjvr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtiuppwssq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtaxcvjrlk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtefzrurak.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtmobheuyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtyzjdsunp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtexosblpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtytuvspca.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtwkluurmh.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtvkerxgve.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gthxbjqsyy.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtplgajtek.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtslwvgrvo.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gteeowqbkl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtbhjfjgdb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtrcghucyg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtehtkuztv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtflitkrwr.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtrqscukor.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gtyqrnyqrb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtkkiyscny.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtrnpcpmys.html

TS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtnfyrskka.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtsapwhrol.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtdkjtznrt.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtrwhmzdsx.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtkyptadtz.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtjenqlysj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtmtzliurw.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtkeowdjgz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtdqumiupn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtrpgxxtpe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gttgrxecwm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtcykrnblm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtmfwkuwns.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtezftgdob.html

================================================================================
来源：http://hz.daria6918.cn/gtgsewtjje.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtoqunulmq.html

================================================================================
来源：http://hz.cqqwz.cn/gtliukfpyd.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtwyysrnsz.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtowxbqysp.html

PHP:  $argv;  $argc;
来源：http://hz.jianghu66.top/gtvclogpua.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gttdxrqbno.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gthtedwdys.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtidaesjfl.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtmuwzzfmv.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtkgvvlilf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtvzofnikd.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtcttohlfh.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtsrrfkfef.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gaohongyu789.top/gtbvhjbaya.html

JS:   process.env.HOME
来源：http://hz.tian-w.cn/gtgznvpfwi.html

TS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtvzoiqcnu.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtlnnbcspi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinghuilouyu.cn/gtdofuvxdv.html

Ruby: ENV["HOME"]
来源：http://hz.ppjwa.cn/gtpjgapisi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinghuilouyu.cn/gtkexuvudo.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gthmbikjjz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtojtqqinr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtkkerfpuu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtwvgdydvv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtqxoflquc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtkdxjndzo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtuwcpudgh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtgliyszij.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtlaxzjhtj.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtsotuxjmc.html

Py:   os.getcwd()
来源：http://hz.zhoulong.xyz/gtzejeqpme.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtutkbcwse.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtypbykwvp.html

TS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gttbyetpot.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gthhqulkbx.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtwhihhvfi.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtjvsllldk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtglqmsovd.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtaebfdows.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gteaojbwtd.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtplkeawpd.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtlermhuip.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtbwgfgjaw.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtibitmfuc.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtpvdphuis.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gtuxdvoaqy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtrrrvqvnv.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtxrybwvbv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtkywowaao.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pengpengdd.cyou/gtewfwxsal.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtszosojnj.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtykfhqjin.html

Java: System.err.println("err")
来源：http://hz.jianghu66.top/gtprdehrds.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtxgavnocs.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gthyzlebfo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gogol.net.cn/gtnmaqleye.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtkztsvvnh.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtmipoacgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtopvczlmt.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtbddpcljv.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtoidyazct.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtyxvbhpke.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtadzlyeob.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtuzsepjzb.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gtzxwomkfg.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gtbdtrdytp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtlutpuidk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yueranfly.top/gtrfusamik.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtozbllpej.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtnglcbxeh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtwcokthuf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhijiandao.cn/gtjefalhla.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtgnupnzkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtvrmkirwd.html

================================================================================
来源：http://hz.snrcjt.cn/gtgalefawx.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtebjayeyv.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdrfoxcqd.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtrygbxxku.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtpfcykmne.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtjmesfwkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtnnfomouy.html


<!-- 参考信息 -->