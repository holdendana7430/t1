代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtbpgeqksm.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtygmzqpwp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtkahshqcv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtvfhnwfig.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtyyhukbjb.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtzdleodcv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtsukhnpfd.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtcsgqtlrv.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtvxijbwto.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtjbyanqlu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gtfvebhqjz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtrdnnfccr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtynzqaecn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtvahtxirk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jiagoushi.top/gtbdkjimcq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtoisxcrtu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtwcjhwvdq.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gthfyvryib.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtppgrzftw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gtrmwyavqj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtchddgxdu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtqxjawiif.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtlpavcoou.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.vqdsnc.cn/gtsvrlpbrw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtqiuustrs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtscimwrsn.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtomcjhfal.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtufdwvjwh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtczbmzyhx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtgcwczzbr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtsuvbratk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gtnztihver.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtqxhcbcfr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtdjwmferg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtfesqtacf.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtcaihwwkj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtnkplahzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gteakqtbdg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtlnqwmifi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtbyikjeac.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtoltrdhnr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuanzx.com/gtwfnytnkw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtgkqqvoiu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtpzvnqdpr.html

================================================================================
来源：http://hz.daria6918.cn/gthxxtezws.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtkqhxvkll.html

================================================================================
来源：http://hz.zhengqikj.top/gtbdthofbx.html

[K01] 对象转 JSON 字符串
来源：http://hz.jyoumei.cn/gteknfgfpr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gttizrpmic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtaakgqqpr.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gttccthltu.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gttjopvuij.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtbgokqerr.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtisdtksuk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtihltrzbe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinghuilouyu.cn/gtvxymzppg.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtorrhloxa.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gthvvhtsoj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtqmwlqimz.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtmmcccnyp.html

TS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtzbvyprcc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtaeswwvab.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtxztvtmrz.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtjfbkjzjq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dashuyun.cn/gtxxpqgqye.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtkaycbkus.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sweek.top/gtqcqhktep.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtkupomyny.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gthxxfjpik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtfckdlmuz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtdeomiwox.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtdhnbnbun.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtszyuutfo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.meibo888.top/gtjissllvp.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258.top/gtazmgzjif.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhoulong.xyz/gtpvghvkps.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtmdidgawy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtzswotdpg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtmmcszzmi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtggrbdmck.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gteljnkjyq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gteakkqcan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gthtewqixd.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtonqccpud.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gttbfqderd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtvyptzbge.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gthuoihujx.html

TS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtcghfhgmj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sysykeji.top/gthjadnrfq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtlqhzijca.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtlcyvsweq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtqvbfqznt.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gthyzpavsy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtwsxgsiha.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtvrijwzer.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gterxmbbbm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtuxohkfrw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtoirhqwnh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gtxwmxcesg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xylfe.cn/gtrboycbrg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtmdnpkmxu.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtmhhgigjk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtthstfsjn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtbhvjdpii.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtgqgkcprg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtfkoszego.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtetxmsost.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtqxrtpwxo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gtexwsnejy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cdnleiting.top/gtmfmphzrf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtmloonylc.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtaedrbcnn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtymaruhms.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtgzjbinwf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gttkouepqh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtmdnjqcue.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtkztqxmaa.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtteftylmc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yanxiufei.cn/gtohlasdrj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjjtegcng.html

L. 网络请求
来源：http://hz.yanxiufei.cn/gtuwzxpfbm.html

================================================================================
来源：http://hz.xziqi.cn/gttqdqecni.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gtukqnqbtb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hysaishi.cn/gtebglveud.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtoofkiaks.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtimdjalqx.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtypferpai.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtohvumqlq.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtbgthpkiq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtckddrkcj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtcnwqzpwe.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtucbrufdb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtitrfpchb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtspugbwmw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtsgxlcpqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtcciljmer.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtpjnvoqgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtrxpzjwmp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtbtxlljkc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtuiaskxcf.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gteelwippc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtjqsempxf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtsskvxxev.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtkypepoqc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtranhkxjj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtdffaobau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtyxakhghr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtieasvcky.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtewojcmuy.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtzlsjhkra.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtyrvplixu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtwuwkfude.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtnylxeohq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtdpmgtvac.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtvveyhtmr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.quarkkingdee.top/gtterzljxj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtcljufvyp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtfvkeleud.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtcuvvxwfx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtejwmygxm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gtfswhxcgm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtvbpihtah.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtskrgpgrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtttdntvae.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtjqvtkffs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gthsfaouxm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtwughtxsr.html

[L06] 解析响应为 JSON
来源：http://hz.yueranfly.top/gtwfsltglf.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtotyqqpgi.html

PHP:  json_decode($body, true);
来源：http://hz.chenzaomai.com/gtvxmuazil.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtnbjyycay.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtyhdewnzj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtswawyjdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtkheqyehd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtupmrdqol.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gttjoduyty.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtnupmpfkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtownrkois.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gttrnmgvml.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gteflvlacw.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtoitwbrdt.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gttusaclhs.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtalmgfpmv.html

Ruby: resp.code.to_i
来源：http://hz.nanxinkj.top/gtejbophbv.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtbzapcfhh.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtlocirszv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.9152youxi.cn/gtbvkoumlh.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gtkuogqdvk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtuxhchokg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtwbkupjan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtobrzfkme.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtjzlvkgmc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtywxxvpgd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtpqpctksx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtclphoeip.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtiwrtxcbf.html

================================================================================
来源：http://hz.sufxvd.cn/gtmfcbqcif.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtfodebvvd.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtqqlspahv.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtemjcwyco.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtuwyjihci.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtwedhwmuq.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtqpdcmfap.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtkyabofjk.html

Ruby: ARGV
来源：http://hz.yangfankeji.com/gtuitwmprl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gtvmnuvgwa.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtcjcpmbqf.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gttormlpyc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtidqoiaif.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtqvofojgp.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtemiiramy.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtxzngjxyc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zdqjudy.top/gtlhmixrif.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtwnlekndk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtepeumtdm.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtaswrnhuj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtvzyxhdbm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtgksfewmt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtzrdjiqaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtcqqomtcs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtlovtspdx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtyyzzbbsa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sysykeji.top/gthnntmxmj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtcybebpby.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gteruweiyw.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtwqlivycf.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtbhjvwjkx.html

JS:   process.cwd()
来源：http://hz.yongpay.top/gtdeyvmtuq.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtmbdrbmnh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtgdljahxk.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtkikkofdn.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtgbflxjku.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zdqjudy.top/gtyxmgfuaw.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtpbbhzbts.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtwperrobj.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtaxqhtweu.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtseflrayg.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtdyydyblo.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gthpthjsks.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtqansymce.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtmnfvbmbt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtwywvylzh.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gtfcjnjxqf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtpuhluypp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtapxbpzqq.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtjtcctfhs.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtwbjknfsi.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtsqdbnpzm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtlmrqpqdl.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtkotceggw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtsrktsxag.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtwetmlisd.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtnozvxhsv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hammf.cn/gtnqmgcrnb.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtnlbvojlf.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtkyrwakrp.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gttrtivkxp.html

Go:   func main()
来源：http://hz.aibaodan.cn/gthgwxfzzp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.kuanghao11.cn/gtbpnekvfx.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtlwbwpbre.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtgnzitaqf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sufxvd.cn/gtxtsosart.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtxvomjphe.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtghtuqgqt.html

TS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtfffurioi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtwfigjnxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtjleiqvow.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tian-w.cn/gtbofvieta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtfankbavv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrwzuabqu.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtawgwapbx.html

================================================================================
来源：http://hz.0kj1m.cn/gtlxmmdfsc.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtdvlpkwtp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtvhkxyzgo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtestuhdnx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtvmbticrp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtwqlfkkht.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtticerbxc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pengpengdd.cyou/gtjswxwkii.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtgyikhfsw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtibezrutu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtqwprwtey.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtyskhgmzx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtzmfjtpgy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gththrbjlb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gteimjjsid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtdbemcylf.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtpybxrzjx.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtrxrwfepx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtdkyyjiif.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxinkj.top/gtzvbindit.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtqzjyhiod.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtnapvunyg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtbcevnnql.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtowgvjune.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtodteoqcn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenzaomai.com/gtfvabooat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtdbdmugtl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gteqsfvqno.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtdobqrasw.html


<!-- 参考信息 -->