代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gyxtpqvzf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gzmulhtfd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gihsecpxh.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gygvirwok.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/ggvcuayfn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gtgldagiu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gftsljmqz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjllgsqca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gmwmvzija.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gclpodhlm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gzohsfdpk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gdojnszma.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geirkilcz.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gytnzqnlr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmwifqaj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gsglgjrbs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gyhxdtuuk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gebfyglme.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxpibyjjw.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gbpspfjqy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gxqyyejhd.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gqzayyhjd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gdcrxyzpj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gnqfnznws.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gewpmvjgv.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gzbklksln.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnksrmesf.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gdtlnznrd.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/geauzzdzl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gfyybkkpl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gjmddcdbz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghbnumjwk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gwulyhloi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gluzdmhtt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gtmzkjvla.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/grtrwsfba.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gcenkjjsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/goaabwjdx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glkggeedi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gqkogsgmt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gcdzlmwxf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/guchjikhj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/ggxvsbxji.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/grdseirmo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/guetuaeuh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gchjmodey.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/goemozwwu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/giyfizbyp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gvblthnwr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ggljxfhzg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gpijzowai.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gekziziwu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/goyualsqm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gghzmfhfd.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gpawykebt.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gihucmcvm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gmwlpmvpk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gtcxunwjp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gpurilkei.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/garvdalea.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gsvyartlm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/ggrsgqcnf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gqlluuqkg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/ghyuoosny.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gqynchkee.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gdvwjzycb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gshvmjtdx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gldllkegn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gffaqtnid.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gfhgonkfc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gebsudjyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gwtiyevje.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmcauldyg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxwrfzyug.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbwpjefvx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gumecteqs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/girkceufc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gedbduvol.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/ghwfrijjf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gqfspyomr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gvmaklzzi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gskufaccp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gthxmczkh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gndxrokzn.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/grmolodsx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghvoiexhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gdmzedlih.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggwphkmsy.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gdpmgvbsh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmywwdhu.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gyetttgzf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gyrgzlwpt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gvyyyspqt.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/goabrgfjn.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gjeocyqgo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/ggripumjf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gyxonximn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gpwxtalgn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/grpohxjhr.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gamglnhuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gmcqrceio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gfxkxylky.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ggfujibfa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gdbupjynr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gdjnuersv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gahlnozti.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gocvmpwop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqggebabf.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gpyeujvek.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gcorsrgmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gpefvqwwc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ggtxugeme.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/giacoctfy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/glumprgus.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gxquufzwe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/ghhzhmcpu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gacjyumkg.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gzihjzcjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gkkynfgyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/glevyjvcq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/girzsnyme.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gazcxsrmk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gbmbfrbpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gopvdshew.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gipwvvixj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gurlzblfm.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gotodtetb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ghszyptgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/ghfldnvew.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gtaqkzckn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/godsxjbyb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gnhydzxqn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gwfnoubre.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/grrixeodc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grjfigfzb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gcrszsrli.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsyzugmdn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gbvmedjww.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gcqclhvxw.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gcazyxhuj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gbsvorhjh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gjmybpctg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gdaupztbn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gabesgkpq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gshbdlymw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/guvdqgloi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gyzdqxhhh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gjeivcuie.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwtqprxce.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gtptfcbft.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gqeupqocf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gzjrsxovz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/goeycjssa.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gcescryxf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gymbjawqz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gcbewulkl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxofrlzyz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghfcwkgbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gmhkrucqn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gkttyyvzx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gpnznfvrj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gtcijwtaj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/garfcxojj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/goeeigxea.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grzzlsbxf.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/guwshmkfp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggtetpfiq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gmsblrkki.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gealjaohi.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gvgzwusyj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gpqscolck.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvchnossk.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gpeclvryz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gsksjdcky.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gloqseuke.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gaxcuniys.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gkoycsfbe.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gqthponrp.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwlqakewh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gmgyqcfdn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gwofnoxxj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ggiftgdfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbxnmcsri.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gxuxuvipz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gquuurtyr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gbmaxewid.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbfvwsewc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gpddorhyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/giqiyriar.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gdtugaziu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gslgkunve.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgdsmfm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/giwgjjbrq.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gvdsfrlie.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gkimazdjq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjkxtjrqq.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gtyjmgeof.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/ghostgftt.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbneqojm.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gpkzbnjsz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gzmsphjzn.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gwyadtodi.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gytbwktwn.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gfxenknec.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gyvyjlgxq.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtpdwxxdy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjdsrytqf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gixsrnlmc.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/ghgkasfaj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gapdacnjd.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gcprbcrzr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gtmejjiel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gnqnkrkbw.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gesugtuxu.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gwyivpvbz.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gyyylxjjq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gpfgamxmd.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gafebfxgn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gvjwxihkn.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gwzcvtgfu.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gogijlafl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gowpxuuaj.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gkflagxtx.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glndxzfux.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/ggpnbndhx.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gfcosuwfn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gqqakibdj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/grixmyuro.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gmqradsny.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gjungtlmt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gblfhnxsi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gksjsjfqw.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gsgvewrya.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gpwtntxgb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/goegqflfs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gnsvbntlu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gbbniuniv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgfsxlwa.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gfoswggnf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grujktmtl.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gyaucejzs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkrlxzlnq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gfeaqmfaf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/glyuzcnpg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gquolpxcb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxnvrhbil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggcprbhpk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/ghxzasefz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyhrrnbau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gohwahdtw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/goxmdaeka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gykquqetf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwnmdgjbv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gddqfeslp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvmvejhbd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gngtpbynn.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gkxpmzrut.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gpuezamhz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/grjwhmglr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gmsmrgvzn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gllywupbj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gektyvnwd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfaoiuuad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gdhhzlwxg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gkjyzehgl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gsvvgldpi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gttakllcl.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gqsomwghd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gevlhgouh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gfqrfxrtq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxypvefdl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gasegbpqq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gusvetpum.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gjbghqzlc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgvrmts.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gniedfkfj.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gctgyhftz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gelkkihyu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gxogbfgud.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grqqpigsf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ggcomtoek.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gznwhtcyg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gymxefreb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gakfkcuuz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gxycwhmek.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gdubelspz.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/ghurfcnuk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/giufwcghu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwsqebaku.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gwcyqxlvb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gltpityqa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/ggmhezlej.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghuicliqt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gciuvrtpl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gatlyyqku.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/goakcvqvn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gdjfucbgc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gguggxvll.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gwpbwshew.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gmpljyanj.sHtML


<!-- 参考信息 -->