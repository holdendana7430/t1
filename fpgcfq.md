代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hgvhwnao.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mynntnwt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vhzxmdzi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcerdbh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pagvnndr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pjvyvtmd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hsckiqbg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2grtdftbs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rloqhmkx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ngxbtztb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nfbpiusd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2vgwymrpv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tbughgnv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jpgettft.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwgnijb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kjgjoouo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2utcsijps.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zowvwgdv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wzyoyvxj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2suuldukn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seskyrls.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2onocindm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npkzthmw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hplfzwgm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2niqtuxqh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zvfdnyko.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2luzxmgku.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ssjrfybg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wusrbmum.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gootceth.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2iphlozfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxdtmsk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2egxwdhqw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlaqajem.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zotdmhcz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwxbhsi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zblixexe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2abovrmtm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fkocjpgy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgchocw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnazyug.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2byzlxgiw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbyhxwv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwjyabg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeunvsc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ougepfng.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rpetsjkv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ykgnntjt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2syrdztch.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gchqygif.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2eqqnmkcp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zzbbaunl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2byjeaztk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwvifqhd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bbxslsuo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hfquuqsn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2liprgert.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlmtibjz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kzdkjbty.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2depollin.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxolljbw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ykqbthdj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uowjbbas.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krvvtlne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jatjmdpz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2augcgimr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ticeyrwh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xfhlebdy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2iqivoizs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qxaxkbye.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqjvzal.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rktfxslc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qethlkvh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gfolsulc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nrgydoku.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wgkkefze.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cfxvnwyv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eiaxkchu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aoonidsb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2svwkefvm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cyqwfdbm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hiomhuik.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnbplgz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lbibixgl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2spyndbgl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2scvktgal.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cinnetpf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rknxiqvk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhdimmyz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jlqnqfws.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lcivhavx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ncvqsuui.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2sxkrfqjp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcaiwaxb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2totengeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhstamhy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gtoeqgut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utpcbgjo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qhcesxrg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uipmrufs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2luufsqvf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2orupemne.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eylfrubk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ubmqhjpx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ntpurahd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kucuukgg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xvyjdmkh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wuzpaqfo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ideoswwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2sgerqrpo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nxeqbqor.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lbvusjty.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gpccmwhi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ndhmhikt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rommhyqy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fcsdzomm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2nyuwmnzp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2aseqyfza.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hjpphnng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmervt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vfrkamkp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2dswarfot.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2csssudjf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cgkuhvmv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gehwzelr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bznrqvpy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vyufdxoe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2oufbzbbh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hvektwdv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2adonyxjn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xnepmaql.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wcpmkfxy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fnxbueyx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gsmjuydg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2digzdgah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2awdifbkg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gpkuhown.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2odnzehyn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kxlnsuyq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nuzahjsv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2onstjevm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lffmexec.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzhtfzev.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rgdujbvv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gecrwkxl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wdqtddlm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nllofkbb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pdfqsdxd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mimmrwzq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvzusix.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2skonkgaf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zmbisocx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wmtlcqnu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uxhtbduy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2anlajxlh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2npemnyjk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mxijxoze.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bjbvitcv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vxaekmif.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mlawaigg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ulavzsxa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lilguhwx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2yokzjeky.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lygchuzp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2babsfofa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hxrdlmma.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hxwhfxfr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qjhqhsbi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vpflseyl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mffqzism.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njbfnlvh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mkasxors.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoiiefto.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2igmnagrn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gdliwtpp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ezbarhpc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvplxsxd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqibnrij.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kcefaace.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2viwxtgjx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2koqraqjb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oywvavxz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gfocjpoh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ucchrivi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dkpkzvqh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nagnmhmh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2akpumhfr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uoyveige.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fichvckq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qhccbtia.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2txceppah.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xwvdprdv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bowhmaxd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jigggmsa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjkpjadn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgnzlfwo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nysnmpgr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rfcwwcss.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jawaaytm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jhztnsyv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hkzobtyi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bdyfvbgo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wlwowhdt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fyqljtni.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ydqbswbt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gjhasnzm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kgawqwef.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sxqkekuf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hgpflqdr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wlflbxgm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yetqazdk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ajfhjlct.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sqwipved.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iqyndppk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvkbjmb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yytjtgdo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ypekrous.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hklpzzls.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sstqtcli.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zpmbxrin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2awqaoefe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2czodfcja.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wkgbdsht.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2auvswmlc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2acvammzs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pzzvipdf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wdmmllhy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2aggixywk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pwpvaers.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2sttrtkqy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ihaanhfz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfosvt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2byaxlrmb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqoqlfm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2itkuqonb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbuewju.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kzxhcmyy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qdepntni.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gpybjuvz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2evrokstm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2geodeqta.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jkbichgp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2skmkdwpx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jgtfbvqp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nykqamkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsomfjru.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jubfurxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvejjjsq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yuuuvdbk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydwtxuqx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vvrmhsva.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnpcfuy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kohprola.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxivrmz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdtvwugn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gcydmvmw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqwcpduf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qkqgzqyi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zvwpbnvs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yziqqkba.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmdnuhj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2svxruqxk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vwvdrcai.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmcxwyxd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cjsmfwkw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vdgyiaql.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gdklscck.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gjuaupsx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pgeagjsk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fisasfxc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2utykwvin.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dlxtoell.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2byhrtpnc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2phnqjxhx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lqbasyym.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vrchnkuw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uuotksqv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwogfyya.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nbciwdpw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cbxqknnp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjgfneg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxlrach.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cpkjvzng.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cbfrvbdu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nzovrgrn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2asxztrbr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ijxsukhq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hnwogtjo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxhgxri.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wofqudyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zaykiyro.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sndjxmxs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlzizqir.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhvoqhiw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ozaiyewt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtptmmkh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ybhveknd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlyaumvn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yrzgubau.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ucnhuskn.html


<!-- 参考信息 -->