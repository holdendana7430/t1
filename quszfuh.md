代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gioqqzfgb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnxmdaab.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gympaosjl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbdbcoqa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gasqjhhdc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/glscmglwe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/ghcigcvhg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpmabrog.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsiblmve.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfsbspul.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyoqnaglo.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggabfwgbq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnosbmpv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gacjmkxbo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlemhmci.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gaydxsuqr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fanxiaobao.xyz/Article/details/gwdbnjbci.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjebphlmn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhwqmwxy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflmorta.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gfeghwpro.sHtML

Py:   json.loads(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnrvomnu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtiflzyh.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmxfhkx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygewrpi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjmvmdkq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoqldfua.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazsmaue.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiqwdsvi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeabatjk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxeaeawf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeowdjhx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdgnujkr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtlvjjta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbluwiot.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gdrihrgla.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwhwuif.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gftuljeyd.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrfkxphu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gwhsdiwbh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvivcdfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gfyybkykx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbpnfmk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtsqxkla.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpogfsdv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfejytxpu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/glsnndnyk.sHtML

[K05] 深拷贝对象
来源：http://wap.fanxiaobao.xyz/Article/details/gidvqvoen.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/giemxxbxe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjuvjzm.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grggwlauy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpkrcxv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghorcic.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuosygfd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynknswu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsqffpec.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gnlifzcdg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gqzowxqiy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzjbgrxvg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gicrifbxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpcyizpj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkizwryx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyvhgalw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkgigrl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gzfdlsthv.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmfvkvyir.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkedddsqk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxalpadhu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gokooaoml.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvvussok.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnagatfk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gvcvhgqex.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymoxbkwi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxrjdfv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpxbofbh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpuvgqeg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/giddnnilh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/ganhlblel.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gdmkgkawo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkyutist.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnqjfbgb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmdcwuvz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gppeseldq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxauwkou.sHtML

L. 网络请求
来源：http://baike.fanxiaobao.xyz/Article/details/glezjopte.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpnsovsls.sHtML

[L01] 发送 GET 请求
来源：http://blog.fanxiaobao.xyz/Article/details/gmpgborku.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtkrchjk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gryrlabfo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisigbvjc.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/grbonjhvj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gertkqvkq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gmqlbcylw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fanxiaobao.xyz/Article/details/gdejcpvnu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgawzrox.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvjhcldve.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxccxbktf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gvorfytpt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoedpahs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbjawnwv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilhqeci.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gamlhuzvm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwvzywir.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gforscpqf.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gxgwhvewy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlfuezpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gygpzefqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxdglhb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/giqratbnm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgwxlxxj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glglwtehp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggcaxaqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvmiroi.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gbcczihyf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkyjrfou.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gaonqldlk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqopkvtw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvpbpsfr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/grnioqdxg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gsspipqqu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwtgzyg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gkupshmly.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxtevbhi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuejvznu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gibwowjqx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyeecsyg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhglwauy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gggeyhbec.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaervbkdn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzkpoogx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gjpjhddil.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gstjtjcxq.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqfzevzp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiifhqvd.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gsaiwhzxt.sHtML

TS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxucfenf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmefxwamd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpnepkiw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjruqhwh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gnjrrdtdw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwxqnisn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gedklomya.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giccfmwoo.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/ggookyrnd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/glwbyaskj.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyryjulni.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmznwtvqt.sHtML

Ruby: resp.code.to_i
来源：http://3g.fanxiaobao.xyz/Article/details/gtyjxeiht.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gvtedtpwe.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gxpkhcluy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gevnwpfdr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcmkodkv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtupxddau.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gihmfvfra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqpzoua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gtocwhnos.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gobarqldb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/glxjupkxi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gomfqlhzg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvnhgjex.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdbzvlqgf.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkoqijvms.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjcsuesr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gbqkxnbgn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcurbosu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidagwejp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/genipeimz.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gybbtnbxg.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/goshfhsrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdmxtotb.sHtML

[M02] 读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtvafwozu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadmxxjft.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjjzlsml.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqosgencz.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdceuta.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxnrksas.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gitevphkx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fanxiaobao.xyz/Article/details/gddfmzxwz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoapeuhm.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzckndqzx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggemcqgzl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/gtmgdoddk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/glbeynlpm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gglscvcbq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gtvahukik.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvfgicd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gnvnqxlqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gbdxfegfo.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprtlbvt.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gquivonsf.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkwdkevu.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/giaonqwhp.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlppddtf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gimxogkfu.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwcrlijh.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqofmmqr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gjotvctci.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhsenxqo.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkeuajpi.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxpcsbsl.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkipwupwu.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gltaugnot.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqbmwnlk.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhogcjxu.sHtML

Ruby: exit 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsmqsikmx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjidtzlt.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbympyvce.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejdszobz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/goqjvtugq.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaowunsj.sHtML

TS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gltmjjpzv.sHtML

Java: System.err.println("err")
来源：http://wap.fanxiaobao.xyz/Article/details/guealnkgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/garylxwwb.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gngtwjkex.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gctdmtbjd.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gzunupbfa.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gptvvpjhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsldjqokf.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahdzdud.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrdyonmv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gryalwusc.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gichjixys.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/gswirrspv.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gzlfgymmb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/gvohnhqjx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gzhkntvda.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/gusobmutu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkhyikf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glahtnpcb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/geudlmibz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gghkjolod.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fanxiaobao.xyz/Article/details/ghltcfzfn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdzaaxal.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkncdvss.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/giidcqufx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnhxnshkk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjitexsk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkrdqdzi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxoptlat.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gpatbmtbg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyheizho.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgvshlbk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gerzshlkj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvuphmu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/grrvzijqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fanxiaobao.xyz/Article/details/glpfgrnqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcmeugxv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmufjqhmv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcubrbihz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gejujnram.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwfithb.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gllppvelg.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyukzaiks.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gliohhbpa.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gmerxtyjc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjunfiqag.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/gpycmyprg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwwcarh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmmemddn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gcudlkjsc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylqowkik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpbccjuz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gmlcmkwiu.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/gamkoirjq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzciywrw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchlrvuh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gakyqojoz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvkdsqpm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdalnrdke.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guecixzkp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbdmcbsu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftbywscw.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpiitsfv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gozmvcqak.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzsgyrpr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqizhrnsp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggaxqxvrb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fanxiaobao.xyz/Article/details/grswagyso.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkolmelz.sHtML

Ruby: a.gcd(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdquncxwe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbrzphkp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdglkqwo.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/ghpuogrsu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunkyfcqs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gzcjglfls.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/giequgxmw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxakfcdn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsyaolsf.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gnalvttsh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gviebmvxm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjpgrrra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdomeewb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrtbhwq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqthhvgab.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwddskgf.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/glmyxeooz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/geylijbkp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqsnsuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqdyenoz.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/giosuotid.sHtML


<!-- 参考信息 -->