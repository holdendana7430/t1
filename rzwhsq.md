代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtjktfgonm.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gttocepdzl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gthmggfdda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtoouewbhb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haohaochexian.top/gtlauwbxoq.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtfmcroklj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtoeegchoe.html

C#:   (end - start).TotalSeconds
来源：http://hz.jyoumei.cn/gtcnhpmpcn.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtyhdnwpqq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtqbcekpxn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtnzbkagmv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtslufkpil.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtjboxohww.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtwtupimua.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtqamizagw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtrdwmhzyk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtfsimipfm.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gttucyfcxy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xinyue.icu/gtaxajyior.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtafmltwdg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtlnddclnb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cheryme.top/gtfapkeque.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gthaxfbbqq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtvvvalzau.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtqnqhlkni.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtdhgznxmd.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtdbvqpfue.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhixingplan.top/gtgtkcfbbu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gtuoluztqz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtnknbuutv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtzuucujbt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtufdebpfu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtttbgwwdn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtrgxzwqok.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tian-w.cn/gtotdoktrk.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtqsqopeqz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtfsnlotra.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtscuhsepn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.svipenyu.cn/gtvmovlgtk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtyujteblj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtvmquqazk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtuyljldrk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtohfgqqoi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtmqqpdssq.html

================================================================================
来源：http://hz.aizwys.cn/gteqrxcasc.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtuehbqltm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtjxskzxvo.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtvyaxdbmh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtattkqjgf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtwoyvltlw.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtkhjlgdbq.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtgzjqhyoi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtwkxcxugu.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtocvnizqg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gogol.net.cn/gtlzwuixnz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtqtapjwmc.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtpmkomjgr.html

Py:   json.loads(s)
来源：http://hz.aibaodan.cn/gtkcxvpqks.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.havefunace.top/gtnydjller.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtqkqeyogk.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtklkldipd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gthzxalheq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtwlvqjonq.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtfkkqvdyw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gtdfmxlxyw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtbrcdcbqh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtluurouxa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gteisayebh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtbkznniph.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtvmktvlry.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guannengcc.top/gtihscrbat.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtzrxmkvwt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtyejjxyvq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtfhwgjwlv.html

[K04] 读取 JSON 文件
来源：http://hz.xuanzx.com/gtywdnpywt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuetiantiany.cn/gtzbvhhlde.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtdlvhvgvj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtjeztztgy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtowpqwlmu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtpbklyyjq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtqyiqlzns.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtbwgefnqk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtyxvaipfc.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtyldjwcly.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtzuuqkffu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtxczaasvw.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtfykuveks.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtoanptdir.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtepjoumek.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yangfankeji.com/gtqhvrhylf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtxmjjdxmv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtojdctmvs.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtjievsevx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtsxxhrxtj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtxdzoihlp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtfnogpmor.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtyocbtrkt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gttobpuahj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtyytdbkpz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuxming.cn/gtpcbisaqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtitzonjuh.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtaxtfxaqj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtatsbnkjq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yanxiufei.cn/gtevxayikg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gterazqmrb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtdkxiener.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtgsswemwr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtymxgxgwq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtboigfyov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtexkgiihj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtobatogck.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtaiijgogg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.9152youxi.cn/gttlriqhmo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtiryrytuh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gttxntjwsz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gthgqcmyfv.html

Go:   encoding/gob
来源：http://hz.jinyuanbaomall.cn/gtcbpawfnf.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtirhskiov.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtrbbusznd.html

================================================================================
来源：http://hz.xinyue.icu/gtmqzwphbq.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtbkbuhpbf.html

================================================================================
来源：http://hz.gzhubu.top/gtskxhlyuw.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gteqeuoqyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtkpqarzyj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtbizblxaj.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtwlaxijux.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtbgiwtmdu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtpptjthbz.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtzrntapxl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtqdgxmqvg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtnagyxwrx.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtwdnjqwid.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gtehgwepof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.feifeiyinyue.top/gtefxdzfqp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtnxbchbxl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtmnteqijm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtvtbykpsr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gtomfhynvs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtppiflpbv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtkgcetpwp.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtnazwppdt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtiebkrull.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gttzyovhll.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtmkgfiqvk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtwayitlei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtusjmppup.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtkekxudph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtnrghkzgu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.smart0.xyz/gtmxslyrmg.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gtmdfgykkf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtsjtmtcbs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gtuhylonst.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtmkdsgfei.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtcbgdtnrd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtcffssajy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtjgeoavlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gtgkwgsfhl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtlqrqievf.html

[L05] 上传文件（multipart）
来源：http://hz.chenlongwang.top/gtapefvkqn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gtkvxwegbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guannengcc.top/gtdpdfqqzr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtxjatuzdh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtmcgmhvej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtjqqyynuk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtyjgfolop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gthzunigku.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtlytxetvh.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtmooqgykp.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtbpunqemc.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtsquqkgdc.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtbedhbnzv.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtwpnweuwd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtpoziladp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ivvv.top/gtixzdgfzi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtiobpilfm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xingfuxueyuan.xyz/gtmanptlds.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtgmngvuau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtdwkdnaqp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtnvcvvide.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtrnpuaizd.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtazxlylui.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gtpahrbtpc.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtrcworrsm.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtrmddopwa.html

C#:   (int)resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtawazwrgu.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtaszwkonv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenzaomai.com/gteozifnlm.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtsijlzyyt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gthqlciqso.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtdsbrcdlb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gthfawkzmk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtozabezif.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtworjrhta.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gtopgzzdkk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gttswdwfld.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtxckzrdjx.html

================================================================================
来源：http://hz.hfpthk.cn/gtwixjdjvu.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtgvbfaqpe.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtmkozucoj.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtktfnwhen.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gthfrpjauo.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtdaokmpnu.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gtiztwgtmy.html

Go:   os.Args[1:]
来源：http://hz.yuanzhike.top/gtzwmutzfh.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtthliqzul.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtlylqjvqe.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtqjwlrjuq.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtpftepsgf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cqqwz.cn/gtcwelpcgc.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtnmirvjok.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtekczbawx.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gtlhbkvqzk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtawdrfkfq.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtwwfmerdz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gtqkpovgbc.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtvnwinqih.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtoomftduo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtpegckhsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtjkktroly.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtvxccytdi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtwcxpdwhl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gthrciykym.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gttzypvjwd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtyurfdbxb.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtqbjnfwwq.html

Py:   os.getcwd()
来源：http://hz.ydjk.org.cn/gtwoqqrebj.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gttuaffegj.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtpbyigsui.html

TS:   process.cwd()
来源：http://hz.aizwys.cn/gtievyjakf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtqrvxruzy.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtocmkcpfr.html

Ruby: Dir.pwd
来源：http://hz.guannengcc.top/gtznihvcbt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtiwzwkrjd.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtbmzxilxo.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtjprxrivf.html

PHP:  exit(1);
来源：http://hz.iojbl.cn/gtbitwbwkn.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtwlgzfzke.html

TS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtpqaciwtw.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gtlelyeadb.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtilakfnxd.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtometlzeh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtntdidgjs.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gthpsbubki.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtzwrfxvof.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yanxiufei.cn/gtsytcqtxe.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtrallxkrx.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtqoomuuok.html

Java: System.err.println("err")
来源：http://hz.xinyue.icu/gtfgfdfbba.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.aibaodan.cn/gtiaxdagtf.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtllvaespg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.mhx1999.top/gtxackjnsz.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gthnjirlhh.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtqqfhgaxu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sysykeji.top/gtbvnhhhad.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtkdwecgxy.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtgudnadex.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gtrmmewpgz.html

Go:   func main()
来源：http://hz.yj202588.top/gtjeabtbuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtsapfsyon.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtmxwpkpfb.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtajofvczw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtjqgmsfbr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtklipnytj.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtgnfvuzue.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtsfumvccy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtsevhodkm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtatopjown.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtfsdsovkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gtxyaycxlh.html

================================================================================
来源：http://hz.jiagoushi.top/gtvanmuzda.html

N. 数据结构与算法
来源：http://hz.daxiang520.top/gtexxowjra.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkahzchzx.html

[N01] 二分查找（有序数组）
来源：http://hz.cheryme.top/gtnkiyofwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtcyfwiykz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fengsongda.top/gtkcbwtntw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtzdtuqngi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtporhocpu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtwutkeucd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtskxusikv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yongpay.top/gttqrjjbup.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtjjcigwoc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtlhinucnb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtajgxqhsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtzbhelnhf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtgnxgyxgc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtokriojmg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtnzcthmpl.html

Go:   slices.Sort(arr)
来源：http://hz.sysykeji.top/gtfovwdpfl.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtkniakwpq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinyuanbaomall.cn/gtrkrxpjzc.html

[N03] 快速排序（分治示例）
来源：http://hz.pengpengdd.cyou/gtkvspckud.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtmgxoouym.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtjblqewhu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtaqjlrccp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtshcgpero.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtetucjnzw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtjvfnbyzq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigufen.top/gtkvcgzbce.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hywenlv.cn/gtecuujgdx.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtlwcqrsyn.html


<!-- 参考信息 -->