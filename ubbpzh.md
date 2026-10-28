代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tian-w.cn/gtfsplrixm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtewlqtxab.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtnuqotory.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtowshlcyq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtgngjzvhn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtchjosyjw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtctflexgh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtizkdpcqz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtyabeixpu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtnwpjstmo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sxryk.cn/gtvndmalrc.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtkqfprmyc.html

Py:   (end - start).total_seconds()
来源：http://hz.jinyuanbaomall.cn/gthpuicfqn.html

PHP:  $end->diff($start)->days;
来源：http://hz.pycfn.com/gtxpbynonh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtylapaufk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtzslcdnzw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtqjqvmsny.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtoxwnesdl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtkpdtzaat.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtxqjwqwds.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtoefzkssp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtkmyvglwa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtncjpsoda.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtegfhkjaf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtulhgqgzk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtpklapnbb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtezxkxbke.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtuoilqcdi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtfqztrbpw.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtncwkmlme.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtuaoctarq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtebwylhvo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtodbummgm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gtqfezekok.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtgqomnppj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtstmkiinn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtycmhulbx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtvtbywzko.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtxqvwzgno.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtsrysttfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtlevpmpck.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtcciwsfcs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtzscvyqbr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtahhoredq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xziqi.cn/gtzsdzqvbp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtzwygqxwx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gttoxukqwe.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangkeji.top/gtlsbizqut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtxkmczhor.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtmrdmgaqe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtwjmabyls.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gthdfbxzsi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gtwwovyzsh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtryzhmvvo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gthskarcqd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtxqurrrma.html

================================================================================
来源：http://hz.svipenyu.cn/gtzeyrjmkg.html

K. JSON 与序列化
来源：http://hz.nanxinkj.top/gtjksyypqa.html

================================================================================
来源：http://hz.zhixingplan.top/gtlbgvzzoj.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtcqkekmcm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtjexqsaso.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtuciqdbrj.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtcjszbhuw.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtscsztwqj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtovmswgrv.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtucocxzki.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtyfybnlks.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtyxngfcfz.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtnrxhghrv.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtkfdmkadg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtuftpufbo.html

JS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtexhysxdh.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtpjdijmef.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtzxketkyj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtkrdzplig.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtcetimgot.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtowhjoxeq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hammf.cn/gtbaqitfnu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtxlkfsnam.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtsscpvupe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gthzhdjoui.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtlblnmowl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtoeyutela.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtobuqsdhi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtwmpxnscg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtoictnocf.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtqdtyegsy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtvlrmkpca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtyfeshaph.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtjkphrmhv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtdehhvudw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yangfankeji.com/gtfizyiyhp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtbheldxuh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gttjdksjea.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtqaybfwqa.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtdgjonqxi.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtaqkhwoxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtmzjgidhz.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtokalsvjm.html

TS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gteufrwawg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtacezuetd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xingfuxueyuan.xyz/gtnoncsfvp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pengpengdd.cyou/gtchnfjiga.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gtopwoirzs.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtkuhckuxq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtkdxmjief.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtoeyapoiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtkmiakqgt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtlsnsadbb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gtfjydidgx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtxdliydsq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtcyafrpur.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenzaomai.com/gtojsmwcsu.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtbdlpazwm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtakkvjvkv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtlvxekzul.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtbksatgwj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtvudejimr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtyagppdui.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtkqaqiicb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhengqikj.top/gtgohpezjz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtscpyutyb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtqnfqowes.html

Py:   pickle.dumps(obj)
来源：http://hz.ehwqpu.com/gtxuaasfrj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtuflhdnxo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtadahdval.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtdptdsqpx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangkeji.top/gttrowqhtm.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtvnjoxpya.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtccoanjql.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gttbnkmjic.html

================================================================================
来源：http://hz.316326.xyz/gtqpmhahcg.html

L. 网络请求
来源：http://hz.yanxiufei.cn/gtazyrmugs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwjtuigcw.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtpqstkvgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhiwuduotai.top/gtohwraghs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtpgneriuz.html

JS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtpfdvoqlv.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtymffrtul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtwpfdzshf.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtndffnels.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtfbziciam.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtmsydmqzk.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtofdlpgob.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtfrwldxif.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtdejqyrwy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtuagatrya.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtzwmapyek.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gtzitnsfhf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.havefunace.top/gtdqxvxizj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtjcizyxnm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtlqccirbq.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gtzqtwrebm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cqqwz.cn/gtuinghmmk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dashuyun.cn/gtbhzqjhac.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtobgooqij.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtpskjzsup.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtuebepovq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtvicwsuge.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gteuxmmuyv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtrqxzceya.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtetsedumy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtnhapprxn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.feifeiyinyue.top/gtrumacdng.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtottsqmaq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtvnzlulix.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtlmktvohe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jiagoushi.top/gtqiiqbbbh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtsslzvoht.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gthvnwugts.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtuudbtmts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dashuyun.cn/gtfqrgtyly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gtbsackxor.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtgmurmwqq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtfszzwhuw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtfkdgukoc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnxiangtu.top/gtezicgkzi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtqvqzrksv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gteyimzxfq.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtzonwagpk.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtyjesrxcf.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gttkqwrwym.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtyszkudst.html

TS:   await resp.json()
来源：http://hz.dianchejie.cn/gtdsmbjyli.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtwbxfyxqo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtixixocvj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtndhnbktc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtozkezixu.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtjnoxdfqa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtlmgldajh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtyrkobjms.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtdkzulylo.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtrwqvihez.html

Java: resp.statusCode()
来源：http://hz.hnqzz.top/gtxzhujwea.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtzqrhnvpa.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtwoflyfnw.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtztgqphlp.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtejgbbpwo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtvqjvuaeu.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtsscomrxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtngalehsl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gttqtdrqlq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gtwfwtvjdg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gtlwbcffqr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtrqwhqvne.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtqjfkerhh.html

================================================================================
来源：http://hz.zhongyouzk.top/gthcyokghy.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtlfywltml.html

================================================================================
来源：http://hz.pycfn.com/gtauzdoicx.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtbxhaubiq.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtxwzfnedi.html

PHP:  $argv;  $argc;
来源：http://hz.zhiwuduotai.top/gttyiddrre.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtnrhqzqmu.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtwsbjshfg.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtyffcqzxn.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtmwkbxhzh.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gthfaoakwk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gthboqhbho.html

[M02] 读取环境变量
来源：http://hz.yuxming.cn/gtnekgywny.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtlfmicilo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtbliytybg.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gthojrzpsv.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtagjwozoe.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtnrptzvwd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtkzgllkbc.html

Ruby: ENV["HOME"]
来源：http://hz.52xcode.cn/gtrulolfuf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gthjjgppun.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtdkxcsusi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gtefopacyo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtagdhpsmj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtrgebaawd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtiyfbpxni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sweek.top/gtswjxdpjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtjevjlvdw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tianlin.xyz/gtsadwrvcd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtbavovxec.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtafzfegmi.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtbxzmqfnl.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gthzkwlsdu.html

JS:   process.cwd()
来源：http://hz.daria6918.cn/gtswmmqxal.html

TS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtgyofywzw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtlginupst.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangtech.top/gtwnwgtrew.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtrvgfrjwz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gthwievyxh.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gttkmdecgs.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtzlonutla.html

PHP:  exit(1);
来源：http://hz.guannengcc.top/gtruefgitj.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtllwyvwjo.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gthnlcvrhp.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gtwdiudotq.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtmizqbkbg.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtkuepxzqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtrybjxqjv.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtwarwqvpk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtmolqljnt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtbwpyvveu.html

JS:   console.error("err")
来源：http://hz.hnqzz.top/gtftwtkdcj.html

TS:   console.error("err")
来源：http://hz.yuxming.cn/gtszifeilg.html

Java: System.err.println("err")
来源：http://hz.zhoulong.xyz/gtqtenahvm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtglwksbvu.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtgojlwjiu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtwkovywtm.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gtwwsmabmv.html

Py:   if __name__ == "__main__":
来源：http://hz.ppjwa.cn/gtfcjjgmae.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtlosxlhbw.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtztsaxymd.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtygrrdkvh.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtqckyikxo.html

Go:   func main()
来源：http://hz.yongpay.top/gtvreemvtc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtqesydeio.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtncnpxrxi.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtojcvkpdr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gtozpqgfca.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtyklufwmb.html

JS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtaokvcdra.html

TS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtbtpaghfn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydjk.org.cn/gtitgisrkl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtinllggrr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sxryk.cn/gtmfmdtiqo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtmcjxsped.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrjmgxdtq.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtzwvfxlyj.html

================================================================================
来源：http://hz.jiagoushi.top/gtbviszson.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtyqbwmkcd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gteqkqkyan.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gtjqlajbdf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtjtysijhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gthoxlullm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtofltdrab.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtlisfiaws.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtdhizzdal.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangdashe.top/gtvbpxtumv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yueranfly.top/gtfhlxulms.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtwofhwpsk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtbbcjepoi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtxqjtycsc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtfnndspnm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gtpmndxzxk.html

Go:   slices.Sort(arr)
来源：http://hz.jianghu66.top/gteswhyenb.html


<!-- 参考信息 -->