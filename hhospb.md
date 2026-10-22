代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2teitcrji.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rcjzwoie.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ilhgswbg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2kbixefkn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yuoeffjj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgqhgxx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yuwjyixh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vrnzutfn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jbibpxsn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dgtgusbl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gzgnpmbk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2wcrmrgqo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxqksxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rbzuvrsg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2dqkgnfbq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxxzfav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smxosmwr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zluwdlvm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2xbpbietb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxhhcim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgsgeflp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2putjcten.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwifuyus.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wdyzwchg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oruxgpce.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yiozjlwl.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qguuiwjx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2czekevqw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2eayljqyv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oegieaxi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ponyuyrp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxvkcprh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xvntkhct.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qohyzcct.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tjmgswbx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hqplcaxz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xjpqifim.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cujavspc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcrzprg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ngmvwrnb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atetdtua.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jsxppvah.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ltuydyxu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fckutwui.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrabgoqc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eicpudzs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yycdtzfh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mkfbesxt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2orknnhtc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ykuoqqoa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jjceixnv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ooishuem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zshsmjdy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxzeeulh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ftakayak.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rirrnduq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2njwhgyeq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mguiamwl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2czoupbep.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lwmrbtrf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jasaxrpw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zcfwjfou.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wcgmffla.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aykjcffx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2taxcrxyh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lifuenpz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ppewgkix.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kpqgnzcb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ryhqwjfz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xquxtywf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2acklbqgg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ahldblze.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gewhmjud.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jlzlcvax.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ypqtcdhs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ljbbwrwz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vboumzuu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hayjhpwp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2toxfkrgb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2pckyxudz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aquumlgk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aprzqmpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2teueswkp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nhjloebu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzahlea.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hxbuggyu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jdtmdzai.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ngjzbfjj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rxybjdcx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2isyiyfbv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rvxgsvqr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qlspctlg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hbyxyasf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtqdopd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lilbsshd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijxcpogt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jwlhjiir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sytrlotp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sggynnng.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bsrpkxpl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mcpgdrzr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcmsfrf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lkxhahoc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rntrvtpc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tlxivmon.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zevcnrof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mkajinjr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tadrcnwy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bloxgzix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vdvhzfbk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uzwixkga.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2etkcqaoe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2eiybvcoe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qoixhnzx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bmbcghod.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2otujirll.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lqrrkcyt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sbllzdmf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hizsugyn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hzskowwk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2suivwtqo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mfjestut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbosupx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dqfgxbeb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xjihuyas.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uxxaujrb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bmrjusmo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qilvxvug.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nkiwowcp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gjqkdjrv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cukxmrhr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jitmrlvx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wuvrfxwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xucavtoa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hhhtrgxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2eioaakmc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2irsyblrd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ilsiexev.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ejqtnppu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ywhakiqs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiprzhfk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vivuoqpq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvufoofq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2liuqvbpa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2douuldin.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sxshbrjn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ypkhskoh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ffhmypyq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dxykvjol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bruysxkc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2geoqfdde.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iymlapwx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2whzgubsc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ladztlfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lkinptwx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lekbcwdb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iutpldok.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zsfwqlsi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kaskzutv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fccrfpsm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rknjeooo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ovkoapzu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ogkpleow.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fsozetkj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rmuwgior.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ruhvhxiy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zbzluiau.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tetslbxs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pgvsgcds.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wwlazsys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyhhasls.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bavbsjoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqkvqdqu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2okpwydaz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kcyyjown.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cujkzyzd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxvmqur.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2arxwplsj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fpxulawz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gyalyjuf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mluoptgu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gkloxcls.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2iwjvuscc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xgpflzmm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ikhdmtyl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gzchweqr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bjexnako.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqkdllx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lcedfecu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ungkscqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tumyrkma.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vhoekvyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fwlumxnc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ucwgsfcb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oewhipxz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pyclgswa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mhisowkf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mdbessaa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yawqxowv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2alspwgtq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jbdoylfz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2izdrwppu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mbqabwey.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aojbnfsp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tbggsahh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qnlijwwu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rggphtto.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hqhtoecr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hlydmugz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gxbidpto.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kagxfnlv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nyhhqaur.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzrwjkr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pvmftnte.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aqmiqjlf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xitemhji.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pkxjttvg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2flzlbrff.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zfxnkugj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yucgsybr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xgyyjgcv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lmecawnk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2urcqbirl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rbuegtsh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cruovfyu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iuuetrvs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kdrwvxap.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2keqmstix.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dqqhhfaf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2grpmuswv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ducasogv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dtsmssie.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwujawz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2skeokfvh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ncafhred.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fwgiqxac.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2azrqsdbp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2andwwpyz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rwlixolu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kcgwvkco.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lzvvbuym.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2idcmsjaz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wyidthga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hswkbcjh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cglqhlhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srrhxqiy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fgqkiqnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdybmlsw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gaxyvwey.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikieopde.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yoeoxngq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbwuiny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mojngieq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eadeojde.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiayrham.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2znikjkzo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iivgfwpq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xfdyspjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nbkiufph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rwpyqsnq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gvdofxtk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2avtbjtqe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vojedstt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yalsfwtm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eajidogy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2igelsbxb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iqudwxmu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kmtquvws.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xcfbuink.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sttienhm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hadococp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zppwdaez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vabjmozn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ydaixjwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2witeuyod.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gewqfqmb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrwgvsb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwisyxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uyqhxjix.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sivhjwsy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kgjwfocd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zbqahybf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iijirhfr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nrejfpyw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ogonbwbl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oadvlygn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pkhrqzat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ybjipvan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqfhaosl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nlomtpfg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2onovzzkq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sbdhlcbs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvrvhns.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kvaepqcq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cjxxarls.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2edhjqjsw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjnzhupf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ebsrbvcy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2maufurcp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oiynkgbi.html


<!-- 参考信息 -->