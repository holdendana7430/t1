代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gtlksravwx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtyqcxfrrp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtnehgmiof.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gtosemimmt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtutonslvl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtryvnlkcn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yangfankeji.com/gtzsenwbks.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gtnjuelreu.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtzxyewcxq.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtkwzmnqhg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtlyatigak.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtkmvkmtuw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fengsongda.top/gtodtqbtzp.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtbmvydfkr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtvlvejffq.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtfisjsbgs.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gtgjixpaoa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtwcpkloju.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtmvmnltsv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtwoouuvhu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtjnkxtqag.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtrbmhvhbm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtjsyspyfa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtuuazhjdn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtpmodserp.html

[J08] 提取年月日与星期
来源：http://hz.ydjk.org.cn/gtjvrvmidb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtyfnumjib.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sysykeji.top/gtpqvliizs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtqfadcozg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtcfbabjxi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gtcqbqfylw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtlvkgxkzd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtshgpdbmp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtgwvokadb.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtovvfhzzm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtanfcqlqn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gtpcjpyowb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gthnabdxbn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtehyiaeho.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtgvvzppix.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtyxcrabgn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gteoslzdhf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtosmryvst.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtiuooygei.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtrphqutiu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gtatjtiude.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sxryk.cn/gtqxlwvqdj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangshuangyany.cn/gtwktavmlo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gthjckhmas.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gteigkrrkv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtzjqmrtpg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhengqikj.top/gtatyaqsfr.html

================================================================================
来源：http://hz.ivvv.top/gtjwzxzhul.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtddmllcey.html

================================================================================
来源：http://hz.zhixingplan.top/gtnujdyrpa.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gthxrkarmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtoajfanvp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtlzbmrnxx.html

JS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtijhkqods.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtdlusldne.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gaohongyu789.top/gtgoclpyqs.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtykhgessp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ywan-chungtsiang.top/gtrrusyrqs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtadgjxxlh.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gtuxcmfmpz.html

Py:   json.loads(s)
来源：http://hz.zhongyouzk.top/gtpbyspazl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jiagoushi.top/gtxffrbqnu.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtlkqzytjb.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtxjrcqaau.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtzuoauars.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtnpxjjvwk.html

Ruby: JSON.parse(s)
来源：http://hz.zdqjudy.top/gtfatzathn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtyizwgger.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtxttvhvja.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtodweeglq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtnzomrcmb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtzvifzqbf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtzgtalagn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxuanxn.top/gtzfwdfikb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtazaipliz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtaoqmshfj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yanxiufei.cn/gtsntdhplq.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtxniingjm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtmumvfnta.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guowangkeji.top/gtqsylthuc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtihoakzwi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtobdnexze.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtolrveoki.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtspwblosk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daria6918.cn/gtnqmybzzw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtxrwlimhz.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtfvtzmqwt.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtkjecfqap.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtngjoacdu.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtlyoqwghv.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtywhqxcfd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtqzahctuf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtypttukyv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtraqvybef.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtaqveipgj.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gtlvfvqvmz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtczxwovba.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtobrjnpwq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtcmhqblkp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtytcehona.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gthiqqzfzu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtedsgjmtq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuanzhike.top/gteylxtlvk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.9152youxi.cn/gtnmwmcfob.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gthuladfjt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtsoqilmwz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtyzheuxzv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtpjnkmnjp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gttyoicfbq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtbrxfbsej.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhongyouzk.top/gtjestorvf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtrumaszbq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtkryjebnk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtsrrprmid.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtxsonlpwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gthyzvqamq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtjsvouhfp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtmxsgopzw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtepptmpsl.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtwtihfptw.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtnkvtfdbm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guannengcc.top/gtomsihsoe.html

================================================================================
来源：http://hz.yuxming.cn/gtgylqybgc.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtbpxmruno.html

================================================================================
来源：http://hz.hysaishi.cn/gtjcpdyhdt.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtvjjbjdqo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtruujjwpa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtlchrryig.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtcmovoigt.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtzbnsvrbd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtvkudlnos.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtqgimonnm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gzhubu.top/gtdngaurca.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtsmkznaqe.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtxkyvmrcx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtfvtklvbd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtraaqlibv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtrutaugyx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtzkrpitzi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtovicousv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtznwlzeeq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtrrxvrzcc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtcrmwuali.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtydhjrpsf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtppybrlkz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtbidtzcnh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gthvorzbmy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtolwqyjtt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtbamdncwk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtaoqjoczg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.316326.xyz/gtclvnzdip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtrsdvuvvs.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtazvxtjoo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtufqtesud.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtmnoxmojl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gteziyzwlx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtnyxaxwud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtflpuuikc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gtakfjqlft.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtwxumknsm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yanxiufei.cn/gtmplpsdad.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtzyhnvmsv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtuufyzrro.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtyibpqjlb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtcqwcizzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gthlrkoses.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtwlcocxbv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtzuohonhd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.kuanghao11.cn/gtrxjfnduk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtmudjaekl.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gttsgcbhnb.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtdurgjnbp.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtkrdlisdu.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtfmbugaim.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gttvtxelhk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtkatvsifi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gthdhzkgoz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtdfjhofki.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtrsfuvpws.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtkanwiawl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gtcnyoxoar.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtzryqwhca.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtdliplcka.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtijzvdccw.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtzlowlrjq.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtrkoqrhhh.html

Ruby: resp.code.to_i
来源：http://hz.yueranfly.top/gticilhfka.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtaqtlviva.html

[L08] 并发请求多个地址
来源：http://hz.yueranfly.top/gthhxxteli.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtsrrqkxic.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gthzkeawvo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtxolbiiri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtkrnoeobp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gttmhnibgr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtbhkfiwsi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gtqsehnojf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtbcunzvkd.html

================================================================================
来源：http://hz.cashguo.top/gtunyhuxdx.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtplltzqxz.html

================================================================================
来源：http://hz.9152youxi.cn/gtuwktcqlj.html

[M01] 读取命令行参数
来源：http://hz.zhiwuduotai.top/gtbnvljyis.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtsdvwbjyb.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtrnfymcdl.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtyzkrhans.html

TS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtmghknufi.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtapbyxamy.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtbehkbvio.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtxgudwgrr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtvfmvuwgk.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtrypmhkpq.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtvqajdzof.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.9152youxi.cn/gtznflzlnk.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gttdtjnupk.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtqsqzpwwt.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtzevfaeft.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtrfaklabo.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtbglwvhqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gthtarsyow.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtuwagvjjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhiwuduotai.top/gtyejchnzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtbfzjvkcq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtzgdgdopo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtbuafrwrd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtbsbfumcv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtxczginap.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtimprqrmv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.havefunace.top/gtjestdzwg.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gtaxzrsuhd.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtnswvlykt.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtqbculhkl.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtgpylztps.html

TS:   process.cwd()
来源：http://hz.aizwys.cn/gtcfxszlss.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtbfytvglf.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtvwwnxyvi.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtctfpcuht.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258.top/gtjjkwusvz.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtiwqtqcqd.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtvuctlzuk.html

PHP:  exit(1);
来源：http://hz.shanyushiyangkeji.top/gtogupbuot.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtibydcxgm.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtefbdpevp.html

Java: System.exit(1)
来源：http://hz.316326.xyz/gtqhnexyit.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtrasobxcq.html

Ruby: exit 1
来源：http://hz.ppjwa.cn/gtspnssbhx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gtacxrxhrn.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gtfatstigh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtqiuztwyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnxiangtu.top/gtrnnygovb.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtkzbsubww.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtfguwwwfk.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtisjnwmue.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtwuugocot.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtjaqzfyob.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtrhxtxjjs.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gtmoqwehxb.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtpcmetcpf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gttmmjadao.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtkwowptnw.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtkfbqhcbl.html

Java: public static void main(String[] args)
来源：http://hz.9152youxi.cn/gtljbdmguh.html

Go:   func main()
来源：http://hz.chenzaomai.com/gtziwjjzcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtreuawaxp.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtksozefud.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtkcmslsig.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtyakdizyx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtgdhbvzbs.html

JS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtodszxuvf.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtwviwknfd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnxiangtu.top/gtbcmzpcai.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtkkxgczwp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cheryme.top/gtxxxwmocl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtlfpwaxhk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtobgyzeam.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtarnuoymd.html

================================================================================
来源：http://hz.nanxinkj.top/gtnouyvijk.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtwxmbwfkc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtyiiklmwi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hysaishi.cn/gtluctuwpx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtteurgukn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtwuhqkxib.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtnnumvkcx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtcggvnsbu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtpvcqjoko.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gtynwjmths.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangtech.top/gtujvnenix.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gttronobki.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gthowpydzd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtzseggnks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtcwmqyjph.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgufenzy.top/gtyuivnoda.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtbczoedop.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtkmpqdwbg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtnrytmqqx.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtqthnrgwr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtacpqcmzx.html


<!-- 参考信息 -->