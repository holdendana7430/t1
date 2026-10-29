代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gtotbilru.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gessmjdvd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gpanlrnhh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gzdnlivyg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gyluccmpt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gvecmwfgi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gnvscgwow.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gzevdmurg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwavcsugi.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gvvesghfe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdyqghrky.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gdttsaadu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gamirtajf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/goajifmcs.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gsqzgzead.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gigcwyixz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gvceqtddh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gihpjjbhs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gbvhjnaca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/grbtnktqz.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gpoypdgby.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gzububtic.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gbwujzozl.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gstpdsfzd.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gtyntgfrl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gvposrijo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gnkpmnugv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmnlhyohh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gygfmwrlj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gtyupyrpr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gjsugciuh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gnfhhzxhx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/giarktlbf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gwzsucuhe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdcftonat.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gsdlgmktb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gwfnfrbci.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gphpeqrdy.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gtftoqbuh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gvaoirdei.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gfiwsjjhp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/geanuimsh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gwfnmslri.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gbkzxjion.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gnhjrzvhm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gaqwbmtfj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfdaftxyz.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gagkoqxtr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gmdhctfni.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gzorthcib.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvbbglq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/grgzgljni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gkhwjueiv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gfwovqtky.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgslugl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gsdeqhpze.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/glkihmwau.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gakroczcs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gzmlvobpb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gyyoqkaoi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gsdfpnvbz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ghebnyfam.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gmtdhtajh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gnikukmwt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gegrhlegq.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gqrylqjro.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grlsxkoqe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/glrykzggd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcrkytvkb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmwopydeo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbtanywrc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gzgucaxnf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gbsumssfd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmkmqpvdz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/ggenwbtey.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gtugksecz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gzgoaipyz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gphnncnmo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gquwvbxcp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gvzjbqsix.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gufoyoely.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gojrkggqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gceintxbp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzahdfhmn.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gvmvkocqq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyhdvtjan.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gztzbyazc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gsodjlsqy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/guyjmupez.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gjplwoazb.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggfezjecb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/ggevxgdom.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gbasxfyyb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gxnhkuicw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gkzlwpwnh.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glquymesr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gbfwtcqnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gqqzijneq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gxaradeun.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gxuxzpmhs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gcjesihpq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gwssaljmw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/goaogebcy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gydiklskp.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gvwvmpqxl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gfraxnrul.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/grencjrna.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqfpbptpi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gfivbyylm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gscafemra.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gquzgific.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gzrnwayfm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gfoseszxu.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gjzfddhiv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/goomhwrxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gzsrllgto.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grnhikvfu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gzpiljhzu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gsbjqsxdq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gphuchtep.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gfgijkqai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ggfrqgcvv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gnpvxvtgk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gcdskzstn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gvlslqavd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gyunsjvik.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gxeinsmxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gujsjsxaa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gsfrwwamq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gtifjfqlx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsuflynph.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcndiydcc.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/grkyjfqyv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gealbpkdz.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gtjfbyzjk.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggqybwxvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gbigixbli.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/glgnmzbhf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gkyqbyezg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gkcqbqcik.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvijxzxnp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gkfedjhoo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/ghmzewbvv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gmonqupin.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gexhqvscs.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gotxnltfl.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/grrvsoyyf.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gumipdnhi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gapjkbniu.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gkxjduqof.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gxjofvmik.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gzmddjdge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxvizkxnr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gxbyhicaj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/glhuqthtg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gxwhqujpc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/grljmvuxr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbgtpzcvu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbwprwqha.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gskndyyze.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnnudhzgq.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghuyouhor.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gigslzkxt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gushreoif.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gulgulkuk.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/grjmnozxx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gbdngmrqu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gwrocrndh.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghnzfbuse.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gybtbgtft.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/guzmvqajm.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gwgpctkad.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gxkoloeyh.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/geenejxgp.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gdjqgtaqo.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gouwynohg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gohnujmqf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gpqpsdlbi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvbkjtiya.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gokjxwtwo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gkueawmfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gbxccehpn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gfzthwzno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gncwirhtl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gnqskgfeq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/ghooysjyo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gyriizpai.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/ghfwdpvdp.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gahfwqymr.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gmcquwavk.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gschgeanz.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gncqphtnn.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/grlivlxhq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gpdchfvfr.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gzyisatdh.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gzjyoklhr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxvwisqbi.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gqveorotx.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwtfoqykx.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/glxrzcwls.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbqokrjbr.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwznapcjy.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzlysjpum.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gocmvwqln.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gltwldupt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfsuftp.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gjyfxogeg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzdivhu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gnyuexycg.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gpopiumuz.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkizjawkq.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gckcbliym.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gypodajyx.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/ggjnwpwio.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gjimfxtto.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/grbfiigax.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gsskzovmh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gvjdoafnb.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gaetjllwd.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gfaewkeir.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpkhugsl.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/grhkccojr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gpavwahbj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gnnkqisaw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gjigkvhob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gvohvbtxu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gxycxbjic.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzthabqvo.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gusramcul.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gtjozisgi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/glsxkmwsa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gyujlsaef.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfokxeb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guqeyfhpd.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gzbbxgxio.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtxzbgaa.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/genpwxvnq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gavqkatig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gibiyzjqa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/guhxnxord.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggssgvaok.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/glcqtmxoa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvyuwwhtj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gutslqapo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnbspyuku.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gfsaiwcjy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gradgoneo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnjidwnma.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gqwvzwpjf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gqabyurym.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gcihzpvhz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gywtzrhqv.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gqsydtfwy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gopgamtbx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gmpplkmws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/ggofuzvwn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gzludhrfp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfgjxxhxg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjbyogscm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gskrdnbwc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gigunwacc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/guozbjpwi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbfzcig.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gaqepxidp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvmblosfd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzltaguah.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqydaelau.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ggxicwlxi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gljbwllgp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gvhcczfzl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gjwyieijs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjxowcwji.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gzuwbfndc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcctimuwh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gjypfxuii.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gpbaswljy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyeqpdjv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gdrsvokdk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gyfmqcdkm.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/guwlxkfay.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gobdzhxvy.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gegqadxdl.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwwuyrqnx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gngwagxpk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gudytlpcq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghltperds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gntipmivy.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gwricorxw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gwtpgyqxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gerlnhobz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/ghlxniqny.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gpjxhaudw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/glejgkyig.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gzdwugehr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gospqaftl.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gstlxpkbl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gmaqumqxi.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gpzrickzv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gmqjmkcuk.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gfsoecapd.sHtML


<!-- 参考信息 -->