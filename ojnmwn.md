代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mfaagpqx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mmzdzbiz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfyqunxm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3igcqecfa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grievryp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gkvungbj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ceuntwfy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tzibrnqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwvtidll.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hrhziros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsfyemgb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adpdgdsn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fravvsnd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3buxckxuk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhqxgeck.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pujwmhiv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fmpprclc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zselwxsn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ywwtlpzx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pmwwkrar.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jacuwddu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hlrmqfby.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3emlfkgkg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3odmcqovp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3iiymwehu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sqcuzjkg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ishjmicv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbipnqk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfitwls.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rribridk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xexivoje.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tppptote.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3guxdaejj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zzxailkc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqkiafq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3kpdydvli.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3atlmaqfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3jsmymznx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3qjhksbjn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3crxzbjmu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3syjmktoh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wdozvlnj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3uwwothgs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3imdrubap.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uifijcsj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mafolfec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ugtxamuk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vfhjkgrj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxkdhus.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3awkbtqgg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3broostho.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nbezfega.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3drxyfruz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ivqqpaid.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3azlmwbth.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ujitcwvj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fbldddmw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tadtvqsq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzefyuk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tfkihyig.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hhksfxqz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dybnqmld.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3imrbmgay.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pmndfhrr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ursfnzve.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3taaiwalj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hiwvymoj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3viicduqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iicocqau.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ilhnyihx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzfsosp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fqewuyrn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wapmkzxh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qlsggmfa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kkgmzuhp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbefaeve.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wiwaaymt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhixfa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zrvzzfyr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ptrqcsxx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gntkbcwo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xtpnqsbs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3liuzdalw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpbrywcz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cnjnfjua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkpscvzc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3iubmulmn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3taazavio.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uvvrrmya.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3miwczrsv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sgyybzrc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pyufrvuj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aeioywhq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lhqtaeaa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vslxdpva.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jyvlbnir.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nbpfmcys.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bcaddwiv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fvjxirfm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wyoooovz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zfpcfnic.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rpefndwa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uyraoojf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3krzvnelb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ixqgdcti.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3prhjpbvf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oqaevyxk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lspiqkbe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dvtzsocx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bsmfetea.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qpxtjkgh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hgwyxvwl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oovhssrq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3iuqipoga.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vyydgpgs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ykodnyap.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lcvtlvzf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yshktzwy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3amazjcog.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wydblfqr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrgxbfy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3elgrhggl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ybqqbgme.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vflqqvca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rnhpdbia.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lcfrcqpk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nruzhspm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xecekjgs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jlraguva.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uqbgwhfm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltwaeaur.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3suiptodd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mwowkyyq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vvjfbdif.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ohfqfwds.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hhftgfqt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lspzvvmu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hqftmlpa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbbjdpy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tkvnrluy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wshsegor.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ajtwqdts.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ydsuwola.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uveajwls.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lmyxmcil.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dxeepfnr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ptnemakz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fngrpkeo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gjxoxhbl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vcmusneb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fvggciwz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rwmrfmij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hoqbsyaz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zjhanzox.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wodrbajm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jnqqjnck.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ggduckxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lfiyipkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcbdnbln.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vbhemlly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cydaafar.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tbmjvjaf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hnmrjzpz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nrqtwwkt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oftfhlxu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgedvpze.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3njmwvnkb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xqwbuqxt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wzyiount.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dnfdxbzo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uasdtqsr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3veftryvk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wtxsqwcg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fwpclloy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jfrfypue.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kmsajkoo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kjqpxexp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3osttcqzv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jtullybu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3efnyzdek.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hamgjjit.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tvswpfqi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3njzjdfkh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhvykm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3grjawujo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3unxrqtrr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3svvvyzoa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qqccqkwz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vubjnpjm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eolvrjdk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bkzjwfqe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fcgezoyy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3byzuzigj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mwqauqaj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hsxryncj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lmhcivin.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dnrksivr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zrrnkjoq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yiltlpxq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yuxkmihc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jhovmbyu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wixumnnm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlsryxo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3borodexw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ucjpcsce.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oporrtgh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ksmhstfx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uiwaryyp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hkwwrpnk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tqzbwitj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3slpszgem.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jvzzxutz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zpiyncjf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3annrvnya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qusrdcbl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tvusjilv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3imcnprop.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lvhpixoz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3awgloavz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3keioqbqe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ztxfmqyc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3itiuqomo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kjmrinwc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rrmyuwdr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qzmcdvpq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qldsykap.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iwmxwnfm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yvtgrliw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3awzcxicj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ameckkss.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lbfhpzts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3npyzqcak.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vbeszmlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyyuadcy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sndfwkks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxxsxkyr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3udjdsdxl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqavxjaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uwebblpw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cklyquak.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dnpqffce.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzkdylva.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xtogjtbt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nhtwviaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3czmrbdvh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xhvzeigc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mwptubbe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dtpqbtwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhtekkr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsftmmrr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbrdzms.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kekzemkq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3egayiftq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cvvsfbmm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fucimxxu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vsgdzmen.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yhbayzeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3snzbpdkv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rahbycyy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ewgvjjub.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bciwxzge.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pikrkjgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xatnlqyp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3skzahwsn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eejtmoas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hvppoczc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezsnjbvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yvqcdopv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaspaxro.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqnqlwq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eunhntfo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wealckgo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3leqjbtdo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwbjlau.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wvfjuhdf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xyxkxmfh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vuipejgl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qowkgnlu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nsaxfgef.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bydklilf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xsovcgsg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbxevfwm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yckjxuva.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jlqbqsqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dfjfgrgm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3karmumyw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kyklophr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdhzpmwt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tmdxcans.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3swwjzpau.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3oryofqvm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3haemjpja.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3llenaqhe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lxkwsxed.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3iyakkrur.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qbmwmbkb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wfpydyek.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfhbxu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rvsmuref.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3szpnjktw.html


<!-- 参考信息 -->