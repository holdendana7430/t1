代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ryvdlttc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rjfbnfxd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jqryridb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zelsezze.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hhaxixbv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yxkvpewa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dkrxbplj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3hbonisbd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3yulqkblv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqqohpq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3sgpascjw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gofxyowo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcekcxtt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pxydkjtx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jfwkskjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rnfmcdgi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eagpswrv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xstwlyhx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3idggevjy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjwhogp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrqqilmu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wdbvuhiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukwzsarf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3fjwcglcl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nydrkrfr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ftrptgjk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mjelbrgk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehyeohat.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wdtuaqtj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtdmrhe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3idsgtizw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yavyerbm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nojvanmg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3irxmgfkb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kjjvhtng.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obfvxkhe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hteqjgmj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ljoohwiu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3beutwbhd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jchwwvzw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jecsomhl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tuyayjeh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsdopjt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uyenxcev.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqeyutde.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xanufvvl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjiretlc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbvusdti.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gojkqvno.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3huabkwth.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzfpouhv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cbjapzvh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lcclbszq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nhwvgsfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3umdvhrvc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zplnimwz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3alkfvwmo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rnfadtca.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ilxadena.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3nvvujvhj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqmgfcjb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ahebfpgt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jcfhxbey.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nrrkzpea.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3etvwbywm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3panbldgp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fphwtmgn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jrboccos.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3phjrqewp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aedywcmh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mmjhkuxs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tkgdgngg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ctfdebkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zmrrmjme.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3myqlkxmm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mbcowfib.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jzprjaxm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ymamdlif.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvhmfch.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wiisgudd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bgsfotri.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xprqltcu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3erqbtgpq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lnftmztl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vxxrdght.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uscmamcv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3loezydpc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fwsxingy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpfdrmhj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3offsmnto.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rdsdjxlu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3imftlikj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3teyysjlv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gctkvsub.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kihlecey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oepptlqd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mdvehinf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqbsgqlb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pqfukjah.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yyyezcvz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tgqylqkl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pgpklirg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3byqbxqpj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mfwfgbvl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yysncqar.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rfvogzmf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjqafzs.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qwwmzzmo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jxiwgekw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hfrsgiqf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3aqbhtobv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uwfywigw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uujqhyve.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fcnrqbya.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hxrgkkju.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ttdndpwf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fneyyaae.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3awspryuq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajenzvab.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lpdvibvd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ehmyvkzs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvoqvlp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3twplnspf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qpbwqctx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zbsimjzf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dgaprqcp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kiutttfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qiujeudg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fxhrwzrj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tfawpupe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3counfrrn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ziivgblw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3khyroqbc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iyaqqmxi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uqwsztld.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3afnoqwkc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fdlsvujw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hwhdnkbe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hnzwtzrm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ilizabgn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaogkida.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3snldlgjo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ffngzlpl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pmzubizw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gpnxkhra.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nzhcwaey.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3clcnmmlr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dqbezfng.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dywbojhz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nukdtkjc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3okxhmtbe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tmsrslkr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qcbbmdos.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tggllrao.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cfqhhprh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ghwymawm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dqcubtzh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hznqunwv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yukfwujn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pvyoyqvs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rwfkpozf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fjugspwh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gzujczwc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tzvsqvqq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3appybkmt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sgjrnvwf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fefiogza.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mvjuhqdz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pqlynanm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vrpcsaxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uafzdxdq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3puuakifl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdjadswx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gfwmyced.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mkbxhblx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zzmxftdu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dkighmtz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3brqzssuu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3orxhfqtq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qvkjmlbs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kvovqlga.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hnglnnqs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iysllsgd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eiepzeqc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jmuncclg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3avbjsxpd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kamvfapw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xqvqmczx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ckvyinwb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gaodrtwj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mspsnxzm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wzpawevp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lodfqedc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jovhtwjf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hiysnovb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xfmzenoa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3aqjbnxwz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dcomdcea.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ukcnhndj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qbgytbmo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gtphyypi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zlxjyema.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wohaqbrq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tfnfvcpe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rawirzcs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wwymxpkf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cvatlwcw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3guohgiyg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sezyyynu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ncrkhadg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dudgholo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tqerqxex.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvfmnrf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yyjwzvns.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ivajpuim.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bppwlcmr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcvlpnai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tfgjlpjm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3admkrvjc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tttukeuu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xmtwxlkv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tfggkbuf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyphahu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nfduhjup.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vikvdiiq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ijxfmbvv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ddklibym.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pdyqsrwo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bderklok.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vkhztgjg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dbnvudqu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mbxtsgaj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvxnbjf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lzvkvdfq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yxabtjxo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3foysdpyb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3djidjzja.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yjumifip.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zedfygmz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hysvdxlf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kukfteka.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qxmhftmi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3oyeqvcjk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wmdfgmuw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qyqdqlhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjoghtfn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ecxmihne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrudobdz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3whypjzfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3otaeyrre.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yhrsjkkw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3foamltmf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sauirhlr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnvkpjq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hpcvmbse.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ieueuthq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kijaprct.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vcliecss.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rvtuijyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qgaoxded.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkuqcxb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwosjwdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kgfbgovw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqdnncaz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hxpgcqay.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fxqkwivt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3euxwrxdw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ilqboaya.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zfmfgtfv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ikwkkzqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fzcckwgj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hmjylubp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mkzknvua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wbnlgmqs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fgzghefr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3efvnfbfp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqzootc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wosiyqgm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lkndcgap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ktbnlzwp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fvaddhup.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pcreqpch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tccmcugh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yrtgugea.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ohbcsaht.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bqnyggcp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3okifbcxc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzorgaz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3crdiyjdn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zvmcwcfb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mptoxtes.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ovlwptau.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3earaxbfx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfxzyuks.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yymhyfae.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjdxwnmt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdfylyyv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wmovlntw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dkfvessh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3itavpmas.html


<!-- 参考信息 -->