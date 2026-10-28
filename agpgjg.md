代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtxxaxhlvt.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtydmbnxdh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtnixjcgom.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtyfuikoml.html

[J07] 比较两个日期
来源：http://hz.zhoulong.xyz/gtjbuthugo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtjkkofixr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtpzjojwgc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gttmpvjhga.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtiycgcdjm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuxming.cn/gtdswnxfzo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gthqbebygm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtfpqnhsrn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtspfzywhq.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtskthzqnr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtrjhyimyu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtnsdbzddk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtisixfutv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtwoqrvefj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtuagaxssj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtjamvntoz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtpfkayfnf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtprgshfii.html

[J09] 时区处理
来源：http://hz.mhx1999.top/gtztxzgjks.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtejmivjqp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtazkaeiol.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtgwmzgqqr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtqorcdpwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtacuxfzuk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hammf.cn/gtdqtkvoas.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtvkzyzzyk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtwjoimuta.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtssttnyxw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtiflnyrup.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtoygvcjry.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gzhubu.top/gtsqzuqmqc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtqmvtpzlg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtxkxclzgo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtkehpjzhl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtgiyllhru.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtiadytifk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtggpnsefv.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtogslpuhz.html

================================================================================
来源：http://hz.chenzaomai.com/gttmngxuyo.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtgjlfofkm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtyvpcczao.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtujteucor.html

JS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtberuvdrf.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtdkhuldgb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtklvxgcot.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtgjauikoq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtgwigezjh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gtczyjwllo.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtdvnlgfbl.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtaehybdsy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtdulwgqtj.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtmedmbltw.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtvqiypgpt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtayusfxes.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtisgymcgs.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtmzwthmqr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtbipbcxmm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gtafdgajwq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtebpwygia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtcdoesoas.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtidwfymzw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtuxyqmqdj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtvpglcasx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtokhewagm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtqowcfnpa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtyizgpuao.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtpkwrqmcu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj202588.top/gtpsbcnosl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gttbsaylzw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtaehdsemq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtoezcnacy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtpijpbsxq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gthyfamqqa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtekjfzlif.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtxcgxkade.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtmuwakkmn.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtdwjyzcof.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtqlnohjfo.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtiooxdedm.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtnrwwzzoy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtiuehjnwy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtgqzyioxu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtpgnbakrz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtdbvcfhug.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtdrutgkaj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtktaukhoz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtsspkedce.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtkvqqwbcy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtgekxpsem.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gthzqkmhmp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtdmdeijku.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtnvvlhnyy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtftuihiph.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtgwikdsyc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gtndmvndny.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gttqmtgtqy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtvqorzepr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtswympiws.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtcjichalo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxuanxn.top/gtseckgqiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gthdexajhi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtnfjlnenz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtfigwoxpn.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gterfbsekw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtqauongmh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gturzhnzrd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtnwxsgbqf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtfdmpclqx.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtkfgrwkss.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gthexpohwb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daxiang520.top/gttazgtvqg.html

================================================================================
来源：http://hz.guannengcc.top/gtwzeukmqo.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtwhpszhxz.html

================================================================================
来源：http://hz.meibo888.top/gtpgorjprh.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtstmpmyet.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtrajntfsm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtwldswhik.html

JS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtabchrkhw.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtjafgqbjl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtfknhbmwp.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gthnkziwhh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtqhbahiyg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gtapojotgk.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtszelfxfe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cqqwz.cn/gtjvkwmsew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtlwsasyow.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtvbfwgsem.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtnqhiyzsx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gtwiibwrin.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigfzy.top/gtorwmtncn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gttieryesy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtzzqrlwax.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gtxcsxbxxi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtcmakzgct.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yanxiufei.cn/gtkwtkgxif.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtrfycjwum.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtfwuwuqcm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hongshengwenyu.top/gtdblbysyn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtohecekld.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtsaeooywh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtksexeolm.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtwebthnhb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtlpoitwib.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtuybcxozu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtzoxhfrkb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtusachtsu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtxlzynoll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtasetiimo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258.top/gtxyhqoxur.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenlongwang.top/gtppghrxix.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigfzy.top/gtyklvqlhk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gtvmgrebqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtsfnjtcly.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtigowklyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtosppqfbv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangdashe.top/gtabqhneis.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtqaocsbpg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtqwsszyti.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtctpehlyc.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtvgxavrjj.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtmneinfuc.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtqrkrdjow.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtrjcszjnj.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gttxojrrza.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtcatxfvkv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtkypfholj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.mhx1999.top/gtjdyqdeji.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtwpxzumsr.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtefzxymss.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtqqkejmyz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtlsgsbtrn.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtivuwlsez.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtjkxgdsgm.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtcdxlberm.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtfvbpeetn.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtprpxdrmi.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtljacbrgg.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtqfgsalef.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtldlteqik.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtmeecrakg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtprpidzgl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtrwfkkuza.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtvkawtzft.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtieclnhzq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtgvmgpsqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtzupgddtt.html

================================================================================
来源：http://hz.yj20258.top/gttxozocbm.html

M. 命令行 / 进程 / 环境
来源：http://hz.hysaishi.cn/gtnosqvdrs.html

================================================================================
来源：http://hz.gzhubu.top/gtihcbegmt.html

[M01] 读取命令行参数
来源：http://hz.xuanzx.com/gtewalrgdv.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtybdxysbt.html

PHP:  $argv;  $argc;
来源：http://hz.haohaochexian.top/gtgfftqngx.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtmstfgwas.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtfemkvpyp.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtqublbops.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtqncghjsc.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtxdkbjlyt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtpynkuigh.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gtphmjreyp.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtadvmwhyo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtkzyvbgby.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtvarfqgbs.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtersstmhu.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtrsdnnxan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gtkfagmsxb.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtievmgapp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtuqcjvhhf.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtspkecxcq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtrstnkyst.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtfaumqcpm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtujgyzhpe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtywkapgnv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtkfmeozgr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtoqxznjuf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtkntsgnbl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtkfqhqorh.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtgzlibolz.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtylyeislk.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtjxxdyzjn.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtzzffwlvh.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtbfasxcre.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zycfv.cn/gtzmbkxrtp.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtdjjqugqr.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtywksffnc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pycfn.com/gthgwwmdko.html

[M05] 设置退出码
来源：http://hz.yuxming.cn/gtjxcvxatg.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtibkvzpcg.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gtwxbjcnis.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtrflajmmw.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtxeciwqjc.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gtwezrbuuk.html

Go:   os.Exit(1)
来源：http://hz.gzhubu.top/gttvihgkwr.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtqtofdihe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtcwcihzix.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtgatbtklt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtvlpegsbl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtagceqguh.html

JS:   console.error("err")
来源：http://hz.sufxvd.cn/gtqkcdacwl.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtgjbgunmx.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtneevwgfx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtpohgiotq.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtbdxbacbe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtdwjuthaw.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtdnsnwelx.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtsnjajflo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtyzmzpsfu.html

JS:   require.main === module
来源：http://hz.guowangkeji.top/gtcoqlvvhj.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtzivuofun.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtdqczfsil.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtxcjybgsg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtgafnfiqe.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtoqcwnejo.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gthlhozafa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtvgvmesxq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtiopshvzh.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtglunuxbk.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtlfomwgmh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtwsscatdt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtqsqxksyj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gtxvapmpwz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtnipgehgw.html

================================================================================
来源：http://hz.sxryk.cn/gtpoyqkewv.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtivubhepz.html

================================================================================
来源：http://hz.xylfe.cn/gtuenebnza.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtzyktvzhb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtcrgwcxub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tianlin.xyz/gtqplmklxa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtxmqcvnun.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtfdntmifo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtqjlpwqwh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gthpsjzzpg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtiecddskg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gtmkuuznhy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtopjzuwwh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtpicditkj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtolwesale.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtfatlwcxx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtgmqvqknj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258.top/gtyoeziell.html

Go:   slices.Sort(arr)
来源：http://hz.chenzaomai.com/gttubsxzot.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtebdbsbix.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shuidangran.top/gtfwxrytit.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtzqmcstia.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.redwolf501.top/gtuybnrqfw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pycfn.com/gtaybnvjco.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtuzulwlxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtzluvnwgh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtedeowxkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gttxbobfzb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hywenlv.cn/gtwmvqpzad.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtodljxyxv.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtarkthwsv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtufvoduug.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtsxjfaits.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtuphvvbix.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtwzuqbwwv.html


<!-- 参考信息 -->