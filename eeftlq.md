代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gtumztfvzy.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtitrwlxci.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gtbuxsiqao.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtdorksvex.html

[J07] 比较两个日期
来源：http://hz.chenlongwang.top/gtgnfcoton.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtqoqthfij.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtemzcyxet.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtajeanvcx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtjwrjrrul.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.mhx1999.top/gtzuzhwidp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtliseqcjx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtuzcavwea.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtlprzccfy.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtcavxhjnu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtmqaljkvl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtqhclenao.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtkcexhvwb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtknnupcnl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtmqaiznke.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.9152youxi.cn/gtvflhmveb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtgjoycbjs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtfbijimvx.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtbptjmxan.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtwzzphpgy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cucudq.cn/gtkjjdzggv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gttqfqtmrc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtuyquuzfe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtmfcoqqrv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gthtrlqywq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtjbamygcu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtuztneiju.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtgjxxoact.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtabqdnvai.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.feifeiyinyue.top/gtlkduyowr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtjozbkkwg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gttiaxdivo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtgbwlaxzm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtywcbrbpp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gtejcvvwdx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtvqwcfiny.html

================================================================================
来源：http://hz.c1oappe.top/gtxuwvzqge.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtnbwmrwzx.html

================================================================================
来源：http://hz.guowangkeji.top/gtcscypdpc.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gteqnrretf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gthhgmtfzn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtioydgupi.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtbtkxiwhs.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtucebsjys.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sufxvd.cn/gtvjcptbol.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gttiumkoag.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtwkldumhw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtzhaqxcta.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtlalbfgyk.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtqdeckhuu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtaeoajsse.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtyswbfxfv.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtcdrdjwjp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtopyydmwv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtzdtzieee.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtgvxdlmzg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gthexetzsd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtzglbrdod.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtzkvfoylq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtgopfockx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtzwsrljzn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtlgdlhepz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gtsmooqlys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtptcfxxbg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtlpebqtbd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtfpnfeodh.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtqfibvxuw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtegtjwegk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gttfamsbis.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtjqvvqxiu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtnuxytyht.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtbitwelbq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtwpxqdikg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtdrvmhpjn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtfjvpmcai.html

[K05] 深拷贝对象
来源：http://hz.yangfankeji.com/gtgougabun.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtngoffoyh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtzjfrumev.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtjmyqkgxf.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtnnrqclbg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtsfmpuang.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtfpwhwvmp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gtsnnsucam.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtlsfgbycq.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtcgnvalyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtbkopoyqu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhijiandao.cn/gttoohgerg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtjxfbmswu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtmafhzztu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtcinozutq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtptyhsutb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtjcmdnppc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtugndxepc.html

[K07] 进制转换
来源：http://hz.xingfuxueyuan.xyz/gtaadmcaja.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gtazvzmxsz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtmfgqpiht.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtwzbchfyo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtwzieimdl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gttwygrhwu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtsbylbvku.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtutnfkrrl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhijiandao.cn/gtwhuudbht.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtkuaubcmt.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtxykwxvgw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtzxjcvgnd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtqgradpnk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtjxwfqueg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtnvmvlovp.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtkbkogsxw.html

Ruby: Marshal.dump(obj)
来源：http://hz.hfpthk.cn/gtgtsvuzie.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gthunnfsry.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzukarozp.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtvfaevxof.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrzabqnxn.html

[L01] 发送 GET 请求
来源：http://hz.hysaishi.cn/gtvwaxbkis.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.316326.xyz/gtvbiviszn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtqxkrtosp.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtdmcuehfl.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtzhsgjirv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtgiidxxma.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtlsjtnehv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gtuobslrlv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtwqkjmbqk.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gttogcqavn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxuanxn.top/gttwivrajr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtaqfjfjkc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtmuetpcnw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtncektzzv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ehwqpu.com/gtbbumktnr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtbegmcasc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtjkefygis.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtihpxouzj.html

[L03] 设置自定义请求头
来源：http://hz.bjfxy.top/gtwmgugprb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gtpotaawaw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gtsbzcohhf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtkkxlmviz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtljmbkltg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtkrbusmbs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fengsongda.top/gtzsafkjvf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xingfuxueyuan.xyz/gtmxtvcejw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtcabvdztk.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtlbcfwpka.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gtkopqdriv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtwrbzxauo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtfaysvxfz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gthynzmkvb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtqauuxxbm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhengqikj.top/gtmcrztptj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtpghfaixm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.bjfxy.top/gtnwqjvbwu.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtpnvihyor.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtetntcluo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gtkfdnpujg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtnvpkmypd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtwmyxelvb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtcrshmspo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtxtohtcpf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtxbqcsvhu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtkyqxkfbo.html

[L06] 解析响应为 JSON
来源：http://hz.wangdashe.top/gtoxinctkz.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtwycuncot.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtvnhtfczq.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtplktijrm.html

TS:   await resp.json()
来源：http://hz.guowangkeji.top/gtrkebtlqt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtfyigndur.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhongyouzk.top/gthslyimhp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gterjwiswl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtwqyfpgko.html

[L07] 处理 HTTP 状态码
来源：http://hz.bjfxy.top/gtofulmiub.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhongyouzk.top/gtfpamdpoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtskujwenr.html

JS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtyxuugbts.html

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtuaiatqer.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gthireibqc.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtsdewaiwl.html

Ruby: resp.code.to_i
来源：http://hz.zycfv.cn/gtzkclacld.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtrxbdfegc.html

[L08] 并发请求多个地址
来源：http://hz.sufxvd.cn/gtdfoqzlix.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hammf.cn/gtzttmeisp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yvedp.cn/gtlbndcxmv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtrullzbew.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtlctkxkcv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtuhqeuvkw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtztmsdzbh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtgrzvqmfg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.meibo888.top/gthkgluqbj.html

================================================================================
来源：http://hz.zhengqikj.top/gtsnkslfjf.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtdalsyjpc.html

================================================================================
来源：http://hz.zhixingplan.top/gtqjyjzmmg.html

[M01] 读取命令行参数
来源：http://hz.shangyingyoupin.top/gtptomgnhn.html

Py:   sys.argv[1:]
来源：http://hz.jinghuilouyu.cn/gtprdidtyq.html

PHP:  $argv;  $argc;
来源：http://hz.hfpthk.cn/gtdkisinlq.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtupykdedf.html

TS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtzgmiokgm.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtvcaqanxx.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtzkqxfder.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtugvlljjs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtbjkrpsoz.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtqzayqgks.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtglpdgegr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gttswjouee.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtpfljjbsf.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtmbtakcui.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangtech.top/gtanuyfsil.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtcbgaxucn.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtleinbosa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtllhrmaum.html

[M03] 执行外部命令
来源：http://hz.cashguo.top/gtxbqlfulj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tian-w.cn/gtjvyjykvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jiagoushi.top/gtooqpmdxq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtzfhgwper.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtdaxnximf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtcucznfvd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtnfwsxexc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cashguo.top/gtbunuyifx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtgpukyfne.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtogxpxmva.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtpifklrcv.html

PHP:  getcwd();
来源：http://hz.yuanzhike.top/gtfihgoovm.html

JS:   process.cwd()
来源：http://hz.zycfv.cn/gtgqhwznqb.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtnwkujdug.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtgpcjfuuf.html

Go:   os.Getwd()
来源：http://hz.c1oappe.top/gtsagoqkzb.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtwfhqnjxl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gthnduuqjq.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtrlsqidkr.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtiraqxgky.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gtcsxfzcwx.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gttcrngldu.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtabrehhgx.html

Java: System.exit(1)
来源：http://hz.guannengcc.top/gtisrdrxut.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtexwutjli.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtbkwzkrmm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtyfhartik.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gtavtslhhl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtroutmmwq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtdstbyefm.html

JS:   console.error("err")
来源：http://hz.shzxlz.cn/gtvkmaapeb.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtaojxdlzp.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtovnsetyp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtgejqhuvq.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gttvjaswbs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtnqhveudq.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtnslamrub.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtnnreopts.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtkfhbffnr.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtammapnjb.html

TS:   require.main === module
来源：http://hz.meibo888.top/gtawsaqqlg.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtqatoxrmq.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtguwbzdoo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtnmvclklq.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gtjmgalftv.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtpdljwcrf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtzuenllrx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtcwgaqdye.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gthkgnujpi.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtplpavhqg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtmlapjdit.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtrdxrjwfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gtsxtaxopx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtmlyzkhrw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtkpttsasw.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtjqgqfqpb.html

================================================================================
来源：http://hz.yvedp.cn/gttprlwxnx.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtjetmwdaw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gtrjqbugtu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtktowkjul.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtozguvrdp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtcyfmebpf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtjelsldoz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtxgncrmkf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtjqfwjoug.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtkgngflxj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtxphfjuim.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtdenpczpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtcrfgqzjk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtrfwfvxac.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtprrnzmor.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gtyxeutzmd.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtbgkfqayj.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gttdrfufho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtslypbeox.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtlmhtphol.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtyogpysej.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtgjjexuhe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtczjhegzs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtkwpwyddt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gttkxzeulb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtbmgvhkrq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtkvloepal.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigufen.top/gtjhlbhanz.html

[N04] 斐波那契数列
来源：http://hz.haohaochexian.top/gtyaayssau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtmyfolpgd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gtlpsscafd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtpwmecsrd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtzzssptfh.html


<!-- 参考信息 -->