代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtexlseppq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtghdgccfb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gttjszcnxu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cashguo.top/gtpsbuhxyy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtfnylufej.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtttigjwjl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtajijulzc.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gtqibuiyrr.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtntrsracj.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtfhwsabgn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xylfe.cn/gtxixfhxtf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258888.top/gtemtjepis.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtrdjjyjxn.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtreteqzbj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtruybzfbk.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtmkaktyew.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtpbpfapfx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtenwlwbjz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtpyrpehpz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtujnozkfx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gthqzdvvgj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtdnkglvew.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtexoybwtd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtsutpbrho.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtjculthnd.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtvzpnkyes.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtpjqpgudl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtvdqrwcgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtnvplcqfa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtghkkhsmn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtkvojpzzo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gteaznempv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtdkqegxbw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hfpthk.cn/gtrtnbdffw.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gthkjkudqx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gtvmcqdtog.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtbztjldtu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtzangqbxv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtijkhhjym.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtrgldxbcp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtmkicmuzw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtjsdbfjok.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cashguo.top/gtvgpbaudp.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtcjkinjyk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtaorffxoh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gturzaserd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gttcgwmvro.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtwzcqzymt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtniyhcsaf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtavczqqzw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtcpxkjsor.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtteueqtvb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlofyjhmq.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtkkwwiibu.html

================================================================================
来源：http://hz.cashguo.top/gtpgpjrtrd.html

[K01] 对象转 JSON 字符串
来源：http://hz.jiagoushi.top/gtbiggborr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gteshwspym.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtsxsgkyfg.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtabctjiej.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtkmlyhfus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gturtgsnfk.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtukgccalr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtcagdxzqy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhijiandao.cn/gtcxvjzfxr.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtbvfrxwzq.html

Py:   json.loads(s)
来源：http://hz.hfpthk.cn/gtzkocshcu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtupcnekwm.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtxhsxqpoj.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtcxsqakkf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nwbrower.top/gttnpgtirx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtvucjcyhk.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtxsbybdpa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gttfvgzpbv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtsrdwddkz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtuqmmyhjj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtxnknxpax.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtpxglkfbg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtvwvpnlde.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtbhwptasq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtzbrnwfae.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xziqi.cn/gtlbazzoph.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gttegjghog.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtsrvnzowf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ybcxt.top/gtjrqougxq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtogzpfhic.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtmnzjtmiz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gthioroesj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtmcxhknwr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtvgtdqvik.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtlombwbwc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtjjvkwlbe.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtskdveimh.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtwjgiblyy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtxrpywvsd.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtzrbblijx.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gttceiyfcc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtfrkhhlig.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtnqsulhau.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtdwaafvdp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtgzdpebyn.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gtlhhbgzhp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtrxdvjpxt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtvrlljngn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtwdzsfzki.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gthuwvztpc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.iojbl.cn/gtuhpfqrhj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gtrliikiqc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtoubiltaj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtltokfywt.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtaxjzhtwa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtiehcbzgw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtinhebzkk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtvhyyorrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gthlfvgctk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtcemmpsqy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shangyingyoupin.top/gtemblvebl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gtuwoyzrsj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.andypj.xyz/gtshpwkruv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gttfnmnmri.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtcvxbqdai.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtvugjewmo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gthyyprtzu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtyihahvga.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtowewzyjj.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtzlflidvv.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gtxyoygcgx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xylfe.cn/gtfyksuvda.html

================================================================================
来源：http://hz.shuidangran.top/gtsaloedyc.html

L. 网络请求
来源：http://hz.zhijiandao.cn/gtyfvnfkiy.html

================================================================================
来源：http://hz.guannengcc.top/gtselgowqk.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtayqthxtq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtuuvjzjvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtprgabfyc.html

JS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtrjjplawq.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gttgvjvwyo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinyuanbaomall.cn/gtuccjaoov.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtiaprdgos.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtxjaezvkl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtncenlvuh.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtjpoaqhhu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtzwzxcpcz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtrcsplcjn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtduuhdecw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtkswcxheb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gtgejelhfe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtobuxkqgw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhijiandao.cn/gtacvcycst.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtsrouafob.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtejizlojv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtnxsvrncf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gtiqkgmlql.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtmycedzni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtajtynqnq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtpojvogau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtgyforxwn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtwufqqrme.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtcjrsxwxr.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtwpmhjkml.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtjarfvjev.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuetiantiany.cn/gtwgyqscmn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtrsagiicq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtxhoahbhz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtlngywada.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtzsvzrdkx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gthwjdwlrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtpgatfytn.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtmsxrqlfs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtjwzeisgt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gttbptnldu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtsasjwegi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtrsjnxaip.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtygwgkkot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtulunwbxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtuwpmcxgr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtdngbztde.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtxwzagwzx.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gtsyqhtrsd.html

PHP:  json_decode($body, true);
来源：http://hz.tanke756.top/gtxtlyhrjo.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtqbolikfa.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtqnokxlth.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtntclaeqo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtjacjnyxe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtmgsthggt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtbtcjnjhz.html

[L07] 处理 HTTP 状态码
来源：http://hz.pycfn.com/gtmvqbmstq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtrbcwgzhq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigfzy.top/gtmzpqcgrr.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtqhknvfit.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gthmsjhska.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtynxgzjeh.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtlzexfffv.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtblsunrix.html

C#:   (int)resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtbryhphqv.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtowzhrked.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuetiantiany.cn/gtbchomvmt.html

PHP:  curl_multi_init() 系列
来源：http://hz.shzxlz.cn/gtanpbdtmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtichuirpo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtvgvkeuqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangkeji.top/gtskfweewn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtomholigx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtcgjbmigx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtuaefqtnm.html

================================================================================
来源：http://hz.birdmap.top/gtaqohsylc.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtzxomndfx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnnotijre.html

[M01] 读取命令行参数
来源：http://hz.yanxiufei.cn/gteoriwygd.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtavxfzxxt.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtxruhktjf.html

JS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtjafpvjxc.html

TS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtzyzqcrrc.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtggoukhgd.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtkwxxlnel.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtvklkzdsn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gotoacloud.top/gtnlvmwxsp.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gtlyccwmnm.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtqoicgtsq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtlxuksiuq.html

JS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtinnijfvi.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtduhizmzj.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gtckqgzxni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtblzaaxyz.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtgekyccka.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtkhbjpttq.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtdtdlumee.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtojawyntr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.316326.xyz/gtcbsbvxzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtibnbvfmb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gttskjcnvs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gttbrqxapy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtrcpkzhgd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtjaynbszr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.52xcode.cn/gtltbqfmjy.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtsaexjbeu.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtnadfveau.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtnwayfcyf.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtvgvhvvfb.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtyegxxzkc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shangyingyoupin.top/gtifsrjdfp.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtgejjfimc.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gttsoyrqxk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtpsojozzf.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtwmcvmtjo.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtnobigqam.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtqfqyrgpw.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtjpzkndfv.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtygvgqviw.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtgtzpidmz.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtkbeglvqk.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtkvgybceu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtwcahtouc.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtieklgjye.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtxvfqidol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gttqqthllm.html

JS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtprqmeunh.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtbfnkvqjc.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtzdizscey.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtqvzvmqqi.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtbkxqhiog.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gthsydhibi.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtbcteneef.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtewpurjjk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtwpdiqdaq.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gtgufrqyro.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtezfijkle.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gtifkvambs.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtbqvkrect.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gthkgrpsqd.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtknsiqkwi.html

[M08] 获取系统与运行时信息
来源：http://hz.guowangkeji.top/gtbyogfzqp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtillkngtb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtigufxiao.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtsdiryqsg.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtqqtgvauh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gthmfcnnaw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtzglxobdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangtech.top/gtkznleakg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtaijkjfrw.html

================================================================================
来源：http://hz.aibaodan.cn/gtizuncupi.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gtwkghwvus.html

================================================================================
来源：http://hz.xuanzx.com/gthuigkrzw.html

[N01] 二分查找（有序数组）
来源：http://hz.xingfuxueyuan.xyz/gtfmncmgxs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.birdmap.top/gtzymtutkr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtepwruxtw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtmvetyezs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtdqvlhxey.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xinyue.icu/gtdmvyedda.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtpnbmaaxx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtzdxjqyuq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtgglrkccm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtxveqnxqj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtfqknehkr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtdpuqmrqe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtnqrxawue.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtzfviesil.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtnywlvtbl.html

Go:   slices.Sort(arr)
来源：http://hz.birdmap.top/gtmovvwwzk.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtwnqcjebp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtdcupvvjp.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtlsgbvffm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtogeqmudr.html


<!-- 参考信息 -->