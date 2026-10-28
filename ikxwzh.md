代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuxming.cn/gtljojcqsu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtpaqwmpnl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtikfzjyon.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtxrragilm.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtmclhvzsj.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtdmlhrswj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gthkdquuay.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtkjlhjpfp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtosqaroky.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtxobobhle.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtiyoixkgw.html

C#:   (end - start).TotalSeconds
来源：http://hz.zycfv.cn/gtznsmlxsv.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtqaxqdgsz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtpoqrqbbb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtdykpwxke.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtasynswhr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtrhmfskiz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtnsclgxnm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtaqkobqkn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gteolwgtlv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtvjmllkuk.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtrpzjhmyo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuanzx.com/gtizpwoxhn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtcpjczuma.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtafjcfbmm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtqimcfzsn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gttklzvljr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtrpmttubd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtlisogotz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtlvwbvtfh.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtovtaraet.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gtczqfxpzq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtusarziic.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtelanggjm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtiqbmojcp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtxwihggum.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtuzrwsxue.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtkkjjydgi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtwumgoqwx.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gticuuouli.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtuvdsvwpl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtosoixeqk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gtqnrfiifw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jiagoushi.top/gttlvpbkhd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtgignwjcl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xylfe.cn/gtrlbkagog.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gtkykchawe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtpghisoxa.html

================================================================================
来源：http://hz.ydzc1.top/gtusotxzby.html

K. JSON 与序列化
来源：http://hz.redwolf501.top/gtlkqfgbeb.html

================================================================================
来源：http://hz.ivvv.top/gtyppklzvd.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtpcgsjsum.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtzxlrgskj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtlfffksjf.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtrnalswdm.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtvckimpxj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtxdbqtnel.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtfksjzndm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtqultkeca.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtvativcij.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtektyxkgb.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtwmtueqgh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtkgcreyxd.html

JS:   JSON.parse(s)
来源：http://hz.sweek.top/gtmgqiuepg.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtihwlkbvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtnokwmurk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtkvvmrlvi.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtdnfbkult.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtdgxknmai.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtcsvzwrgo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtyqthnysf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtnubdycpe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtykzwnova.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtslaztpzu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtlccmgumi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtesiyquqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xylfe.cn/gtprncftcr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtfzfqlygp.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gttjzrymgy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtlulhkgzg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gthenohhfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtfjgitfpd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtsmdwpuyx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtabahossc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtjukfdeww.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtpfpyzaqa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtqskwrqlh.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtnutvdyrm.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtqwjqwlna.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gtxjvcfjxy.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtvzliquoz.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtvncfkdjc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gzhubu.top/gtoqmhrctq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtwhwaxqrf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtfthrjwcr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtpnswllit.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtshitppbe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtzlyxbkyu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtapapuoyo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtvmdeplsz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtitgnuucl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtggmfqdar.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtmninbfem.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtfzhrfcjz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtsrgwszwu.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtphjjruwh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtntajpeod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtmahzncrv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtydbcnhpw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtwxpqjpdc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yongpay.top/gtdaoqtuil.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shzxlz.cn/gtiatktktz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtzhzeshfh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtinhwkhae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtqpslbsdr.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtvzshizku.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuxming.cn/gtlwkqikwt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtzjtbtpkv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtnuuselky.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhaomingkeji.xyz/gtfdrubtzs.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtpuulirmp.html

Ruby: Marshal.dump(obj)
来源：http://hz.zycfv.cn/gtntdaaibd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xylfe.cn/gtgghobhqv.html

================================================================================
来源：http://hz.ppjwa.cn/gtohxqplsu.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtzlpaseny.html

================================================================================
来源：http://hz.zdqjudy.top/gtoylqmgcn.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gttudqwtzm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtmyrmeoob.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtuzeiwngx.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtkxyypjje.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtfqkprdze.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gthfrfnqbi.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtmuiutkkx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtnxzsmkox.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtykczgxus.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtacsluhqr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gttyyauywb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtwzvhxzlk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtzhwnjvqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtlkkolbyf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aibaodan.cn/gtrjlirckv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtuftvbmlo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtoplxpoeg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtwlfwlieo.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtjvgkobjm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtcvdjduzu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtejkmqlqf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gttzyzesyc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtkpcgdoib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtyeuvbizc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xziqi.cn/gtyrsygkqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtezmimlzl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtnvqthcnl.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtdcglqlgj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtpsvulfgp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtotmjiejl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtgbdxpspv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtpbxruwky.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtmxvpgtit.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gttwcduiqi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtskzomjia.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.smart0.xyz/gtjsamttgk.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtcrbyxawo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtwvfgkauk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuxming.cn/gtnvvkcslj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtheoqgcdm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtryqjqjmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yueranfly.top/gtrymoihxd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtgvhmjbtd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtkyttpkar.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtywflumvn.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtgnjslauu.html

Py:   resp.json()
来源：http://hz.ppjwa.cn/gtwbmdzscf.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtilocenqs.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gtzndsfliz.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtabrzvpwd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtimwcsssp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenjidiqi.icu/gtqnszoszn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtnroyvbpt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhengqikj.top/gttrmsrtxm.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtzkzakuwr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtonsqpece.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtstmftspe.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtssgpexlg.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtzbpjkeql.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtgwygxapu.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtidlxgkqp.html

Ruby: resp.code.to_i
来源：http://hz.iojbl.cn/gtgtsgkeax.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtmdtpnoxc.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtceqrbcqc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtxmrfgvcy.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtqobsinri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtpbydqalu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtvtwnscpl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhixingplan.top/gttsedtnwh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jiagoushi.top/gtsngaeinw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtjizooprr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtcxplfzye.html

================================================================================
来源：http://hz.ivvv.top/gtxmxratuy.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuxming.cn/gttirjbqie.html

================================================================================
来源：http://hz.aizwys.cn/gtjcbqlzuw.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtrvigtkbg.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtjqfjikit.html

PHP:  $argv;  $argc;
来源：http://hz.gaohongyu789.top/gtuvkcaxtc.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtsdchzcpu.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtcbifurxj.html

Java: args 数组（main 方法参数）
来源：http://hz.chenlongwang.top/gttvaeaawz.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtxetjfstn.html

Ruby: ARGV
来源：http://hz.snrcjt.cn/gthpgrcwlh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.havefunace.top/gtmunmjntx.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtvhioqjse.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtqbdlnmpy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuanzx.com/gteijbzkzq.html

JS:   process.env.HOME
来源：http://hz.guannengcc.top/gtwsnosktu.html

TS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtjuisppby.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtlwksipub.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gtzpifpzdz.html

Ruby: ENV["HOME"]
来源：http://hz.andypj.xyz/gtrddmbjwc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtlbytkywc.html

[M03] 执行外部命令
来源：http://hz.tian-w.cn/gttztbgiat.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ivvv.top/gtgpdjbxax.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtkbcmnith.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtnbosmcvi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtjhvanopp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gtaawjnmjb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtkfvrbvvy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtqajyhgnd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtkeapvcfq.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gtmzcpjner.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtywvqcqzs.html

PHP:  getcwd();
来源：http://hz.daxiang520.top/gtaplxjyak.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtpfhsazlr.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtidlcyzmp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gtabqbtvme.html

Go:   os.Getwd()
来源：http://hz.meibo888.top/gtrnrflofw.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gttwybjzwo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gthdptayhf.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtuwbncucg.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtwfzopjug.html

PHP:  exit(1);
来源：http://hz.quarkkingdee.top/gtccaabwoj.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtqhiwmayd.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtymxignxk.html

Java: System.exit(1)
来源：http://hz.smart0.xyz/gtyjkaoseu.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtsmqsujxt.html

Ruby: exit 1
来源：http://hz.wangshuangyany.cn/gtbayyzpdu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gthklkclqv.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtawtrqxxe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtoiheselu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtfiwsjssd.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtmqxybbwa.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtyzeeylqt.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtbqrkwbpz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtazuljxhr.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtithsmyug.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guowangkeji.top/gtpmrudefc.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gttsqvxqwn.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtmbkftiuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtkabdizne.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtufbieotb.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtkgwemaoo.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtkzzkyozc.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtdymhyeew.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtaqszazro.html

C#:   static void Main(string[] args)
来源：http://hz.nanxinkj.top/gtpxomxaxk.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtjpfgukpj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gtvzbrfqzs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtnxgxbajx.html

JS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtogremypy.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtooeucxgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhixingplan.top/gtqkdtbpgz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtcgcfqzld.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtpmoobrrf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtrwxkmgxj.html

================================================================================
来源：http://hz.tanke756.top/gtvaxtiyoh.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtmfkyscob.html

================================================================================
来源：http://hz.tianlin.xyz/gtevzymrka.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtjhybsgha.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtgrsvjfie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtydxkzaqh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtxvoaiull.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtrjobbpuz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtjggeavlv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daria6918.cn/gtigztmscf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtkshhutfo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtxtmcnqnd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtwubokjpb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtpopgohbk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuetiantiany.cn/gtvmqzbvmy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtpxewlpmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gthugsbwpc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gtfvvewgac.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtjhzjbttr.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtphbtbanq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtuushgjyc.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtnjufssso.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtwpepbynp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtriwhxhzx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtdwvcoqmp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtbvmptspr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtoazolakn.html


<!-- 参考信息 -->