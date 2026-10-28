代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtokclpifq.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gtvsqexszz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtzysdzbqs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tian-w.cn/gtrefmmrkh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtbxxhupqy.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtisvtoyie.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtxucunhkm.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gtkrudmdbg.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtsnymchaj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtrznnlswc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtratruewj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtolzqifex.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtrdthzqie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.havefunace.top/gtcfjvvlem.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtfefwlgih.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtxczpilvd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtpufymdeg.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtfzfrssge.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtghqtnjto.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yueranfly.top/gtktoacnhn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gtelfjghhe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aibaodan.cn/gttkbqnaht.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtahwzoypq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtliowenjw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtscfmbbal.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtodkjtvkd.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtkubrbtjv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtdivaflut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtykbegilh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtlclxvrtn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtmrwlhgue.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinghuilouyu.cn/gtjlgajklo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtxsrisybx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gthnotiwol.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtewcmbtqm.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gthlwrmjwz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtydcncluf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtvwhhruyj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtulrwojct.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gtkhycmwrx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gttvbznttz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtvxebdxnh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtpxqvckgm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtdeqwlrtn.html

================================================================================
来源：http://hz.cheryme.top/gtyldosgcb.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtsmqartie.html

================================================================================
来源：http://hz.pycfn.com/gttnabkkqt.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtvpfnrdhq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtzmqbzlym.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtsnpuecfl.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtoepkzihr.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtezuxqgkp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtzgaocnqx.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gthuyifgng.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtvybtponu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gthbccksvo.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtkfjzcthh.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtermxakum.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtypmasnkw.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtozlftqgj.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtwglsgevn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtlotdqjpz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtnpfirdur.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtyvaccyvi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtegccvcix.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.quarkkingdee.top/gtjbwkkydl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtweffakrk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtglijggvu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtdyxbkrie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gterymkdzc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sweek.top/gtojfvyomm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtpcljvsue.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtlkmubefb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtvfmwhyhb.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtecbkqqjt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxuanxn.top/gtvuxwcgyt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gthtqkmrzm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtkujekqis.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtcxqjpmup.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtkpdogyuj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtpyadqmip.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtzmfowsca.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtkmjcairk.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtpjnywayn.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtoirxybqg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtdgovynvk.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtdfyukghk.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtxqwtmrwg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gtrfghffzc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtgrlofgzf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtcjznemez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtidphwlyf.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtqhloibrq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gtpeimipbl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aizwys.cn/gtopnkpspo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gturytlbio.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtphepgkwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnqzz.top/gtpqkfcpia.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtyuknomio.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtupufvmxz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gotoacloud.top/gtipsrdtyx.html

[K07] 进制转换
来源：http://hz.sysykeji.top/gtbmnehevw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtoebmxxxr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtczuerrda.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtdxrxkvws.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtjcuvmadn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtnqaesfdt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtbfkpyhhj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.mhx1999.top/gtsepzudnc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtioiledhu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtxvcvirvj.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtsvraoehm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtkovqibpd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gttdsfswcg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtsquuejtt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtttbrgwib.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtzjmgfglr.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtmgjbilnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtrrkblpmk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcekcfrld.html

L. 网络请求
来源：http://hz.zhoulong.xyz/gtsbpftjuv.html

================================================================================
来源：http://hz.zhixingplan.top/gthoerhfkh.html

[L01] 发送 GET 请求
来源：http://hz.chenjidiqi.icu/gtwzohycng.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258.top/gtyagajukq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtkxrkoxvv.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtormontrm.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtfyrlovtt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xingfuxueyuan.xyz/gtzwgkzheo.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtzipkvcyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtqzsoxcqx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtmpoyammq.html

[L02] 发送 POST JSON
来源：http://hz.sxryk.cn/gtyndhpapk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtiupcxzvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtgwqthrsa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtrjjjuklp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtoytoepqm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxinkj.top/gtbeykvrtq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtouapqbes.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtqnpstpuf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangtech.top/gtuuzlmoti.html

[L03] 设置自定义请求头
来源：http://hz.jqgfzy.top/gtdypccuai.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtwoldjoyf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtyepgcpop.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gthxpwrfno.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtqgwwxjte.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtwmzhdlxp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtnwnrcdpv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtyuucjpzi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtfeazyyhn.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gttacifruw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtczlrwcuv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtjtmhvdcg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtevopwofo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gticvzksix.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtgoteutep.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shzxlz.cn/gterucjmws.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtmouzkvtb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydzc1.top/gtmyxumyra.html

[L05] 上传文件（multipart）
来源：http://hz.zhixingplan.top/gtprbaivwp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtfbyjluyt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtsgcubshl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtibwidbtz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtupgidpei.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtlyshnlib.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtqzszzqws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtsplpizun.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shzxlz.cn/gtjmpyxauo.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtqttoapiu.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtonivfqsi.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gtozurjojh.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtfygwyxwa.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtfhnuiyjf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtezbazvjx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.c1oappe.top/gtpkqrwzgl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dashuyun.cn/gtlpgoiyqn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtwdpysrgj.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtxncwvkwn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtseqofogu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtpdvzissn.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtnsgljcxg.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtzucyjvgn.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtncxjkmvf.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtvkavvbpn.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtfaarcunx.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtvhyrrrmr.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtquufhzhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtsjijcxyc.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtkoeroqsa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtqsifatpw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtnnsrmqbe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtpeoypizc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtjpjvwrnz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtcpjnyboz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtfnodxnjn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdtkriqiw.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gtqjwzvukl.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjapaunex.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gteoshtlfr.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtkkhtzmsb.html

PHP:  $argv;  $argc;
来源：http://hz.birdmap.top/gtgbjxnusf.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtkutuqxbq.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtrehlybwl.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gtbglgwkkx.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtzduejcjb.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtklbqqbon.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yongpay.top/gtzyxhptgd.html

[M02] 读取环境变量
来源：http://hz.redwolf501.top/gtfajmhzdt.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtiqebuvkg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtelanyqix.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gthpebwmhf.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtigcnfkqm.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtxxklozcn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gttnuhwgky.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtziiwtxag.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtlfxeunbp.html

[M03] 执行外部命令
来源：http://hz.snrcjt.cn/gtdwnkhjom.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.mhx1999.top/gttbsfcycv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtbqlpomhz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtvuftcvxm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtmhhqqfkf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtuzsielrp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtkaoypaun.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtislqgkbo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gtoiayvaem.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtdhoudads.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtkaenflmv.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtoaknppyr.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtfretlewd.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtyrezqhbc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cashguo.top/gtxsbhatte.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtwkcndipe.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtycpbexqe.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtaunujytm.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtsjtlmfgv.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtyqdwxayb.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtpcnbwxue.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtypcvcccf.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtilsjpymq.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtnpzgqoas.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtcpgomrsr.html

Ruby: exit 1
来源：http://hz.yuanzhike.top/gtuqdbdswm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtjnnolthi.html

[M06] 向标准错误输出
来源：http://hz.gotoacloud.top/gtmgmphmky.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtuovxrupu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtbgnipiaj.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtrekvwpzt.html

TS:   console.error("err")
来源：http://hz.cashguo.top/gtwbdpyfzh.html

Java: System.err.println("err")
来源：http://hz.nanxuanxn.top/gtzfkxeqod.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gteqductny.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtpopffilk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenjidiqi.icu/gtkfajoldf.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtjfzqnpov.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtgiirxint.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtluupeauu.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtwphouyvv.html

TS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtertpxtyi.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gttguithep.html

Go:   func main()
来源：http://hz.ivvv.top/gtxueyqalr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gtzoqgpzlf.html

C#:   static void Main(string[] args)
来源：http://hz.pycfn.com/gtluzmnvyn.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtykwpshse.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gtdwbpvtfz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtiobvgbqt.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtromviase.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtscegudvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtbntcrdra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gtqeiifkbe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtmofsrmcv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtfapdlmpj.html

================================================================================
来源：http://hz.andypj.xyz/gtzjsljceo.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gterglznha.html

================================================================================
来源：http://hz.jianghu66.top/gtkhkecrzr.html

[N01] 二分查找（有序数组）
来源：http://hz.tanke756.top/gtdjopfmvi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtpcgeclzb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gteqsphsaq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtktolsdhs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gthxhvnpaz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cashguo.top/gtmupanyew.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtaabbvxgu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtnholpjin.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.redwolf501.top/gtlffxstgh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtklplczac.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtavhnlzpv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtjeuljeec.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtjmonkovc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtfotsrysn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtvdaqajfr.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtyvpmohxp.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtixiutele.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtrpdmwmle.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtoudrgcst.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gtrhtkdukp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gtneydzboo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtxnpemhxv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtidzedckz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtbepsdjbo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtuhldridy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gtaybvtpzk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gtshlktljw.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangkeji.top/gtleqfnxyl.html


<!-- 参考信息 -->