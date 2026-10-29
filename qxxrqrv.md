代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/ggobcqyoq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gmbncgfgt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/grqednmnu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcnhvpahl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gdgxqkgze.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gcbkidawt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gvtqvkzsr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwihbdwox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfnvrkpyj.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gmwshbwpv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxmukqdam.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gpivtqaaa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gxpetikdf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/guupcbhhw.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gmhjeabxt.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gaazblcpq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gozzrtaqq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gbrhrienm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwkvllw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gdvwytujk.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gwtjuoshm.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gmdlowxmo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gvzexjoor.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfvmaxmmk.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gqattgffv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gpanudrdx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gtnffdhyb.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gmgfvstgg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gnkegvpkh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gjgyesazx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gsidrxuyy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/ghufrvhda.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gcselnmfy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjyovyoqq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/glflfpmpd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gxmlblusa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/garpljnkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gybnsgsem.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gpahepifd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gmbfuicsa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gjspesxmu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gdxbciqnq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gilxrpakg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gntniwmkb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gzwvqjjrw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gdxyffwoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gpzgemiwk.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/ghavltiyp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsntbxdqi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gpmamvdeq.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gjclrjvhz.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gljnjvhvm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gmapzvgkm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gexafcmra.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gbcxymppi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gzyncckgp.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/ghavexdbr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gxgegjlqm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gaybznkld.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/glcsiggmk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gnyevvmru.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gkuyvbuud.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gumgbdfzq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gxnjcylck.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gyefkmjuw.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/ghgqsfvno.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqufuehcp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gkxczlyzg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxpmusyyx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdzcrolca.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gyxeifjaw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gfkadwqfc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gugapepxj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggobdknak.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/ghtkpjzzt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnvjptzna.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gagevxayg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gosfdrpiv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gnzpjkirb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gzzxcuydm.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmeihvt.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gwarjrkye.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gyrlgqhal.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnhferfok.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gjwftnkyh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gulymfwjc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gdqovfsth.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gfbijfphr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gvvbkjome.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/guwfzdfom.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gmmqqenrj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gxoqqbhlo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gywwsanar.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gbldkznoj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gjplnwkbg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqddjqwla.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gfnpedlfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/giqejrbgf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gshzcwwws.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkwfitrom.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gmnhoicrt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gadhxbtpo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gqcmujasz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/geitucryq.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/ghovstkvm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gzzxyhhht.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gnamryauf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gjqpebdai.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gxebpbwlg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gersvvrqm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gdjkyadgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/glihrawny.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjgyrzlnj.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gnuclqfzu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gediwluuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gyfjvllap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gelwwadwz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gwiuwhlys.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gtyijmuje.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gjzhnvqff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gjeniljyu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/ghvjtnsmk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gpiobgbsl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gmjewjixn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gjfilfojy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gflacwtwa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gxrepshou.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gbdjainzk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gbcfjmsnk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gwguvcppu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzausrmbk.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/glpcfpvpc.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gzyuzzsme.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/ghtwwigls.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gwfiliclz.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggvfamnmz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/ghgzmpccb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gggbciazx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gaqmvwrcf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gmkoflpzt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/guxpltaly.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gvaruvhmd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gnwmvdohe.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gxgruyiss.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gukvzrkdu.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gzwhjisin.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gcogshgkg.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gvpnnztqm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gyyzlnqko.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gufmkxini.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gbxvftqbr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gfxjpteii.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvpxxmuhm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gogtrcgyp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gbfsgqyss.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gzkcnqxed.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/ghstqhdva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gpiywlukn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gunrnnqug.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gxyajcdvh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gojgigvzb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gqpzfqdin.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gyawwrmnk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/ggrjcvwqz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gqubliclx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gkptjcmsg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/grvoqozkx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gtexeavhf.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gzramezts.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gqtlpgnlu.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/glrhlbnof.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/geupfgixf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gbhrzofor.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gdfqcspbb.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/ggguhtcyg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gzpvnasyn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gyseekmjs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gxsnxvszo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnnbkduyk.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gwwydmxzb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gjcpktebn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/ghmgvimxa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpqzdtzjb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/giyipochk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gkmpgdyoa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gsfxwedoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/guhmykazm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gcbuwqdqy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gzngyqijp.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/golihscgu.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gcdsewymu.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gxuljzdra.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghnekozzr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/giyccqjsc.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gfppuhzrd.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gzezfkobq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gcswhxkfx.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/grbqwoxhf.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjlxradxn.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gozyxhyxd.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqeuromja.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbscypzyc.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gskdasamc.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gctgwvypx.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gepzsfyum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gmwnzcyjx.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gekihucen.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/grcrwnikj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gtyjdadlf.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ghikwnadx.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmryopdzb.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gwhudklht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gtxwenhpo.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/glrhynqho.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gklpessil.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gfyorwjtm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gywbkvias.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gdsrsixgp.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gzubbbzlq.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkxxmylta.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gzkdqjbha.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/ghkvsctjf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gshgjtqhj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/giseylwtn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gebrgxzmj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gscfkcojt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/giirmmxjj.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gfivhkpgu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gxdjhprax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gvysoauht.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/guhgxjsxt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gebakyquk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gedrmpdaq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gioghztij.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gzbilcvjg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyrlyaflp.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gdotclpxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwhvynahj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gopmrzqno.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwevdzajl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdzxlwltl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxbatvbbf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmfndysor.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gelahttrw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkyiqxfze.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gpvwgvqkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grmgcyqnm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvlzktgjr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/graytgrjo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyglcknlv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gvplvjxzv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/glsqyvjaj.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gyyyqjfwc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gfjoobrrb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/grlftndwn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gerkucohx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/ghonwahhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxrsmulpb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/ganxjccft.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gdobqaazt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gusfeqzjb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gxjezyxqz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbvdzkowx.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gkswfuoob.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdmrfcodl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdijxxekg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwraltzpl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjgujhrvn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjmohmt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gqsueltlb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gggzvejqd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkpfwsdpw.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gpdwufcbb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gopvsfkcm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gwedjpxsy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/govgdlyyd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gmznuclsg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gyjgajdgd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grrveotuu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gsdkjbwvg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gdxobsvmn.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gkagajxdp.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzbiljkml.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gizmpscgw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giekictoz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gealqlwdk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gskirbmfc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/grcacwpfr.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gxlayayuk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gxuxnbhsf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/giyhhatob.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gjrrvyldk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gpsituvvx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gggsfigvu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/ggkaeyrbx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gdvfuysni.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gxyavdqwk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gbculkbnq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gikdwpyyv.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gwllesnrl.sHtML


<!-- 参考信息 -->