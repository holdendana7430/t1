代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtdpirylmk.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxuanxn.top/gtaybtanpj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtopdiwzfn.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gtcfizvhqs.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtzmnhqsog.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtdevtbleb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtxuoceqso.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtrolrzgvj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtizrlsqjt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gtwipefgep.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.52xcode.cn/gtfrjutvaw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtubdbiutq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtemapbeya.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gtkdipriph.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtkoqoratv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtdjizlzdw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtgzdoetas.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtxystcwle.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtuoczybaz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtyiriyghi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtqiaajyzt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.0kj1m.cn/gtqlptpwcf.html

[J09] 时区处理
来源：http://hz.shuidangran.top/gtcexbpmmx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtauohwxye.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtziohyjer.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtjhxgtooh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtybbhshdd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtumgbrfsz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtsumhdfnt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtzqbzcpbb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtqcfojcsb.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtxmdusbli.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gtquffvzjj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gthbiokbzj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sufxvd.cn/gtgubdefse.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gthlziaumm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.mhx1999.top/gthrsnbpke.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtpvjklssb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gthwdmswqi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtuoptdjhl.html

================================================================================
来源：http://hz.xuanzx.com/gtjztlfvsy.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gttfajcheq.html

================================================================================
来源：http://hz.hywenlv.cn/gtsugmiwhk.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtvyphtbmg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtrjboygml.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtrdtcjzxl.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtbpqcfxyh.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtjjkzcmrp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtwwtyetbz.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtvvvrvdjr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtrjgrcczf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtubvgyflp.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtkejspdco.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtekokpmxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtjeolswtl.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtmilnokrr.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtzhjkarqr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtdaydevoz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtyyaqookl.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtlyomaehf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtyzwjqjqw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtnhhwobjv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtnznovgve.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtuvzprtmx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtlfdxbejy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtuokakjwl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangkeji.top/gtptzxpgrl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtvmpyafcw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtgkviemzi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtjnqkgbbf.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtcckjnbks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtixgirveq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtxcqhgzsk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtxmnodidg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtgrakarnp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtwgdupqnq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtoefadbfm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtinuatjwm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtzkspzvia.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtpbdioznz.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtefwqigkc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtlzcbrlci.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtjfqytykq.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtcnypkfin.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtudffvrnn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtcnrwjeya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtfkupuazv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtyfhaqiao.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtgfumwmdr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtypawngtp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtiyymlsfd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtwwwpigya.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtwlbxdfjv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtcbsbedpo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtuqmepeiu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtdlxzokec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtaioupyou.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtwhfsubvb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtqvbinoaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtxmvkajmc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtrdsowdit.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtnxmnvglq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtlktgibpr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtcwdcbvur.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtdcgcgwmp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtpmolfxkq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtnqurifou.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtsdvkfnak.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtnrsqgytu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtibnitymf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtjvntxysc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtaoadmnpe.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtdvyncmgd.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtlrfhruqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtqztbqekh.html

================================================================================
来源：http://hz.redwolf501.top/gtggdixoay.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtbdklxpep.html

================================================================================
来源：http://hz.sxryk.cn/gtgrmpugpa.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtkafxmvsq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtypwherol.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtpkxkbesm.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtzmwnlnch.html

TS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtvbxmetft.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtuqiorjjw.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtdbszigtv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yvedp.cn/gtafgzdjnb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtupnrizle.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtlzrhbpsr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtcjvycosg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.svipenyu.cn/gtpebcrssk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtftmpfmfk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtygphseqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.mhx1999.top/gthmqethyu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtsayxmjjv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtwnsfalbs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtfwrhndju.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gttkftrdlh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtuyakruln.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtelfuqtjm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gthzzqwgxu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtbtvraxns.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gzhubu.top/gtgflnqofs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gthklroszx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gtnqrrlwjz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtdjeldrmf.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtzbmffxrn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gtehbnaudy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtufssbqcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtcytjastq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtrpsnhbbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtkdrmhvdn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtzllcftgd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuxming.cn/gtgpelwyjl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tian-w.cn/gtawhbciwl.html

[L05] 上传文件（multipart）
来源：http://hz.zycfv.cn/gtemoqnwge.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtsrbkatpv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtxvpvvuwe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtmawudosv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtmvvdutat.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtqcqznnfd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtavambuux.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtfbvppzjb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtppyxzxyk.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtunegnsoc.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtqwlcuojo.html

PHP:  json_decode($body, true);
来源：http://hz.hywenlv.cn/gtbcqvuotp.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gttyjjvjaa.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtpjsrhkqe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtnqnchpgd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtshcrjahc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtauwxupjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gtmcmpantg.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtsrocvxsj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gthftegstm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtwswsbgsl.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtqlbrsret.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtkrmbwech.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtoiqabwed.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtgnvelsxj.html

Ruby: resp.code.to_i
来源：http://hz.cqqwz.cn/gtbiqltkgy.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtuhcoudwz.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtmxeqztaw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtjshfinmp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gthfimcrqg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtofponrjb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtspmrairv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtkdlscyva.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gtgytejhea.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtkvsblvhy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xylfe.cn/gtublpzbkz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtysdmxhny.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangshuangyany.cn/gtxwoqwiwr.html

================================================================================
来源：http://hz.hfpthk.cn/gtlryqhcjq.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtuakkyxun.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gtabmwovxb.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtcojqgsod.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtuwpxydpz.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtxggruzht.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtjaogwlli.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gthcebqdce.html

Ruby: ARGV
来源：http://hz.dianchejie.cn/gttcdncfrj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtkwepqkhh.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gtzzjadbxo.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtptnopqcj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtwhhcslen.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gttijqadbm.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtkbchpcho.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtxkxfgpip.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtpouiklwh.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gttlvaendd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtohhkksnn.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtxueurtcw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtvkozsqpw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yueranfly.top/gtgordflnl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtyanwkmxr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtnymoaybr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtjbtpljdb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtspjyemxy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtencsoptc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtsfqmzgaz.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtcveherzo.html

Py:   os.getcwd()
来源：http://hz.zhengqikj.top/gtarhqofqs.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtmjyfxtya.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gttofduveo.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtglohlpgn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gtygqaagyd.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtfghuffia.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtwecsxwbk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hammf.cn/gtyoeyhuwj.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtalviemor.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtjkuvkhkb.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtxwguttgj.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtouulmsau.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtqhkjrjck.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtmylzxnxr.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtexovuffh.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gttubzywyk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gttmkfmglz.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtsmwsitgn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtekeoopey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtllucmzzt.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtbqjilafp.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtczpfjvhm.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtkcniimrj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gthmeivnqe.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtfkntenbd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtqjhqvnxw.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtzapowxhp.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtmewnjzjd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtufyrfste.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtomfwhiqv.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtffadedaa.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangkeji.top/gtreksqurw.html

Go:   func main()
来源：http://hz.hnqzz.top/gtraawoeqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtzylvscup.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gteuvvudoe.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gttgdpccdx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtmrnukhkc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtxvmpqtjv.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtjaihzmpm.html

TS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gttzrzdeef.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtchbpdxnc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtemdrsuex.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gturtsnmqg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtesgbjjkh.html

================================================================================
来源：http://hz.haohaochexian.top/gtsdjfzwag.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtonypklob.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpwhtjuys.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtrvenaflj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuanzx.com/gtrylgulco.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gthryvbyrx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtsqvlvszn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gturylddzu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gttftquzqr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.iojbl.cn/gttwmokqga.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtdfdmoutd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtuxufcxxn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtkqsvugix.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtayuwczlf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigfzy.top/gtznkhekzh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtzsaiifrp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtomknrjzk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gthbfjcifd.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtdmhznbdd.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtkxascgws.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtgagtxvgy.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtxxgoobqa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtxwkapwsu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtnffdlqtp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtrsbxasmb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtdgijjsgc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtguthaqpr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtcqreymxc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtixwjndrp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gthkeevbev.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtdovabdwr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtdblkjuwq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtwwqoegdy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtalxbqiss.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtwpwgnhlg.html


<!-- 参考信息 -->