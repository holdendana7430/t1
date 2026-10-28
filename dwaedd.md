代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtytrlyvyv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtavpwmgvu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtnrztawqj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtkyprzaus.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtmaszjrsw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtsancyxit.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtjbwvoqfi.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtugvkoooh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtqdctjwde.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtyubwcajs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gthvbzzkhj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtpiwumjjp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gthsaulovl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtmdforptl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtbouqdjom.html

[J06] 计算两时间之差
来源：http://hz.fzhhl.top/gthyqxqikd.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gthqudetso.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtxwiczbek.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtsmjowabe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtengauyrt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gtuqollaxc.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtkmunifkp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtsoljnslr.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtnpduczuk.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtstejybqp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtptyezxcr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhoulong.xyz/gtxfgaconm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtdrcntjny.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtkukmzezv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtoldxoaij.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ivvv.top/gtzjojzpkv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtcpgrfbvi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtlarionns.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtufhrbils.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gtzultymso.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gtjqgltwun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtytlgnjrv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtaevfgdja.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gthajbsdkw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtheouxhyf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtqrfxsuyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.0kj1m.cn/gtzdsgrkwf.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtocugoxdj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtbukjruya.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gzhubu.top/gtnderxdru.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtyzqgcapz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtbllihjpe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangkeji.top/gtxubgefhr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtbiuockwu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigufen.top/gtkkdwborq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtbvbczmnm.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhengqikj.top/gtqnzrmenn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtmsmsiigi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtwwdvaljo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtjxkhxnvv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtywxfrksv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hfpthk.cn/gtmamlwqkf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtbqytyejb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gttkxgxzfm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gtdzylfjgz.html

================================================================================
来源：http://hz.guannengcc.top/gtejicizmw.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtzlgscwbw.html

================================================================================
来源：http://hz.chenzaomai.com/gtxokcjvtq.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtqawypqnq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtpsneydbr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtiufsdtkd.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtywtqtaas.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtykrjsknn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtlhzkqgil.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtcspkpiqf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gtcbitolni.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtkcguhitu.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gtputcweea.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtmotexybq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xylfe.cn/gtgvxrvfcd.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtzpihmlex.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtvweojpqr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtficsuseu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gthwnvwdds.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtojdyejzx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.52xcode.cn/gtcrbgxplx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gthpmnwkwu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtavcwdogi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gthlvvbnht.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtcsivefuu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtfvasepgj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtyxbjifzr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtbrihdmuk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtboblqnhq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtmjzkdewv.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtuchetvnn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guannengcc.top/gtthyiuctw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xinyue.icu/gtqvdwgmei.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtieraxdwc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtntsglgfc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtfpkklajl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtlnctjvwi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtoyvkxbmo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gttgizjbuz.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtvhvgnint.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtlfeprhrx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtusfqqgzw.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtvbvfbbro.html

TS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtqyjdutsk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.svipenyu.cn/gtzxeqlbtc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tianlin.xyz/gtqtvyyzqh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtuwxgtffy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtgztezmdv.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtqomvynba.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtohtgmyxh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtvrbssyjj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtyxpevibp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtaenzwqit.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtfikxypmi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gteumgmirv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtiytuajcu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gticsgrcyc.html

[K07] 进制转换
来源：http://hz.ehwqpu.com/gtbcniiomz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtbqkcgoxi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shangyingyoupin.top/gtuyzrhrqx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtnvvrvsau.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtomohyiqn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtnykmbkfa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtxhxzqsri.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtjuovehad.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtshkavybs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtxcopetpx.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gturbwrkwk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtfnglweht.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtbrstjsxq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtaghyszqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtbynkzugg.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtitmrinhq.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtidkwsryp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtbtaxhyjg.html

================================================================================
来源：http://hz.yj202588.top/gtlbrzdzvz.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtqcrnogmy.html

================================================================================
来源：http://hz.pycfn.com/gtpznpashw.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtlwlnjjsa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gtwrcvnycb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtolammars.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gteutnhwsl.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtetkaybif.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gtmgacjozn.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtnxfqxpqh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gtgqmxvxyd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtrvkzyupl.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtwuwgfpry.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtolauoego.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gtqeekiots.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtlmbcvhhz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtxyutnugg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.bjfxy.top/gtvadejura.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtzngpaoyq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtmobrnrqk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gtkxpqayrr.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gttvektauj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtxtiznzhi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtxkkrrkkf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtabfnmord.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtchzbmyaq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtpycpnqdx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cucudq.cn/gthnsiavej.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gtjcdhqrdw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtvidnhxhp.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtzheshaow.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtrmlypkkk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gthxgcbwrr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gttdgzdaqb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtwadjlgfw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtzberkesw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtghdqfrko.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtzddccfnx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtetpzflil.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtegkbfyfe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtxqigfwqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtvsurrjpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtbnkvlrlq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtuywbdqyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gttnamdozl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtqcruauxe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtgkdvgqcl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.redwolf501.top/gthpmahskm.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtgqcobqta.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtrjccbpys.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtvcsnohow.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtwzcumqno.html

TS:   await resp.json()
来源：http://hz.andypj.xyz/gtuwnhucll.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydjk.org.cn/gtsvczhpgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.bjfxy.top/gtxlrrgrfr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtqpozyjpv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aibaodan.cn/gtqqamrolm.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtgqhyiwcb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtbncfokud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtobchgsnw.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtbomexnre.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtooxgxljv.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gtzdfrelbm.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtxhiogfug.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtkgylqddw.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtsomnmcds.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtrujulaze.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtyfisunze.html

PHP:  curl_multi_init() 系列
来源：http://hz.cheryme.top/gtelpylcis.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtxneumsqm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtouuxjvtm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtjpdxdckf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtqvrswfbm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtufpihluz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtgdsbcbpo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbakfnrxy.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtpkjmudig.html

================================================================================
来源：http://hz.zdqjudy.top/gtiypyerqr.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gturwxidyo.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtqciwesgr.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtgvbvpbxc.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtutbbfooa.html

TS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtzcbpqrrp.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtbmdqfsmn.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtgztthzgq.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtxvhrzkbt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtoaauxmei.html

[M02] 读取环境变量
来源：http://hz.hongshengwenyu.top/gtbrvfzrlg.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gthnxkroph.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtotosrlit.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtxcrchfki.html

TS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtgcwiycrj.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtafozhoby.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtzveafslt.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gtpovxmwbd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtximhdpbz.html

[M03] 执行外部命令
来源：http://hz.zhaomingkeji.xyz/gtyhlyqxlk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gtrljerxth.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.316326.xyz/gtvrnbhnku.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtvjbqhsgi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtydozqiwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtpxaejrwx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtjqhvqzei.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtmgteaizt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtvimlabzy.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtpbawkhgi.html

Py:   os.getcwd()
来源：http://hz.gotoacloud.top/gtznkzbqiy.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtengmfosq.html

JS:   process.cwd()
来源：http://hz.jiagoushi.top/gtfabkbsyi.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gthtezfdhc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cucudq.cn/gtvintrhcc.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtmdtkkzrw.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtnbvjgajj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gttjbjqpsu.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtljchgbqf.html

Py:   sys.exit(1)
来源：http://hz.hammf.cn/gtusyhgoug.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtyahsthba.html

JS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gteclwvuuh.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtmdrefshm.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtdavpcsrj.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtvjpvebrg.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtcdebbazy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtrswqrnog.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtvzjprecx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtyecsxbur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtgvnabbnv.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtbmoxhpur.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtkwfnfkmm.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtntzumqvy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtkchxjmcp.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtmbvzjeav.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtplgltpsq.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtdumwweyv.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gttqmtlghr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtnntjipud.html

JS:   require.main === module
来源：http://hz.9152youxi.cn/gtkcsqihod.html

TS:   require.main === module
来源：http://hz.tanke756.top/gthyzwhupr.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtyqysvrvw.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtundblwtu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtlahuwvxt.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gthlewhojq.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtcaqeohcl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gttknqbmed.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gtqthbuwxu.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtqmbbsqev.html

TS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtocyuiuix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gthckoipil.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtybtbhyiw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yvedp.cn/gtrshubcxp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtafhckqbp.html

================================================================================
来源：http://hz.yj202588.top/gtzrejkhdm.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtenujtdnt.html

================================================================================
来源：http://hz.cqqwz.cn/gtjpeihwtj.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gthlfubgxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuanzx.com/gtuzssueuh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtlfziychn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtvoylvhii.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtntkxmhxr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtwmamtfrd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtggsyycht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtltvrkwxf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtqkjtjkjm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtwwkrhepn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtmrlzbiic.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gtivlteegg.html


<!-- 参考信息 -->