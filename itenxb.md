代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtfkrdscuh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtlwnmylrv.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtrfuqbpgo.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtnogcclgj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtbucymnqo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtwekinssh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtjjxsjsdp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gthyxyzuat.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtwdecepre.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtoqgwgoiq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yangfankeji.com/gtquveqjpt.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gteuyngffc.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtvnzvimxb.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtbiajkmtj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtzdoprnxv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtxekbqanr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtgrdoaojl.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtquqwlyjm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gaohongyu789.top/gtcpyiqnow.html

C#:   (end - start).TotalSeconds
来源：http://hz.pengpengdd.cyou/gtwsmxltsk.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtpvsajxmy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gttbtcgsla.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtskruvgjg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtgfkeuxbt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtwqshuegs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtqvybxmhp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtywyattvh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtyctapelh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtfyohcfll.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtaspxiprr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtdoaiwjdh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gtjktwkgqi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtfteqdsvv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gthbblnedg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtxohmkfwy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtiynyrusg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtsbvtowmm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sysykeji.top/gtelebnfrd.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtufxsycsb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gtnhpvcggf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtkcfienls.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtvyxksmno.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtsniyqnva.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtmpyapwjc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xziqi.cn/gtcrhwrmvd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtbahjyoji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtddxnfemb.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtjpkpfowq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtlxubobcs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtphkhbhmg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtcgsfvbre.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtixdopkdh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gtxkcyvkkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtzgfrwrfo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gtojivrpfj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtaskgjdql.html

================================================================================
来源：http://hz.shuidangran.top/gtupwzmneg.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtmusvhsgy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtooxypqky.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtzchybgnm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtdfyyngqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtllgusjen.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtnahwsuuh.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtecloftzi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtumyjuifs.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtltiiocno.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtwnsfdxua.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtbjgzupsl.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtarcuxeqy.html

Py:   json.loads(s)
来源：http://hz.hnqzz.top/gtkzsdbsee.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtffsktvde.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtrjxopjdz.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtvktagsya.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtiujtowvz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtlwvaikih.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtgwgpgibb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtiypoujfa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtzubdcgbq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtrcecnwcs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtzazjxorf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtetwfpkoi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtkmjhwbsp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtxcfdogwt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shangyingyoupin.top/gtzrovxedw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuxming.cn/gtqjxauszr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtyrybgnqu.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtqxvximbm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gtqbsvolkw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtmqkaxdfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gthdmbekum.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtxsarzyje.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtmoiwweli.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtoqtegsvr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtekzkcnsl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gtydssvwtb.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtvwxxjips.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtsqvejuos.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtscaphhyu.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtqrldxxhs.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtpmnsflep.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtwpqtmeay.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtgrdhiyog.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigufen.top/gtkptdsnuw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtfxpecsob.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtvjoqsaoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gteriszoqr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtdqvgqlrn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtgxvfgzky.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gthvuuqass.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtkjdvdljp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtcedingzg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gttzzfcgjq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gthxfchdkd.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtfokdbivs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtvpbtqvkc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtrjtjvwbk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtfwzspgua.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtljklrppc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtfsmoztld.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtripedozy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtczqrarzo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtkhuyrgtl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtnewycwzr.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtmngkoblz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ywan-chungtsiang.top/gtfjmytbbg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtfwyhwovw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtoszsgigq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtfgtadfly.html

Go:   encoding/gob
来源：http://hz.redwolf501.top/gtphijzqxg.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gtqddoigyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtclauryrg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtroxyegxh.html

L. 网络请求
来源：http://hz.xuanzx.com/gtsrscqmic.html

================================================================================
来源：http://hz.tian-w.cn/gtpcqintjy.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gthrvoasao.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtywnykxqv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.birdmap.top/gtxbcbhhqr.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gthkocjmmg.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtvdcobjaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtkcpxumgb.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtcwgmqaih.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gthknqqylk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangdashe.top/gtcymtjylk.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gthyjczuxx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtcrzrdkln.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jlsjyb.cn/gtnmjwvhsc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtshipjemh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtzuofltqm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gttkdobwhv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtvdomfwci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtfqfumgoy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtfgtdkstj.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtkrwhzlhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.9152youxi.cn/gtrmwlftuj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtlmstawle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtwsxqtdps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtkubbcrpo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtgorucqhv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtmunvtfgq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtqrgjikci.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtdgtbqtvz.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtislefnhp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtjgspzaya.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtqzbdkmdf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gteiufzuud.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtcppjhesx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gttelltvrl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtwzrofiic.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtknvjycdd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtjcgdwbcp.html

[L05] 上传文件（multipart）
来源：http://hz.sufxvd.cn/gtlgamownr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtychtezhe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxuanxn.top/gthjpgvvza.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtssihdurs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtdrmotfer.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtlisjmxjf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtxeqtrjva.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtcorsolae.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtxkungnpo.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtpsdqbqkn.html

Py:   resp.json()
来源：http://hz.ydzc1.top/gtjcgulnad.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtgtjkewig.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtygchiece.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtrpjdwxck.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtlhbeospq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yvedp.cn/gtntjmjbbq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gtjcmlmkas.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sysykeji.top/gtfgouoqzm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtxfdkctxt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ybcxt.top/gtgohqjkps.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtxbxljmuu.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtusduhqaq.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtgqvbncqb.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gthffysfwg.html

Go:   resp.StatusCode
来源：http://hz.cdnleiting.top/gtbhflsuip.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtnvvstpll.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtivrkdbrp.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtyhlxatxf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtzhltbxxa.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtokseuqdc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtgfznqxyg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtxzwngquf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.mhx1999.top/gtkjqndhgg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtxlqurrda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.mhx1999.top/gtvwizxwzh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtdzaiosng.html

================================================================================
来源：http://hz.zycfv.cn/gtrabshtzl.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigfzy.top/gtbxwernve.html

================================================================================
来源：http://hz.haohaochexian.top/gteidmdlhr.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtalcsrhmb.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtflfxorsc.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gthvgmkmiw.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtrjptgpsx.html

TS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtmgfstbnn.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtjriyqqyt.html

Go:   os.Args[1:]
来源：http://hz.xylfe.cn/gtaadlgjvc.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtsxfroxza.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gthxtajejw.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtczrnmohc.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtkgupymmc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtanibcmau.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtdkafdkvc.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtsknxskrq.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtfbtyihcq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gtgxopinjv.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtwhhwcglu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtglhlxqvg.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtaypzsfiy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtiebanefr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtuokafnmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtpvswwjhm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtiupoxchn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtifsgvash.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtmcqcqcyk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gthqajvomw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtxjkrbyeh.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gthsczyctb.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtgfwzhjdj.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtdyhvtrdl.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtztdyeleb.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gttkpyzgrm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shuidangran.top/gtgpjjapnh.html

Go:   os.Getwd()
来源：http://hz.gzhubu.top/gtcvfwbkte.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtniqsmmul.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtzbmonhlk.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gtqoehehlm.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtpbztmwba.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtjkgggbzn.html

JS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtxmftdkqp.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtlghkjucy.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtkjdlwtuu.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtzvpubctv.html

Ruby: exit 1
来源：http://hz.zhaomingkeji.xyz/gtdahlrwdm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtmddrrfhp.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtsyivzsvs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtdtipgkce.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtxemzxwyo.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtqkmvobls.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gttggikeuj.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtsewltjlp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtfqxvbqkr.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gtzlahabab.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtgpdzqkyt.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtdgcpttgp.html

Py:   if __name__ == "__main__":
来源：http://hz.ppjwa.cn/gtjxprywwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhoulong.xyz/gtowomksqu.html

JS:   require.main === module
来源：http://hz.daxiang520.top/gtfplpnhpz.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtzjtabrrw.html

Java: public static void main(String[] args)
来源：http://hz.zhiwuduotai.top/gtohfdoghb.html

Go:   func main()
来源：http://hz.yueranfly.top/gtqzhixwrg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtcavbgamh.html

C#:   static void Main(string[] args)
来源：http://hz.yongpay.top/gtgmkxwvbo.html

[M08] 获取系统与运行时信息
来源：http://hz.cqqwz.cn/gtesoquhcj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtoayegzzw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhijiandao.cn/gtjhcmcidx.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtyuksfhin.html

TS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtajorrkgo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtozvmeaic.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtnlzlyduz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtfunhfved.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sweek.top/gtqovaduzj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsoexazpl.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gtkrxfepwh.html

================================================================================
来源：http://hz.jianghu66.top/gtjrmvlibk.html

[N01] 二分查找（有序数组）
来源：http://hz.daxiang520.top/gttcyxftyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gttsfpxssr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtfibotwqj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtxiktkjbr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtnnrplxje.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yongpay.top/gtzrqmooqi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtjcxbfmts.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ppjwa.cn/gtyfksttel.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtkyqmgnht.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtmlgshjga.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtvnxrzsbb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtwdmimlea.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtrvekslmi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtzfymlsxz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtdssxfsxc.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtelraoofz.html


<!-- 参考信息 -->