代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtsdwaauzn.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gtqhcujbbh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtpgikrvnw.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtngpvckgd.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtsigekpnu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtitwzqypy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtpmqbmxch.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtrqwmmftn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtrpxegrvl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtyjzqeyqw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtfrpuizhy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtoysrzjyl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtaeumkfwe.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtkfwhzxuy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtxfehgqzi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtkakkaeib.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtnbdrzfwt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtbvokzwru.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtkyfukvuj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtolljrncr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtudxdwppk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtkpavogzw.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gtqhogeidi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gthpwoxiii.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xziqi.cn/gtvbeusdcm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtawlpgpla.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtgkandcie.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtodptxktp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtvhflxkte.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtpfpcsvrc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.quarkkingdee.top/gtgyiacdao.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtuygiaewt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gtogswlbrl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtvidhkbaf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtlfdlqtog.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtfjlmrlgl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtiuwhgico.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtakwpqhhd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtowxhecyh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtrndrgpll.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjohuneoa.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtnfgfvnsu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkndnnfci.html

[K01] 对象转 JSON 字符串
来源：http://hz.pycfn.com/gtsxumtikk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtmgvkzzlv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtcyqphwib.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtbwlutfjy.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gthgtzdvlt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtjbnlrzap.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtexhzhsnm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtdjholafj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtyuqrbzpi.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtvmfytjtd.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtovwupjeq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtvfayzflo.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtpkwusaho.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gthmjzqmkx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtyuevwzdo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtuzhaqnzk.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtlnmxmbml.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gttdhmqtke.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gttuxtmrhp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtrpvipmgq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtrjhmevhz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtyrjkjpck.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtikvsnxul.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sweek.top/gtytqkzpqb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtyrcmkacu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtpbextxek.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtgmqjyhex.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtntrdcwyk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtpjmwfvum.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtkmdnloix.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtdwiucszn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtmlfzlyfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtxkxcfsyo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtlnifvrej.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtdgoorlyr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigfzy.top/gterzuslrh.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtiotbqgea.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtealwnaxa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtjbhrnzel.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtmtgvrejz.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtqvhjmuun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtpwhypius.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.feifeiyinyue.top/gtbcwdibgg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gtjncobkuo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtjwfufofk.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtdkjutfok.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtdgqwyffh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtiogficro.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtgipdcojf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtcommlgdi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sxryk.cn/gtekiwqvjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ivvv.top/gtcygcajsi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtwxrdccpy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtvqlvobrf.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtpjugzmpu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hywenlv.cn/gtbiksgemq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yanxiufei.cn/gtgdbytvgn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtcfyrqzej.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtscrqoomv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtyfhjyfrl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gtnbtkhcka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtbyagjmhy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtogwvhsto.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtazokvfif.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtvdrxwhze.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtwhfefvwd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtlueuxwne.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtcrkjyqhg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtataqapnc.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtumiganfg.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtbbonzliv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtaykccqdi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvjicdlhq.html

L. 网络请求
来源：http://hz.xinyue.icu/gtxavrquef.html

================================================================================
来源：http://hz.ydzc1.top/gtonkcswhe.html

[L01] 发送 GET 请求
来源：http://hz.snrcjt.cn/gtxdefgole.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shzxlz.cn/gtfbawyabu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gteglskvur.html

JS:   await fetch(url)
来源：http://hz.jyoumei.cn/gttgwcqjsa.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtndnzkzyh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gtwomrizmy.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtamwudzqh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtlobzqtjf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtijiavhgj.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtnlrxdizm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtcufqfjtb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gttqsvpdxt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtsifefkki.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtcgwuadlx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtxfqlgfzi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtcgmgkcki.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtwprhcnyb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtchetomss.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtjuswmbdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangdashe.top/gtjcoxkvnz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtdbuyiyte.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtkgmssigo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtzputinjz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gthiukkgsk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtxbrsovua.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtejuufkbp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guannengcc.top/gtmmjfkhyz.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtmhxvyuoy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtmbgdyhbc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtiqvicadq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtypkpklsf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtdwfsotug.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtljboahqn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtwsnocrmk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gthpaotfsq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtvriwafgx.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtkqhjbpgn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtzddkagfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtwypvgtny.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gttlaztmin.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtqregmpgo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258888.top/gtgrilewtp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sufxvd.cn/gtgnhyrygh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hysaishi.cn/gtvnfnlmtt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtsmdxlkfw.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtlyfschdu.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gtemyhpcxg.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gttovwqyfj.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtijhidpsj.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtwvamttfc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtwhbaovxq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtexetglkz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtqorqoony.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtopnnennh.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtgtiddoyi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtxcqjcoyc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtnxsrbiex.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gttuvptonl.html

TS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtpofiuqsf.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtzrjbqgkz.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtwrdxgfvc.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtkpdhgslg.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtbqeynith.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtrffadfgc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtvuyrljmc.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gteouooqez.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtstdxduzb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtkcgkmxiy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtvixhozon.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dianchejie.cn/gtpzlordux.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gttaqajzsp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtxpdcxuln.html

================================================================================
来源：http://hz.meibo888.top/gtkwiinxot.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtjyoijezn.html

================================================================================
来源：http://hz.smart0.xyz/gtkbulcicl.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtaacbriwr.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtcpmxljic.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtnkjzdcwo.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtjwhkfktb.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtbfbbyhqj.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtzmywmxex.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtxrdcpyxi.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gteqgeiter.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtdfdaqubg.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtzezfnhdw.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtgydoahqd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtmjsiiweg.html

JS:   process.env.HOME
来源：http://hz.yonumen.top/gtwxbgnkjq.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtwduynlaf.html

Java: System.getenv("HOME")
来源：http://hz.tanke756.top/gtyhhxqyfb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.redwolf501.top/gtzqrdnash.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtzezicmpm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gtdkrgedlt.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtgowojazd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtahjizzms.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtnvsygtiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtafxnwycb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtvojuvqbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtaxzrfrcv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtvteboxcb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtwvqdkbcr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtikngbhdr.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gtqjndohct.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtrvjbewrn.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gthhemialr.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtbnnqnwkl.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtqcynzvre.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtgrvxsvcn.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gthyubhasz.html

Ruby: Dir.pwd
来源：http://hz.yonumen.top/gtsmlvmknt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zdqjudy.top/gtibrgevue.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtcdngdihi.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtgvlttoel.html

PHP:  exit(1);
来源：http://hz.pengpengdd.cyou/gtuamyzyzj.html

JS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtgsshhqbh.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtskiiwzrc.html

Java: System.exit(1)
来源：http://hz.cdnleiting.top/gtsoaoqmvr.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gtbbsmutch.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtqubbydsu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gthgytirtx.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtoqihjeux.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtisfsofxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtxtyrvaho.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtkykosuct.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtygfutyua.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtvxdtbbrr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtxlfjnkwi.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtfecovhix.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuanzx.com/gtieswocfk.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtfdyrtaly.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtmmbifpdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtyayvfvsc.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtceqbgevq.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtscscaifp.html

Java: public static void main(String[] args)
来源：http://hz.sufxvd.cn/gtykxmpxcj.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtgsupjvhg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sufxvd.cn/gtokkvktlk.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtvexxvvxk.html

[M08] 获取系统与运行时信息
来源：http://hz.ydjk.org.cn/gtkxsiunva.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxinkj.top/gtikhqwjtw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtsxnahznp.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtspwhhxlb.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gttyuvtcqb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtoxlpwwlv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtesrnbrcv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtfssmxkvy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pycfn.com/gtarywdqlm.html

================================================================================
来源：http://hz.dianchejie.cn/gtyvghherk.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtwfodllxc.html

================================================================================
来源：http://hz.chenlongwang.top/gtmsrjuomg.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtmjlyimuf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gttedhhqlf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtmjuiliag.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtpxbkhxzi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtbvwdjgbd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtppcodcwa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtlijtztbu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtrqxydbfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtnecydoiz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnxiangtu.top/gttuyzpvzt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtlfcrkqyq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtlfhewiix.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtbbuxkfdk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtxuxedsrk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shangyingyoupin.top/gtgpwwbuiw.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtzcknngvk.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtjbwlxkdw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtribymiom.html

[N03] 快速排序（分治示例）
来源：http://hz.aizwys.cn/gtgktdoshg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxuanxn.top/gtpdozyysb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtgeisdxas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtfheshezs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtiqfkftch.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtpxfrmgtq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtupilatmh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtvkktgfqy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtpzxeuyrf.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gthmfqpeky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gthexrjbjz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtcxzcbyeh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtldpwzibb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtihgsvtty.html


<!-- 参考信息 -->