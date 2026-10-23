代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3wcwdpoye.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3otjgrqqa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3cwefshvp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3iuaoxcze.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzdsywzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ouvtsyjs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3owuwkfrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ebzybojc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uswzhwaa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3snhjmydn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3pkluijtm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3psupznuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijqfygff.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ujcphcze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylhbwpda.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbjxmhzp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zayzubdz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wcdkfevp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xwbvvnpm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsfnaro.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jibnrtef.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pajlitvm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gbymgwgh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hjngqaag.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3kaicqquy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ksowaqir.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ehjokekg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jxubdsxr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjldpzp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vlpozafw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3afsmjign.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvlmqwab.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndtrcjoj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3mgfdhblz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iitqfcmt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wrrfvoes.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tftohzus.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtlpijv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzfxljfk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ucjohyhp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3tjctjwsx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dnnbcrcl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmvqcvls.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrgcttxg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mkroqhwl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gadrczjf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ztckskew.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kjwbhvil.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bohddbfw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vkiioesm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mjnzmdbg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vqxvnkai.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebvucxps.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3riqsesww.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtjpisd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3huncnwso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ioshzsrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fsgsawcd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jzexazvn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tkfetxrp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hedwtgpt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3waakyvqw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ykjmttzb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tafyismm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hplaiuav.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nxbtkzcg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fottglfa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bmfhnfke.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vdnjbizf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3edtloczd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vpnbpvih.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jerlmfxr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wepmtlze.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwtzzqx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3stmbxjrb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wkbknzrl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pftvfytx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ikynmixh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mompftae.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rilyhmqa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3unzotubq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oeevczjn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3suxywtje.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3bhtrzlfk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mmhbbrmu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuzdliy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dsxpyicg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwnnokzr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mrizdbek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rstsqnwr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ktyfmntc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rksreswl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hectzjvi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bqxsaegf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yozftovo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3itmogshy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3avszmrjl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ttktpgpe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sxvztlue.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fjiklepu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ulgxaqum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zbpjbuia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ubymzvfl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nicauzrb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oaqdiapx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iiqfogmz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3oxjvskkr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rflinidz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3oqfpieut.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jobgkklp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zpkvywqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xpkrjbxq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qetkpwwl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wqzmwqig.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mfrndvyv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nmhcrimz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dvilkjdx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3tmugawgg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3odohfcvo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jewgrdic.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aahvonkd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zybhlktx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3iwppalaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wikvemzp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uatjmpms.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3znksumcn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ljdnbnyr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zmmgxuob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3klatrngd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dxnyohpp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3riwhjoqn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rxxhgvil.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nhsgekyp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3inslktrt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3utqkoecq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yontbppe.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ckowzchp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrairjjq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sdxahpus.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3phthavlz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wcvabfvx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mxxinagf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3umnuuofe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tawuqank.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zgkevgpi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mjvnyclx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iwiywrjf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hsqphzoc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3larvdfwu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dhwafvun.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qggljxec.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3isyryvye.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ptpqcttv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hegtgelt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dlhuqozl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hbypwztq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bzcwltqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvuqleon.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3baaniopv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iowhbuxn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjgxrnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ctkvcufg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bndqnanb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dovgtwiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3renfrsrt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cbwpwqrx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qnptkmwj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xvezlftr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ovobpktp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uoaaowit.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kghsoszi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bndlqbjg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wovsipoc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jalgdoqr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cdbvyrvu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3detmebqn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gxlriszp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tczogsfb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gamwmdan.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dkbmkqag.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nswscauk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dkfriudh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lyeieemt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tgurjyhl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3buoetgbp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zyopikad.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gcbeejbp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zidhdbyp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ozkodzjj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kokibywb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3etmgsohc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3eoxxzyfz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ksvcdveh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3scatfpdq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3elnsxmay.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oqjcosun.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mubwkcsb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fdifudvo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yodrusvc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cnokoupr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qzmsgjzn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gdvifuhg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rvcxmncr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ytqwmdit.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfttfrml.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pbkcfxgf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mnzxhqxc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cuyjnljw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eybifzip.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oymoolat.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rhwgdqzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3syrygasc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lxugqjko.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qqkqjngn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hepykugm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sogasaef.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fyvcwusx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3eylnrpad.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wjgfptce.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rysclzrl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zxhmbzof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3adjayhnn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3btpehwnx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hiriytzv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wumnzvwm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kqmgmpci.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zskczdes.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ghllazzb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3saqatixi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qysagivm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hkvyyobs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ykiimqzm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hpftjepl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ancjadlk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dycnlgjo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bfeosujl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gkczbegi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srshgctp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yrqvbqvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxsukhsx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yrhqcpca.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3olcltkul.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zitvbrbs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rfnkwnua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gzsstyni.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wzizqbug.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmediyxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qhzbozic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhqzxlyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fhixbqem.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3obrwqfvj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cfrinqyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kmxrkebg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ffxzxtxs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vnidfruy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zwhkaysr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fbfwdanp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yhzzeusn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mbeltnek.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3krmewpfm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vsnyyegp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yntiyovi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tmqbjilp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bunjygfl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rmzubrgw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vfzscgnf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jgkpnbfj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ohwkgura.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xpgxwque.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ezzdzatx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmgulac.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3luiayfyi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwynewjh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ntcprbik.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ldfgqvhu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzetmqcf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ffjomiai.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zybqptdv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eubsqgup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xowqehtj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lufzfqvi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ugltidvv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lmtfeold.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3axfchnim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrdtcyb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vptmrysa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ayyszmga.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iejweuyv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mgxxymlx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kosoisps.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ebioikvd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kckkqore.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dvlxeiss.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xbsivdej.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pminkdiy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zbfgcjtb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zplsbhvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3doocwzcg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kiaibypt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uqnvyvuk.html


<!-- 参考信息 -->