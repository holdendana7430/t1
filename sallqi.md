代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtbmkcxflx.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtivohjkrq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtccvevnfi.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtwzlypoze.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtncwdjvvh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtnvykciaa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtwwedyvgd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtfhwktkfz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtcoulvert.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gthmjjywma.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtqozlujxg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtjmtzmgia.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtpnwaxnaq.html

[J08] 提取年月日与星期
来源：http://hz.xingfuxueyuan.xyz/gtkmfwtary.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gtlafunxbj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtfdwpqoio.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtzwjoacva.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtwaxhahze.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtolkxtacn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtzrvnprbg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtxegtewva.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yuanzhike.top/gtxgkwwcje.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtixthnrnc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gteoxpgvtu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtsywfufje.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtgukybpox.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtcgvbgwcm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jianghu66.top/gtrfczqohs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yangfankeji.com/gtoubchwld.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xziqi.cn/gtmibovkes.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gtfrapvexd.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtzdigmavp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtkwlozmzv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gttpcixnof.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shangyingyoupin.top/gtkbatfeoa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtvchsmbsc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtfsiuclcx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtkhkipjsw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtwsykcxwj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gturtcvgsq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlonqyqxe.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtfsrzvbkr.html

================================================================================
来源：http://hz.cdnleiting.top/gtxocmbgpj.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtguhpgqdn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtxzimcnvc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gthehmjkxv.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtsvxxjdwy.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtzpnhtycm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtucoggrnb.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtycdramxl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtznbtoanw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtpmpzljyy.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtmvbkbubl.html

Py:   json.loads(s)
来源：http://hz.yuxming.cn/gtsmazdrgm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtijcsyxbt.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtpotgnzbm.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtvryuifqa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhiwuduotai.top/gtrdexxqag.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtuvxyuayr.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtepypubwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.svipenyu.cn/gtfmpznacz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cdnleiting.top/gtauhiofge.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtkpdfpzfv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gteljktomm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gteuwfbqxa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtafncpndg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gtawlmxgbw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtfzacdhyh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jiagoushi.top/gtuvelfunt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtgkzgxwzs.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtoevsbqhb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtytefdstz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuanzx.com/gtvjuvwqbw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtwsbqhefk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gthkatbipo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhoulong.xyz/gtzfrqedse.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtkwetoabv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtavzonqsx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtkwtwwgvt.html

[K05] 深拷贝对象
来源：http://hz.wangshuangyany.cn/gtbzfxfnjq.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtmcbeakev.html

PHP:  unserialize(serialize($obj));
来源：http://hz.bjfxy.top/gtsrwuebhd.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtglcqsomo.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtemhorprd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtargakvtn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtsuznzzud.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtwnkbqeei.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtrgpdoxjb.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtfdjtnqrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gzhubu.top/gtidjncfpr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtndyvheqn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtmkwsksjm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtskumqfxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtdcbkdwoe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gtgfponyme.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gttvnyegts.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtyrwqqtkm.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtuysmdxuq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtioejrcfc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gthpdvmamd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtetbjnxdo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtwcspembo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtjbjgygth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtyxucgfce.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtrdlfszow.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtonymmqae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtgsvcoart.html

Py:   pickle.dumps(obj)
来源：http://hz.gotoacloud.top/gtuxymqtel.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gttnurlzxa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtbpzeuwaf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtybnjhvpa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtmwwhxuwg.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtvfeacmeg.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtjhruszzb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtplzddjun.html

================================================================================
来源：http://hz.dianchejie.cn/gtwacdxfba.html

L. 网络请求
来源：http://hz.shzxlz.cn/gttpnynbiw.html

================================================================================
来源：http://hz.bjfxy.top/gthrxkposq.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtpuvqwlle.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangdashe.top/gtlvvgwgps.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shzxlz.cn/gtiacefjvc.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gturvxhfug.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtnhjtgduy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtkelcddzt.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gthsmdsqsv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtbikeghrv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yanxiufei.cn/gtsyozijmm.html

[L02] 发送 POST JSON
来源：http://hz.guannengcc.top/gtcuyqjxyt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnxiangtu.top/gtgtoooybb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gtpsnujsho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtzrhcdazy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtxczoezrk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.mhx1999.top/gtprsmnikg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtliokoozs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtypuqfjte.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gtjibyksxm.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gthdizgjyu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtnqeeickz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtaearuomr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtaeqtccjz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gttlufkimn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtclizxvyn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtanraxqmp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtogsclcpa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.redwolf501.top/gtsxbfjvmn.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtcxranbnb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtkascbtvf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtxxoeqmwn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtyapdzlcg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtqytqtwrs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtiokezojh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtqlggzxuw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hfpthk.cn/gtaffzcukg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtxdlvdjnz.html

[L05] 上传文件（multipart）
来源：http://hz.chenjidiqi.icu/gttfnyrnxd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gtojzfppsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gthjkporau.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtywcwlhbk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtnlnyreuo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yongpay.top/gtqbozwnqm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtjssvsoop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtixujevco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtbbxfjdrn.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtsfikphjg.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtkawouufc.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gtjqmgwxai.html

JS:   await resp.json()
来源：http://hz.cucudq.cn/gtkcsagoen.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtnpoqqwko.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtnurgtpsw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtmixfzwde.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gtmulunjiu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtffcwnyqt.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtwurvncul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtnafxlkyk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtncopxwrb.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtehzwyhes.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtugcgafdz.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gtalydosiz.html

Go:   resp.StatusCode
来源：http://hz.52xcode.cn/gtozuhxwor.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gthdorejar.html

C#:   (int)resp.StatusCode
来源：http://hz.tanke756.top/gtjsvnmoml.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtkilisryt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxinkj.top/gtrrqgsggv.html

PHP:  curl_multi_init() 系列
来源：http://hz.tian-w.cn/gtmremmzqw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtayhniipz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtnxnbartl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtafjgxsuk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtxdsgygdn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gttmbvyiwg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtxpylxpdm.html

================================================================================
来源：http://hz.sysykeji.top/gtiyodxhwb.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtijocmhih.html

================================================================================
来源：http://hz.ydzc1.top/gtnzfdrbqo.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtjakgpzdv.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gtzmpmzpna.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtdowviqih.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtbqfmsmxs.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtxrpkthta.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gtfaxxdwix.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gttccmfomt.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtvfkoaycm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gttiyejknt.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtxqfljgyt.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtauhdhwwp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtebrhncfw.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtyqjnfiog.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtyecfondf.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtyyrkityw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtmiownrzq.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtukmfagon.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cucudq.cn/gtfhwyeias.html

[M03] 执行外部命令
来源：http://hz.yanxiufei.cn/gtubetvtib.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtygksdyay.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtwnacymir.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtwvrtekxb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtoqqvojqd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gthlbfjklq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gthpgoxcpp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gogol.net.cn/gtbilvhscj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtlpgigyta.html

[M04] 获取当前工作目录
来源：http://hz.xuanzx.com/gtcnlkahhg.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gttfcybefb.html

PHP:  getcwd();
来源：http://hz.yuxming.cn/gtrrzryxcl.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gthezjwdyu.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gtiluxdwsh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gtydzxgqkh.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtczzfbznw.html

Ruby: Dir.pwd
来源：http://hz.zdqjudy.top/gtpnvydcrl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtvgkbonqc.html

[M05] 设置退出码
来源：http://hz.dashuyun.cn/gtfdcvuppy.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtngdigdvf.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gthyegeehj.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtwlaezstt.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtfgjedoey.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtylibbqlj.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtqwzvqvtu.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtncmxtpoe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtuasyfvrq.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtvhjxxlzz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtxmbwsxpr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhaomingkeji.xyz/gtccwkiyjz.html

JS:   console.error("err")
来源：http://hz.yj20258888.top/gtpepqaftp.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtnnawsppz.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtrasdesyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtblvhsvlz.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtfvchxnlt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtvygppcxm.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtswthmfsw.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtbdwvzaas.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtsrrbqhoi.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtzmvzxvxs.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtfmyxmrqb.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtubuuftwk.html

Go:   func main()
来源：http://hz.birdmap.top/gtddgzpeoh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtmuxkktih.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtecllkgki.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtpbhzjtit.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtooqwfrkj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtymqpnbbs.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtonmljrct.html

TS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtbgtywata.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtdqwiygil.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtdiltwyor.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtazrfqhjv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guowangkeji.top/gtwssjavtj.html

================================================================================
来源：http://hz.yuxming.cn/gtjranlyzx.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtnggvtwlu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttvwczjst.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtdumpqouu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dashuyun.cn/gtzglybjrz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtgssjsyrz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtwmtumdou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtylprdils.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtqaohwebr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtrzgzwwvh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtvogqlmsd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gtnhmzvakf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtvxwkaxky.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtnzwtprdh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.vqdsnc.cn/gthlfhdjjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtwboxtrak.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtnpwfudiq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtnwlwzika.html

Go:   slices.Sort(arr)
来源：http://hz.shuidangran.top/gtpkawctmh.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtsivdvhdz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gtlysomyeg.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtzdbnepwe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtduutgwli.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gthoxigfnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtwakpnxte.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtkvpbnonn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtijaqizqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtpplmdeir.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shzxlz.cn/gtmsyapfom.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangdashe.top/gtkkyrdwwu.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtofkjhhty.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtqdyqgxuc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtdnfkpurq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtkprkwzju.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtlwgqjnwv.html


<!-- 参考信息 -->