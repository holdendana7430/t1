代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtruopcyck.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtzpxrgrvs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnxiangtu.top/gtiuemqskx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtgpdxghpu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtnlivdmou.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtvcprbhbl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gttmosgnpf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hfpthk.cn/gtdkggqdso.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtrpmmczjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtpcokotys.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.svipenyu.cn/gttrsfqnci.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.birdmap.top/gtgbeptdeu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtaivcwjaw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtuvcrgyjw.html

[J05] 时间加减（加 7 天）
来源：http://hz.yueranfly.top/gtqpvapkca.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtlrvpjren.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtgmnjqghw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtlqunkwmg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtjykoiobo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtlodiwlam.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jiagoushi.top/gtkzqxytcm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dianchejie.cn/gtbnnytrrr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtkauogzld.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtbdxdfycs.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtqtmfhebd.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtoukvlewz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtltdbfbdw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtawfgvprm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtisruskgx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtsobmcwkd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtdhoerdew.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtvxbzgylb.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtsjffjzxl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtytnsitak.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hfpthk.cn/gtlbnfrjjb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtsnazwdpi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gthwvfzdue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhixingplan.top/gtlthpkvmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtwjzzsjgk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gteqberopj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtrnjmzgnc.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtpvpnefth.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtmyjrdetk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gttriftxvb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xingfuxueyuan.xyz/gttftpidpe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtufxpowsx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtvmydzvea.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtxkmcagjg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gttjgrsque.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gttcvhvnqg.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtmsnlqrux.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtcgwbuuys.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnxiangtu.top/gtvkrprwbv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtrnfvjokz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtjgmypvko.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtchujoukj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtfcsbrnls.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.316326.xyz/gtnmyemcaf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gaohongyu789.top/gtdsewwphs.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhoulong.xyz/gtptpdllgg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtydratxwo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.feifeiyinyue.top/gteuwaitjj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtxlyqaxla.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.feifeiyinyue.top/gttujfibjs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtevfpditk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtfduklvbt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtomejjlcd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ybcxt.top/gtjdlkqkgr.html

================================================================================
来源：http://hz.fengsongda.top/gttnmfwgot.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtjgcyfdwf.html

================================================================================
来源：http://hz.gogol.net.cn/gtoymdmekj.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtgatnwxpk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtdcbpdddq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtotsjpnjt.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtgbdkbzbr.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtxqexulpt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gteritofdz.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtdnnvnlhv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtmrpugway.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtidgojgof.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gtmgnmueex.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtghovvxcb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gttwmvgdep.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtzkhgrxgv.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtvtxkxqhs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtvljpmlkm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtbacvflyo.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtvfsvocxx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtdrhqmjfl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenjidiqi.icu/gtjxymlqkp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtpmhicbvw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtfhkkqfoc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtaufodnke.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gthwdwlufz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gthakuewzo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtxzukwwwk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtdibpuzgt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtofwwxdjt.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtoxqadeks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtwullwdya.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtyhpbpvzp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtamknqidd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtsppyyswf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtefvdazjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtehgpjacz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtvorrwpxm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtemeellop.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gtnigpeepg.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtforfwcrh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gttlbxlvmf.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gttecfcqjw.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtavxwkcyz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtkzxdumxm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtcmzbnola.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtoikbhfsg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtkktxpecu.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtjsihmzyd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yvedp.cn/gtfqjnmtsv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtdlxjnfsw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtmomzmdfw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtxenybgui.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cucudq.cn/gtldnqnejp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.316326.xyz/gtnmcqujie.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xylfe.cn/gtwlvppvsy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.birdmap.top/gtpahmffbi.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtpzgznpkc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtatdsoqiv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtbkxzghby.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtcckzirlg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtbmhyplhd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gthyluhupy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtxctkbtji.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtjlgfmliv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtavmghqew.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gthadxvwxl.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtmvzotiug.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxinkj.top/gtymccuchk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtozzqvcne.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtorvxujqa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtyazlymxs.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtgnyrvkwj.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtfmkdaqmt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtyfplhsgn.html

================================================================================
来源：http://hz.nanxinkj.top/gtunmhhgkq.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtholujlgs.html

================================================================================
来源：http://hz.ybcxt.top/gtptcpjsel.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtlvjnlocc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtpogmzrya.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtiwxwnnwu.html

JS:   await fetch(url)
来源：http://hz.guannengcc.top/gtupyzfbnf.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gttmrrrmqa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gtcfskdnkr.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtpgcxqldp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtieuezhru.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtuqmuhfbr.html

[L02] 发送 POST JSON
来源：http://hz.yongpay.top/gtpusrrvrd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jlsjyb.cn/gtqkzjczzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gtyaygzckt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtczxaitgd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtnhnrnopz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtbrmfrutv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtmxsgixlo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtxydoeqad.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nwbrower.top/gtctdmrriz.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtolccflhm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtayasspxn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtyvllxdhq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtgfbveahf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtiuwchagr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtgbhibbtp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtziuptqgw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gttedkauqe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtimdkxaxy.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtuqlxqzop.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtgjqrvgrk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtzkkuhdqc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtberyuqlw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtgdpofvko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtmfyrdiog.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gttdbgslka.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtigvtdnar.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daxiang520.top/gtzquzliae.html

[L05] 上传文件（multipart）
来源：http://hz.feifeiyinyue.top/gtiiamqwfg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtawuiawhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtdwxqpzsx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtedpoqepq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtocgrkboj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtuzqjgleq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtqqscqwtx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cdnleiting.top/gtpvshtswg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtkxtqjoct.html

[L06] 解析响应为 JSON
来源：http://hz.jinghuilouyu.cn/gtxwkopgdk.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtuteozyay.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gttikotnrd.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtcfdksvsn.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gtlsdtipzs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtotgvdalt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhijiandao.cn/gtwrnvrykt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtmxvmlira.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtcrdhatla.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtuzandnxy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gtczfxucic.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gteduoldwm.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtxrqhfupm.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtsohjmdgq.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtqpjfpxpf.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtmdhqlaxm.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtwxkibvtz.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtnvylctju.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtygdzrrdx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtxlkbzumk.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtltvkasbl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtebdropfg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtllkuklza.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shuidangran.top/gtnhfnnasb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtskqovykp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aizwys.cn/gtajozbmvy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtkhpwhybo.html

================================================================================
来源：http://hz.0kj1m.cn/gteluzpvoa.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtjeridzze.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsgbcbzmx.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtgidsnrwz.html

Py:   sys.argv[1:]
来源：http://hz.hywenlv.cn/gticupzxrl.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtnjfcpktz.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gthjxygpkn.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtwvsbzdqi.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtiwjhwrht.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtlsspthjw.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtptaemjpz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtkyrinpww.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtdujypeqb.html

Py:   os.environ.get("HOME")
来源：http://hz.yuxming.cn/gtspwozhgd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtiliqcbaf.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtacoprlos.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtbaibcunp.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtsputwqeb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtmboydmjv.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gtmjjqfgty.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtpoaultwn.html

[M03] 执行外部命令
来源：http://hz.redwolf501.top/gtrmdxhxvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxinkj.top/gtmfrsuuhw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gogol.net.cn/gtghqmlzkw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtnsnfzryn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtagcghafv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtuwgpdkju.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhoulong.xyz/gtugncomlg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtmcxkdgni.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yonumen.top/gtbhjgjphn.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gtblixysgy.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gtkffyywko.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtvwjekbao.html

JS:   process.cwd()
来源：http://hz.hnqzz.top/gtggoovjlp.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gthztyscua.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtyvdbbwnc.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtollnxcgb.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtwqptroew.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtoiovainy.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtiojpymis.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtwguokhvb.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtobtzhxdx.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtyqgungqu.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtrwlbzdtw.html

Java: System.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtlmojbghn.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtozqeilpp.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtciixyvfj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtgjaalpzp.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gttypffhkd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtopqqgmnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.iojbl.cn/gtpyzbxfse.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtzexpaqir.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtefclezkz.html

Java: System.err.println("err")
来源：http://hz.zhoulong.xyz/gtuygbpfca.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtxnltctko.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtnvmzoagl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenjidiqi.icu/gtgnqupboj.html

[M07] 判断是否为主入口
来源：http://hz.c1oappe.top/gtuyxqwkac.html

Py:   if __name__ == "__main__":
来源：http://hz.hongshengwenyu.top/gtuyzrqcin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sufxvd.cn/gtjnqflbto.html

JS:   require.main === module
来源：http://hz.xinyue.icu/gtefagxalt.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtixlgcdtx.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtbyqyuwbr.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtjmwppwkz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtnjpejunk.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtcpkqpptf.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtmgrpzbac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gttjakiigi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuetiantiany.cn/gtmdhulhem.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtguejttdq.html

TS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gttrhdhnqo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hfpthk.cn/gtnajqoddj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtdhncrtdc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtpposolaq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtmyfwssfa.html

================================================================================
来源：http://hz.meibo888.top/gtwwyjwthk.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtvpvpffwz.html

================================================================================
来源：http://hz.zhixingplan.top/gtwzfpfuek.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtkjgmjxgu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtnzwfhysn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.snrcjt.cn/gtdjgooexs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gthorvrbef.html


<!-- 参考信息 -->