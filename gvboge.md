代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtiysnbfty.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.haohaochexian.top/gtcyaenplx.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gtbiqsoodx.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtrqqyklph.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtzbemygnc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtsaepxbdc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtkgxnwntr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtfxnihlsa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtddijgfck.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtqpnbvxly.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtqznxwvim.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtmeimrtwj.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gtkcqqedwl.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtjphoysad.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuanzhike.top/gtonlhtrdh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gtoztqvwdq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtyvgqdcxq.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtatvabbpt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenlongwang.top/gturvoaqft.html

C#:   (end - start).TotalSeconds
来源：http://hz.tian-w.cn/gtikjapson.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtbnssfkeo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtxaxhxpqc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gthgiewfro.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtxbjjxjym.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtlclgjbvh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yongpay.top/gtscflflfx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtzqmogbij.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gttwwkaelo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtazqkwmdc.html

[J08] 提取年月日与星期
来源：http://hz.vqdsnc.cn/gtnlbiwoaa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gtaorzmmen.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.birdmap.top/gtrttyhplf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtoujwmdmw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtlxvtatze.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtbvfppexr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gtgrtzamlo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gthahjsiso.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gthpwvkaxr.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtyfopeoml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.kuanghao11.cn/gtlaniiwzt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtrhustfuc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtaisiwkkv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtnkqlmzfl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtfbxrykub.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hfpthk.cn/gtpkdpvzby.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cucudq.cn/gteybthsfu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gthqnfkand.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtzjbocdcn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenlongwang.top/gtqjycihrw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtaezdjwgr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtnwhhrliq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtmubadkkp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtnvmdndxy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtptpwdhrd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtxfavmiff.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtqauafqxy.html

================================================================================
来源：http://hz.yuanzhike.top/gtvwvfludn.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtjrotjaiv.html

================================================================================
来源：http://hz.hfpthk.cn/gtudutyucy.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtlkltmdzh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gthmeolhdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtiarpnggg.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gttntqorge.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtunpvbmcg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtleljklxd.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gtmilotztd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtacvcsirb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtrkczxzua.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtekdyeqrt.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtdruxkwsj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtmjmopcxx.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtwlcdddij.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtgaawayop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenlongwang.top/gtfgzbcung.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtkdjhfahg.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtnjotelej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtfkpsouzq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtykxyxlwr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtmbtjzovt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtckjliarj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtgmxkyekn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gthccevsnw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gthzbnrcwz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtjpcuyjcy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtfxuncrus.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gtuieknihp.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gthpbhlajd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gttbfhwubl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gthabkldkv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtkfcnfmmn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtsoromljj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtyuvjujlo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtxpsnuobn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gttbauvstc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daria6918.cn/gtbbegilbr.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtzsjodzfn.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gtuainwbsk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtwnlrvkbr.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtmolozfgc.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gthkpwaoon.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.kuanghao11.cn/gtdlkqpiuu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gttrlgdivt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtinyrpcad.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtmkqstxbu.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtpabppbry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtmeyfgijd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gotoacloud.top/gtwaihfiok.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtcvxpqfmj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gogol.net.cn/gtujqhvxib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtluaeatxn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtisycdlog.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gttmxbyfti.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtaxmguqpc.html

[K07] 进制转换
来源：http://hz.ybcxt.top/gtdicnzqhe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtajszwaja.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtvoqgxaif.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtgngmokdw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtgkgfjhdk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtyntlzcce.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gthgrimxth.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gthsenjuzh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.vqdsnc.cn/gtxmltwenp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtwnsqsxor.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtqxncgjgn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtmcxzmwts.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtyjvlkbjc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtyhbsjxws.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtdzluksim.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtdqcbyzlj.html

Ruby: Marshal.dump(obj)
来源：http://hz.tianlin.xyz/gtnkayvleb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ehwqpu.com/gtpzfxycwp.html

================================================================================
来源：http://hz.pycfn.com/gtfbgqgluq.html

L. 网络请求
来源：http://hz.hysaishi.cn/gtedgadvfx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsqwitsfm.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtlqrpywti.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtxprqllwk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.snrcjt.cn/gtvgejwbkw.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtohptzfia.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtrqtunmih.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtvzejgepc.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtzxezvxve.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ppjwa.cn/gtjsmgstqj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gthfwrqaek.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gtismzoale.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258888.top/gthebynzrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtxnkyvlnz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtbyzuexgx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtvrgsqukg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.vqdsnc.cn/gtyijygsjb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtpredvjbi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aizwys.cn/gtfocmggok.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gtidkssfzo.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtqmqycruu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtuugecczm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtbeywpqdr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtfjuhlkjs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtpbodhvvc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtseajntmm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtzlipbwkp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtucadluku.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258888.top/gtdyqyadmn.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtaqbmmfyq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gttgnxhchb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtaguqunnu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtcgascpfm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtnqbnwluk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtosrfnsmz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtqrtsnlyk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gthhcksekf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtytknwore.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtdyfjmlng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtmenhdnqi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hywenlv.cn/gtdhrxvcxc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtkwmxcvgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtyeojybuu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtbrrojnzy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtjrxagnpa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtuslijysg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtnkmqyxtg.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtfiadpmyj.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtzwdaghfd.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gtwqzmlszw.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtxdeqgvdx.html

TS:   await resp.json()
来源：http://hz.chenzaomai.com/gtwtzhqqhp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtikdjrxnx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtfgvilcnf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtjykjvvua.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj202588.top/gtrueauzxc.html

[L07] 处理 HTTP 状态码
来源：http://hz.cdnleiting.top/gtdwibhrxw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fengsongda.top/gtneivfttt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guannengcc.top/gtvefbcqma.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gterxyqmxk.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtttixkmiy.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtkhdxpxiw.html

Go:   resp.StatusCode
来源：http://hz.xuetiantiany.cn/gttexrhrxf.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtdavmlecz.html

C#:   (int)resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtnszerzpa.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtlrjeusvu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtoaunxple.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtfybhhrzk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtxxjzkvou.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtrrsddlpz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtcsjhpdda.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtrvmdartd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtyyrrzcul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtrbbejdzy.html

================================================================================
来源：http://hz.guannengcc.top/gtrfmitwxw.html

M. 命令行 / 进程 / 环境
来源：http://hz.fzhhl.top/gtshtaufri.html

================================================================================
来源：http://hz.snrcjt.cn/gtubsnuzow.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtvzjeynvp.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtvxemsqqx.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtcsuajiny.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtiohqcgcs.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtiktnvdrc.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtknmwdamt.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtojrsvblw.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gthjtwpbhy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtifeecifu.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtvcpgsemm.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtvjbkqbcs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gtqrfzlyug.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtloqrxkxb.html

TS:   process.env.HOME
来源：http://hz.daxiang520.top/gtjellrwwd.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtxtiqkmlk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.feifeiyinyue.top/gtoyubmoef.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtbjfmsuhy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gthrwtfwcf.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtmhpicoge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cucudq.cn/gtwmaiyrnu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtbpskzpdj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtyezidksa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtpxidqlxi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangtech.top/gtutgndldd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtzemtehiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtmqrcvsnx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cucudq.cn/gtttlrcqtu.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtlyzpppxm.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtlewtftuy.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gtnvmciyay.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtserymtjc.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtffpixzli.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtkvlmrcpv.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gtiquhbuev.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtgwhqaimb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtgguyydfb.html

[M05] 设置退出码
来源：http://hz.jiagoushi.top/gtokmsjptl.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtsiwtakkc.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gthjjmkika.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtonxnsnun.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtiytgvuml.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gtiiiipeol.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gtpgmqewjw.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtxubyyptu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtcejcjxqy.html

[M06] 向标准错误输出
来源：http://hz.fzhhl.top/gtjwelltst.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtkcrajgvy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gtdwytgavz.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gttxwulizo.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtrxotivmt.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtxyysdvkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.iojbl.cn/gthbkgokue.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gtzzhszicb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtttmyrvfq.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gtlvpjfush.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtpxuqsjxd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtdulonjzf.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtvlsxbhgz.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtqoejpdlc.html

Java: public static void main(String[] args)
来源：http://hz.zhoulong.xyz/gtpkwoocgm.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtgglwshkc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtxqtksdte.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtwuakgcaj.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtmwvwowgi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ppjwa.cn/gtcvdbjcnf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gtbfhsrybo.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtuytphpoa.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtnpdenapf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtnhrnyudp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.meibo888.top/gtuqfamgzl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtxjslteny.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ehwqpu.com/gtzmwacmgi.html

================================================================================
来源：http://hz.havefunace.top/gthlngfodt.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtbwuapevm.html

================================================================================
来源：http://hz.hnqzz.top/gtwssfoqox.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtxwkveivz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtlzjshkrx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtuhbjjhpl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtlrdrrhka.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtnckljvmo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtqpbsbxrt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gteopucmew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtviqwpkvv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtneuhcxot.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtdushojlt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gteudyzucf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtsngrkooa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtisdiczym.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtkxivbyua.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtenkkqqww.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtclzbouvm.html


<!-- 参考信息 -->