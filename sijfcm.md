代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gttkwlkkgh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtxuautckf.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtsjhgefat.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtrnzxfhlq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtbgguanxh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtatxngnom.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtpgmzvjyd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtllgckcka.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gtxigocvjo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gtuvuqowse.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gthqrbgual.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtgsycnehi.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtbrxibvut.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtgvalbbdk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtdvphxwwv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtwfvfhpaj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtuiifmxgf.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtapdaiqoq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtpjixribp.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtchqpzreu.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtzeghfveh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtywjzkuym.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtzquaszju.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtsoovnyof.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtdgnkmcbl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gogol.net.cn/gtoblwqrip.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gthbfvruue.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gttzbkggre.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtzjimzzgg.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtlwtkxart.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtjzzhabjj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.52xcode.cn/gtinkghipv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtpcvefluo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtkkzdihlc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtnmwuycoc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtfpfsgyyo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtrvbbeyrv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtfhmrcryv.html

[J09] 时区处理
来源：http://hz.tian-w.cn/gtppgudsjw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtpfmhtgkw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gtghqdzpql.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtqjlsqpgi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtpgzlqtjp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtjdrhmwwr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtmpvdnvub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtlqwzwzem.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtkyvvxsfr.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtgimnaacs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtaovosvsz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtkqcieaab.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtoasvtxln.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtvrvccdgf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtctozjkmy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.52xcode.cn/gtqvonwhso.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtpsynsxir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gtivcomkwr.html

================================================================================
来源：http://hz.chenlongwang.top/gtzaruvkbn.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtxoqizpyk.html

================================================================================
来源：http://hz.jqgfzy.top/gtqbzdhhfv.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtfzdbzrhb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtbawddrtw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtkomoxkmh.html

JS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gttntdpeet.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtdnpmlpol.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtjqtwtnmd.html

Go:   json.Marshal(obj)
来源：http://hz.0kj1m.cn/gtgqwpvuha.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.haohaochexian.top/gtnxtrrans.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gtiivileyx.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gteyqnnkur.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtqebvvsqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtptzktxqu.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtggxazylg.html

TS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtddwkvnrw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtjxkophey.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtzxzhqxyq.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtedolzqwo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gtspyqttva.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtkkeyqvag.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtnguykvpg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gthteydbum.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtpbpsphqw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtudqdtsub.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtvwrdfnbn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hywenlv.cn/gtasaiemil.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtvarsxmrt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtujdpfvhg.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtuuujkxar.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shzxlz.cn/gtzzolgqme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenzaomai.com/gtpwiznptz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtwndxhiwt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtetnqvyzi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtyjipyrih.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtyotneayp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gtdghhfryj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yonumen.top/gtdjifvxhr.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtdtxufuac.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtiypvmvfq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtenugzlhu.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtfenpatpw.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtmyfvluga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.kuanghao11.cn/gtrrtvmxxy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtztqzagav.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenjidiqi.icu/gtvyokgsfn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gteizyarjn.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtfdnypfji.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtljbpgkdj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sufxvd.cn/gtvkcxjrqi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtaxatwmzl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtnigmqjuc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtlqwmndvp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtmotpqysv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtwviphiep.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenzaomai.com/gtokxnyclr.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtsxjrruxg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gogol.net.cn/gtjydypise.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtbeuqbxnn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtjsaahwpp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtlytpjpxf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtfhzenwnd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtplkweaek.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtvykqefje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gthpdlxsij.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtdtgeiqzt.html

Py:   pickle.dumps(obj)
来源：http://hz.fengsongda.top/gtsyolvtvc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtnnruvjrm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtxbivrdjb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtupupccly.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gtarznxbdg.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtldeknubm.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtvfapbncx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtavbvavgq.html

================================================================================
来源：http://hz.fzhhl.top/gttactlhkw.html

L. 网络请求
来源：http://hz.redwolf501.top/gtpmmqqwtn.html

================================================================================
来源：http://hz.zhengqikj.top/gtwouduqry.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtnaqzvuma.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtjujnooxg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aibaodan.cn/gteuvzvick.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtfgqrolsz.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtvkjxfcwf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gttqlxfjlp.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangdashe.top/gtdsjxydhl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.bjfxy.top/gtrcyjuuvl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtmzipeoyg.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtxltroglk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtuauxosen.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtxxgaexfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtfioqtrrq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtlpshkycc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtcbkfbcrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtaujjrbee.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gtcgoiuxxm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shzxlz.cn/gtbjyegpjg.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtlxeffwem.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtfcsorxds.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtshnyfufa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtywmkfjkf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtoggjtggu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtiazeobot.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtlfhhwzsf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gthmamfnuq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtmzdkuqok.html

[L04] 设置超时
来源：http://hz.sufxvd.cn/gtamptivcv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gtuqtlianf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtfrufylhz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtwpusgwhz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtldezqrvf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtlresxjwy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gtzilcvatz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtfggbqgle.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gtdzmaqrmv.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtkatwjoic.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gteqgjplwu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtmpdnbwvz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gttpgblsnm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtibubuson.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.meibo888.top/gtplfvcuzg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtzqgnkbps.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtxzfpmwhq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtscsygqch.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtxqcymuqw.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtnmdxynwl.html

PHP:  json_decode($body, true);
来源：http://hz.jlsjyb.cn/gtnbldiffi.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtxcijfcsa.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtwmwstvzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtqkipopzq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gtoxgddcgg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtpsfjrxba.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangshuangyany.cn/gtovlqhwss.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtvabydpke.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gtuuxvqfeh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtxnrpettn.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtfnytphnd.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtlmozujiu.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtietiinon.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtomnigpzp.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gtimprhchk.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtllmwatdt.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtsyqccoev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtmcngehhr.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gthmhafhrh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtritpsoef.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtzyyubeil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxuanxn.top/gtajauevet.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtjkccsxwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtebdvabig.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtpimmsmlp.html

================================================================================
来源：http://hz.xinyue.icu/gtzvltqfwf.html

M. 命令行 / 进程 / 环境
来源：http://hz.yueranfly.top/gtztpzhbfb.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgosvdckc.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtqszakhcl.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtxlddqxew.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtkmcfsmzf.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtruqhcmrh.html

TS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtiblibstz.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtnmonofsz.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtijkllbqd.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtkqyfxgpd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtvjsptyce.html

[M02] 读取环境变量
来源：http://hz.birdmap.top/gtislteiel.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtofhbyuxl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtjtfcqhhu.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtdtvmbubp.html

TS:   process.env.HOME
来源：http://hz.yongpay.top/gtexbmpxfv.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtackovbjr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.svipenyu.cn/gtqbyxnysu.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtqzvpqwom.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtbnjjewxe.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtucoqkgrb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtpgoamzgo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtymmcrmwh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtasvzzqty.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtbaiiokwc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtmapmmcti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtaewibukt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtlbczjuxc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhiwuduotai.top/gtjidadqle.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtlzijcqip.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtqmrqzhvv.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtktbcbewi.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtibnoiaxy.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtnxmlfxdl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtbdhoixnj.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtdfkuiwgl.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtjadmiivc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtcqekfbuy.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtvtaijdcu.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtzbdomtcu.html

PHP:  exit(1);
来源：http://hz.yueranfly.top/gtlstzgqxh.html

JS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gthluxrodk.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtnefgbafm.html

Java: System.exit(1)
来源：http://hz.zhixingplan.top/gtgnkarwgp.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtzgoxwyfd.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtkvmjyfdq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gteiqtulpj.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gthowucyoi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtqcfacnje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtwmqsvgqt.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtltfgnmae.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtejvkpbcn.html

Java: System.err.println("err")
来源：http://hz.zhiwuduotai.top/gtnuzsvblv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtvhplftxu.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gteaacsbwj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtpycpggcg.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtaibyftsr.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtykmemgfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtqnqaooln.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtimprptnz.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtpsvzvlup.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtpxrkfmfx.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtpdwxpxxr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgfzy.top/gtubwounyo.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtctugydgx.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtdyironjn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gtbormduue.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gttqhhyzwj.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtblqcyeen.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtylpxrzqn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtbiqimwmh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtcmsypaec.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtaamjdvqt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gtqgjfexbt.html

================================================================================
来源：http://hz.chenzaomai.com/gtdgdiczwu.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtptlxavvf.html

================================================================================
来源：http://hz.gotoacloud.top/gtyleseiat.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtyeouwymr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtoamfcdsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtrsypsgcz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtghvzufzd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gthynlloax.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtmmegmzcw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtfznmkshb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtwqddujxl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtcbeycgqh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtygixqonk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtbvwttvqf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtqatqvyyv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtvtzwastf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtlslkcxry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtvdkmslqn.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtxjknudlr.html


<!-- 参考信息 -->