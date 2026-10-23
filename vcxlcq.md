代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3lxbxtvzf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gldhwbry.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvvnqj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xyjzsayr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sidgashj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nuwidqvi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mlhwatds.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3utsfkpnu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3efhlejmd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3hokkektz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jcnlgvwx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnytphwv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3frulmnnv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dxfawadl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3cxtdtzin.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ukltroiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcnuamhf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3twloelov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozfytnnt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khsazcbk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qaaydbom.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3enwrkola.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ieuzpcxx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxmiudn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ayvdmrcc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3grmdnqcq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wjvhjpmx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iwkmnuum.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3plpfybio.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gvscfmdb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3irtcietk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mepwcxfb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3logdgwog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3glpbgsvy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nbrqpxdr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tsaboote.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gfkophss.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3cbmmmvwv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3swcoywzm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cedjgoss.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tetvthaa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmicngtv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lsqyahtk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vmmdldlg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxgjxazp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ovwuaqbj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kgbtwrso.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3laoxwfom.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzfuxra.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3urgocbgl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bvzjfyjf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kzvembvm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kkuisauo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rceejamz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyalgcbf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3adudlfcs.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwodeqs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xrabtaov.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aaxoqlgx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnaawlmd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xdnoarvv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3sfvtbxkj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3suvnjhhq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wqlkgzfi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fagrljov.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zwncybsw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kakudnbk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dxhvsnau.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uhsxbhyt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dtfxzati.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rpyyfaxd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3erjyebdi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dpujayzn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cfbvyowd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qovhdfun.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lagjtvak.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ozcmcrhm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hhnwkqoo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmcfdzq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3makbkiig.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hklictvf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vewgxvvw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fcxniiha.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhetdhti.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3okcemmpq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ybyeoefg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nreomytn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wxkuyisw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dzyelycy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdlurhsn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mevojtra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwlyiqpd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yxmwrjam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uszvmyfl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bwcvnbhu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gjhtcosv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tfxwwgjl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3akllxqvm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmrgov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iqkwxang.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hjsumyoz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lnrjmfzp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uehckhaz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ksofbsrm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ykcsdzra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mevizqmz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dodcplcd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3oqrymwii.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3chsbihbi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ppjahlfv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bnigjnrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvzgwylc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zjbsrqrq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tmkbvyie.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pphpqhho.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fhaaynxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wwojhbzd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3uwifkeoe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gmyizmzr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xfcqcbfk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3viaxcpil.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gkzezacj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qvmgfvpa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bjyxovao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jhlreiat.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3drsfxotz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ohedison.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dhurqfmi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbiqefr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wncuooby.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3hpyllgzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vnqntplj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dizzbikg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pylchscd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kuwavbzv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3yxzaxcyc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdwrvknb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jevienfh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ieuhaicg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mgfawqeh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zuktswuq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3thnscjty.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yvejfodl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jvhhsyoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3squczscf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmomnbp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fgdzduvu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uicarfsq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3endzilge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mzejkghe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3drvujetx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rkfqucms.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rujxqjvz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3rfmneafv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qhcjdpja.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3tubwukus.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ughkdcne.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lddfoxjc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zzxxacue.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gzxjkbwy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dcguphid.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3takdlksr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3caeijpug.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kykijbxf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hhfhynko.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yfkgijlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fukvgbkp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmwdel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yttrpjpa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gwyqxhtu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3clrzluuq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3khynkxlh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uznehhxt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uutzgkad.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vtdubbzl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ofieqorx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sslnikti.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tlzbvfzq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iurgdcdw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjhquerw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3glboiafs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zhcnhhzh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ivbhvczd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ssmfatas.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3taurnxir.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3crchrmhk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtiqojf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vybkydpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ecdmrueu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cqxtvhyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nbhanakq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xaeurmtg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oiumwnrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3izzaruhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dvetozpy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ciuimmmb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3woznrtop.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dxpjytjf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qikvxdcy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3reztswnz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cbebdsfh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kblbnkkg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwaynv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ytfgauye.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mkkbanzb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3scimthft.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rekvlcvd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fwbtrdcf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dnvvxbtf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzeuyapv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rzturigv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zptqkqru.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyyyixcd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yiwbxwgr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xyekdqqc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iagcispd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rrjlpfcs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mpxylhky.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kzgzchyv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cfdyszpd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nrvdijmf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wqdxxxmc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mlnxhmrb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lqycnowm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ondzmobi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lkvdiiuw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3padqtorr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kjkqqclc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rdhcdkhb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jqefqbid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mawrpzlf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xyukizpd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mlldostv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3juowlweo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gdeexcrn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3metmhnbb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zieiwnbc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3btvaxjqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3puyckuba.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gspouthk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gsiqmsgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzonxhgv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hqfgfibi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfxtrpbk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lbtztkol.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dbxadsyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cnymajll.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iyoqzcml.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sinofvby.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyzsizrw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhhwxbi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jxzmgyol.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvkbbkr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mzgrrsoa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dnelqbpq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vcpzckjf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zrrnqlgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzixpzse.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rntnarnj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfnhlbze.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ydquuuzz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vmwmtacv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yszkaldy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zyuebeea.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3orpwimwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rreoiemt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lztteywn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cyyxflzr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zodztbve.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ylyfswpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pqbzzmjo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mgltkhts.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxiiakt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iucixggi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3arettdap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pommkngf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3khvjgwef.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lodyvkmu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbebxfbg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jxlhltuz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kpdwsbjl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmqfcqx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqecapr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vudxbeuj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lbioucqv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rnfmlfwx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbnmniml.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mixkdvup.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qwfdrowy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lchzxaen.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qbrrflyc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gwewfbpu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blfdcaxv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jkkbjxuj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ooycpmyd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xkpfiyhz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zdsntajd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3etbmdmzz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vagfavej.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pignxfes.html


<!-- 参考信息 -->