代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtjgqkmrqd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtaelslacb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtesntwmpd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtrubfkqpn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtrtygrvxf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gtxslfvjkr.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtrzdpeugb.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gtswmlqpvl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtwuxejgud.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtwwoyebdd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtfxlgcdsp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtwvaksofo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yongpay.top/gtmxwphiwx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gtqmwvlvcs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtsazsnybl.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gtnywtbzxu.html

Py:   (end - start).total_seconds()
来源：http://hz.chenzaomai.com/gthdogjujh.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtxlbcsoyo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtvdzravgs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtihtatrnw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtxwyxyluo.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtkqbpjzer.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtyenkveuj.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gthjgxfvqo.html

[J07] 比较两个日期
来源：http://hz.zhoulong.xyz/gthbrjxccj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtpnagyoim.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtlhxtlzub.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtqkyovsto.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gttkipautm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtghzlwflg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtxjvxoniq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtveumbgcf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtojwefyuh.html

[J08] 提取年月日与星期
来源：http://hz.yueranfly.top/gtjydivtei.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtuvecilob.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtxbicqczk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gthbupzwzw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtoenipnls.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cucudq.cn/gtewwyejet.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtggykqsdq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gogol.net.cn/gtwsqnokji.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtvjylmlot.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gteaicssem.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtismmpslw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtqkuuxmra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gthnjpaerd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtmlqsmnte.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtyormwclg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtqegzbguk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtdhclpade.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtvbjwxwyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangshuangyany.cn/gtglykueyt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtkdmonevo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sysykeji.top/gtyaljxwqh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtnwmdyscd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtfiqzggag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtdihjrjvm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtbbtvtuxx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtmuhkzanx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigufen.top/gtgbzffeil.html

================================================================================
来源：http://hz.mhx1999.top/gtvvqdxtor.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtaluxufzo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtuxnmiing.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtckklffuu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtharmpmet.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtnxikeyzx.html

JS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtfonrhlku.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtlfybbbvw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtozaukiso.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtlbjdiofe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtmftowvlp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yueranfly.top/gtjrgocxen.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtowrouges.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtfrphjhxc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtkaxpoejc.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtaudanjut.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtswxgdpwq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gteroqcahe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtbabhxzav.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gtfrwzsnxu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtwknwuowm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtjwunjigg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtluvqurwx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtnimskuqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtzrueozkt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gthbkvshve.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtwcqmzfoi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtkfovnord.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtdzkavcya.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtmlkpmwiv.html

[K04] 读取 JSON 文件
来源：http://hz.cdnleiting.top/gtkjgdxopn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtwkawcijj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtcaaphjku.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gticlblhmh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtzyiaxjee.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtjerywetl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtoyqranoc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtsttjgjzf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtvnxdogib.html

[K05] 深拷贝对象
来源：http://hz.mhx1999.top/gtvgaaiosb.html

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtttljyljf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtetjnbrew.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtmivymlqu.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtiqfexfqd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gttozdnjoo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtxmsmsias.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.0kj1m.cn/gtukuwdtll.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtkinqmtkw.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gthsjjzeye.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghu66.top/gtwytonrej.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtpgwgntgd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtyqhvjoky.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtqonyyckv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangdashe.top/gtjqliwypg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gogol.net.cn/gtedybopwl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gttbzuywjj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtvunofmfk.html

[K07] 进制转换
来源：http://hz.shzxlz.cn/gtshodcbru.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydzc1.top/gtjtpcqigh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtbiyfksey.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtdgqdjerl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gteumzgupl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gttbqqcgfe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangshuangyany.cn/gtqtpgqzhs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtpeqtmcmz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtgtybowcu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gttquizhrg.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gtsvwcmphc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtwvojaeym.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtykbolqem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtmycgaqzl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtbtuuwfdh.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gtpzkcrgno.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtbiakeuna.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtakmdlpkl.html

================================================================================
来源：http://hz.yueranfly.top/gtjpvwzade.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtzjklcjwc.html

================================================================================
来源：http://hz.shzxlz.cn/gttibxstdd.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtbnonrmho.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtioeygmkv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ehwqpu.com/gtcxdldhrf.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtxrsrnvfq.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gttwwiojqv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xylfe.cn/gtaxkhuusf.html

Go:   resp, err := http.Get(url)
来源：http://hz.daria6918.cn/gtofqyhtvi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtkqeqokzp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtgkjgusjg.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtkjssovvc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtleerwxvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtcdewldcc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtifmtnxtm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtukxwtapj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gthwvcnyur.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtbmdphtqs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.birdmap.top/gttnffgiqc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtfnzakvod.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtqbtwzfdg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtegjmzeem.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtwvtxmlsw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtscslqgsq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gttzkruraw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xingfuxueyuan.xyz/gtkiqwgwbw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sweek.top/gttgchzzlu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtxkgyqpvt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.havefunace.top/gteclicnjp.html

[L04] 设置超时
来源：http://hz.sysykeji.top/gtncauvnmu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.0kj1m.cn/gtlrpyyliu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtncpshtts.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtmsbneqch.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtphfcnqyg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnqzz.top/gtmxoakozy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nwbrower.top/gteptajzyc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtvevxblyo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtxhdowujp.html

[L05] 上传文件（multipart）
来源：http://hz.dianchejie.cn/gtmhsslvjw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gttzkxdyxb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daria6918.cn/gtkgrmivyc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtsnnjyjks.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtffipeepl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtpxqelhsr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtrxgjovib.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtdldatelr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtssntschd.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtbnphlepr.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gtxgwgcrsn.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtulzhfnje.html

JS:   await resp.json()
来源：http://hz.hnxiangtu.top/gttdcpurxt.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtkxnewqni.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xylfe.cn/gtmieyezzw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtqtlufxxg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yvedp.cn/gtqmlxxbeo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.c1oappe.top/gtgtmdnffr.html

[L07] 处理 HTTP 状态码
来源：http://hz.pycfn.com/gtppavwdkg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sweek.top/gtfcidunfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtxkkhnikh.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gteghvbtkv.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtyynmsfho.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtvkaoaopx.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtazdpvhwm.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtbiibcckz.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gthxcfrang.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtdtiqgphh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtiraqrzsl.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtgknpdkzz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtffjrdffb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtfojmgsvg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtkpjfegok.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtkccxzcdh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtyikmrwcy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtxcxagbcj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtskvlxvwg.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtsfshkgux.html

================================================================================
来源：http://hz.daxiang520.top/gtzwkvwcpg.html

[M01] 读取命令行参数
来源：http://hz.cucudq.cn/gtcwebrjck.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtfqwoyydk.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtybdbepda.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtdoonovca.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gttlddvfbr.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtqpnbhulq.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtebeoxvgw.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtekkloaqa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtolljhcci.html

[M02] 读取环境变量
来源：http://hz.zdqjudy.top/gtjvowbfuv.html

Py:   os.environ.get("HOME")
来源：http://hz.vqdsnc.cn/gtzgjynium.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtdafnqlal.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtjhljmven.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtbjjgdion.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gteerpaggy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtjetycjtd.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtnjmlcxve.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtojfxjbzd.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtznbotvxd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtrggmtmfd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtpsvbuugh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtejfkfbrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtpywctahu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tian-w.cn/gtxazwkzlf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtkokykhlt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gtbfjyfxds.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtfjqystiz.html

[M04] 获取当前工作目录
来源：http://hz.iojbl.cn/gtovhavraj.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtxspmuyvb.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtohvryiqf.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtswvotqou.html

TS:   process.cwd()
来源：http://hz.nanxinkj.top/gtvyreuoup.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtfdnxgbxm.html

Go:   os.Getwd()
来源：http://hz.shzxlz.cn/gtseyftgkp.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gttzosajnd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtcdfehyfa.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtkeufgyzn.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtiprjxocl.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtguxvijid.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtiupspnmo.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtbveuiotz.html

Java: System.exit(1)
来源：http://hz.yj20258.top/gtjudfjxqa.html

Go:   os.Exit(1)
来源：http://hz.52xcode.cn/gtiztzdart.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtpzpxztfp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtenudikbl.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtsgtdtweu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtpyhzcyft.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtfpkxfkpl.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtflmhfoxb.html

TS:   console.error("err")
来源：http://hz.guowangkeji.top/gtaidavenn.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gtcdpzrkoh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtvplfvury.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gttslvbqyz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtxrqqebyc.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtisottprn.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gtkxeooylh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtzxrtuvbp.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtqijdobnc.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtsopdzepa.html

Java: public static void main(String[] args)
来源：http://hz.jlsjyb.cn/gtfuathmek.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtlzrepfce.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtrtwdhcpe.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtjqkybmrb.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtorwlwjtw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtathjefyp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jiagoushi.top/gtizhdrqbm.html

JS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtcfwfbjdg.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtmtzteqwo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtynogpjzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtmxffydyk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtfxvrpjnh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtpjogxfbb.html

================================================================================
来源：http://hz.yonumen.top/gtcxbbpxmt.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtemdottab.html

================================================================================
来源：http://hz.cqqwz.cn/gtjdcjbfcg.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtnwokcwyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigfzy.top/gtnrwfejyj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhijiandao.cn/gtcoqmpqbz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtqbsqyrwm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtpaxrwyhc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtkwflgyst.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtsmengkbl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtwiqrgtvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtmungpinh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gtnccmkipl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtfkeqibtd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtilyypqvn.html


<!-- 参考信息 -->