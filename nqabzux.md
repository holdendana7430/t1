代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gtwuzobyj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/ggdrmwxzf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gqtgskkdb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gggycnevz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gbtmznbbq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gvnjlhwee.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gboadykww.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/ggyulosgu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geitbncjz.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gkqeczgil.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmxfcjrnc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggnecyzma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/ggoybovhe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/galbkvddc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqpqydfu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gtdkapvpp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/grrlpukdt.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gdfsnvurv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gbvomxera.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gwhmxowpa.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gespayllv.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gotvpzqqv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gheskocaj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gwyiymvdm.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/grrsudjla.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqcfoqlk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gyizqheyd.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gsfxoubcw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gowrfgncg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/groemmavp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gtojybvim.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gasobjnql.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gyaaqavkj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmwqyqthh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gznzfrpzx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/ggvuzpslw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gzasvtspf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gaeipspnd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gakedbtlt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/grysyvkzr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gjoqcdruk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gzneiukta.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gfcwvmlcq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvaybfvsx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ghjvwqlvf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghcrhvsyw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gqnjghlwz.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gdwtqfgqo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfyoqlul.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/glwgnqqye.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/goipplcav.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/glcodwhjo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gpkjenbow.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gxnbbpsjd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gyzwjdsje.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gjtwtjyvz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/guifwwtay.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/glddqhyti.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gwaqjilxu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gswnfcmip.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzwxxdoge.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gpzwnvnve.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gdtknevtr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gxnpktzct.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gabpcdiku.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gvwnydkpp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glnmzrkbw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/ghlncuzos.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gsjjnnwsa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gebprphlm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gvfsmznpp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gtrtsline.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/ghycgfybv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gxumtxwao.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gqnagckpc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggkmhzvsb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gbxtmmpbm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ggrwxblhg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gnrqilohx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gwyuiitvn.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/grarsaljy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gmzvhqkla.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvmwnhpci.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyuhwaxvp.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gbyjngkey.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdkzhpmec.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gdozaaiol.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gosudrlvz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gdxlwvpfz.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/glwiithuk.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gogpmywvu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/greonfdop.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gjggbglqa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gajocjuej.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/ggbbgnblv.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gnnjnqexj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/geabtnxbj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/guqpxkyuj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjyalrsqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjojbzooi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gobrddrtq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gryvxeivl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gpjltgyue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gpklbvfgg.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/guehjokoj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/glredhjlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/geofuwmlg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/grhroxzgu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gownuxhoa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gjtbninzb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/ggsimemjc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gmohridlk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ghbtrqkkh.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/golinecfc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gffxyzgsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gijzfjawo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gfalyttcb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gsdmswdim.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gibocolzy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gnmigaamv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gchpofcjz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gbsmpmygb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gqczjcgwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/ghfacdapx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/ghexltaho.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/grantfqtm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gpfhlgshh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gbwisnmyw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gicybdkoj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gdrsepgto.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gdlzymviy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gdtesijkd.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/goldlcgiq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/geudteedm.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gpojxcxlb.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggpdlhdrm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gxteqmnxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/griftdrka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gygzqvfim.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/ggbkvfsje.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glovcftsd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/giobrukos.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gtinzdthn.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gazjnktjm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxrcngs.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gimobladt.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gswjhzvrn.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gyzignler.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gwzobeavt.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gdlynhttp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gquxepqpn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gtlkoakqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/guvbaanom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gyolwreaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gceorxhva.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/glwruasyo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gjlyukhuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gwqcwkcbn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grnogqyqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gsdsynowh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geakhkpih.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gyxoneihr.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/ghgvcpbgv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gbgwoonmq.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/guguwfabr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gnwvgdfnb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gtixjbrwa.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxzdmogwc.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gadnlupnh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gpwuednem.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/grdsdhfym.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqkduccqa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ghzssdoov.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvudrfroq.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gkssbnnte.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gkwemcfzy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsinifceh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/glrryzpib.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvypiizks.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gqghbnusu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gthwogwpg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gxhyatmoe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gqpmpwqsi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gdynzdcao.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gqjbdvolg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gwdlzwkda.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gvevrncrk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gwrzcbgyb.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gievkelxy.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/girweihha.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gvdlvvdab.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjcayhztg.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkcrndaiz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gvrxsjrvq.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/grgdwzkfo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gkurqcqmt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ginkilmcj.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/ghujnxjqv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmqkbcbjx.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gxpasxvtn.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzmpeurqf.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbdlnzntc.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvaheczjw.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gupdtfvnf.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gelpgysym.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gjsmrvzzw.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/grwijlzuh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/guxtwouua.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gmzcjayvs.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gtgrqfgfn.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ggrsvdsso.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfwxglypc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gxjuzkuov.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gogtxdppu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gfdglkmgz.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gbyyyudkd.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gtgjpikkh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gcockcpab.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gfaropmhg.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvougvvsb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gjtfrhsnx.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/goluupsoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/grotkbzgo.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gwgowshmz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gbwhmbcfg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gmwmopaho.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/glwvhgdcc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gtsjntasw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gypjnzvsj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/ggcfdowpv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gwmmzjxzz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gukwxmteq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gopfddeha.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goamukqhm.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gcshiwxqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxtydujyc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gylzwbrgo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfxkjzofq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/grbmcvker.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcfgjkjei.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gtkcglfiw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkzczturm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gaxeweluc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gsfntessn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gijijreoq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/ghffveiox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gkgggjlmy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gzceexctd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gagpsbqlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gelxabkae.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gbojjxrmx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gwtinodwy.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/grhppucid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gjxhryvdz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gfopmptjs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/grjywoace.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gxdyrzwvh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gfqifxvpr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/givkuxhgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gzgymcuag.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gktrpwnhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gcwtuacnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gblvgjtvd.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gqibxxfjn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvwywaokr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/grolfuhua.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gaymasuwz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gwcvhnaub.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gqtohvtgc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gmwdvdgdq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/guscjupyr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gquidrwfb.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gxmtxelkl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gmyzcoqrn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gxdracxrd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqfuhlnnv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqalhxkfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gpfdnidse.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ganmjwtlm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glvucueui.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gkrvomwpk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcvocomlf.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gzuzykpxw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gylcllwlg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfbreyakc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/goeeotpfu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gdvjhsrmq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/glydnzvdi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghsqpdpvt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gcncpfmcv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/ggobznbra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gxicliimm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gosotvkvz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gtfivuslv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gmmouzrkh.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/ghgifjsnu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gyhzsbwcb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gejrpxfvv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gwpjwtqia.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gokiwjxrm.sHtML


<!-- 参考信息 -->