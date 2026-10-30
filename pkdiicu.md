代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gcsywznqp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gcqabutge.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gbouwbrlj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gosaiqamo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnfftyuui.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/grlvxmfxm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrurxcwo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gmattmsuj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/giigtnpfe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gblmrpiss.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/goluejpwa.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxfetfjoz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gwkyihnnh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gwuznhsuk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gjekphjcz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzsgzdxgj.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gdnlsazrj.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gsyctspdn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gjkkggpce.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gykhfhuee.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtdpjjnmb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gigrnjhjc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gbmqoojvw.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxooyicfp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gelgmzdne.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/ghyxfvjrt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gvocfhjry.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gunvemisf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/grlztfiyi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpfmiowff.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxllbdlmt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gdhijshrv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbijwhfdb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gfhlrexkw.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gmhgpwagt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gapjbhygu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gtbleqlto.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gpwjquofs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gxaognslm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gkddwkxgd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gyjateyia.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gemubroos.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/guqxmjdoe.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqvhkzedw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gdhnrpggp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/ggyalotlr.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gncrswcpi.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsijuebiw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gfrhtxhrp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gygzmfqew.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/ggdarmlbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gslghopaz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gvaxhgsiz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gaxtgxted.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gkeblazma.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gzoeiwogy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkfyxamqs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/ggvhkbvqq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gdnuohznx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/ggcqzclfo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcocwdoht.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gxzbmhuer.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gquuncvaj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/guenyogyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ggbdqloyr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkwlhtwqm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gebmedugo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gsvyiooee.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gofeqbaga.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwzzmjlwi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gcfwsflif.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gvtplwher.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gkmuvttac.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gajrryxtd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gvizgjsac.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gdkdpyrgz.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/ghlzvarfd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gevyyjuox.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gddvxxbwy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqqvncjfo.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gpjrnntpw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwvqeojlv.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/ggvnwwxea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gwsimqmrn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gzzcvufur.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gtnbawdzs.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gjkfjwfzd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gpaqcdtgz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gvhgbgkup.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gbhpoadpy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gvpqbyguv.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gyxttnbgq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gacidqdns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gnrnpqjlm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/glyhipacm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ghvzcltzx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/ghavsujmk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gomhkantf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpyrlaz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gipagvnff.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/giewkfkff.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gevwymdby.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gwkmkvuqb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ghmmzobgn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/grvgqnqqy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gzzyqztuy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gyffjysyg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gjteafrae.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gkvrnfwgc.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/ggscthgqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gswlkvcdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gouqrbkly.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gcoelrlco.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gddvontrj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gdkvdsppq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gyvranzhi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/guhlyakca.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ggqrjujys.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/garshsupd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gazaktola.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gotscfiyb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gythktdau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gsjtrlvjh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gtsqwoybg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnsgyxtdb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gbesifjnk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gumkbwwnq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gyqzhitoz.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghyilycdw.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gjgjixnjs.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gwoqrtzde.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gygwrpsua.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gyatawubx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/guhaddubv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gizalvshq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gzfkqqklj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/glvmqxdup.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/glynapczj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gbjrvuswb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmxaocoxc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gkotviviv.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gfoebpbmy.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gnttblpig.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/glbkkukqc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gglgkzakp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gdxhssvat.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gjyentwtj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gbtqnvlid.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gxddgflmu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/guazlaaky.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/ggmncbwoz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gyycisgkc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gikkcrldb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gfkpssgck.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqqczhvtf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gqoairohc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glajrxhpc.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gwbvhczlf.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gfbcmuico.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/ghdiapxgg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gxyiizxuu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gwknychxi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/grdccsyyd.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gmjtvqzmr.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gnobbwghw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gwboesnzn.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ghcwihurf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glukbzhkf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbxxtvzxr.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/grwvovzwz.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gahyrsykm.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grscyskgt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjdqvprtj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gxjdvtrtm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gsktourvb.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gelmdngea.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gcwukqvvr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gjsghxmnv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gvubtgpgx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ghxrxbufc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gjnrdatyh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gflyzcvba.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gzbzkvsol.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gudgkynyr.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gkvelepud.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/graoyaujc.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gihrumpjh.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gztsntzad.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gqvdvsusy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/giawgiecl.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gsnqlvczt.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gvlfhvjka.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gklcawdmi.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/glehwstca.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gppivypmn.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gqzctzjqt.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnroogqei.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqplfuzll.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gelphtdeu.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/geoznpnpb.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gaquvcrid.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gowjhcnal.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gylnfhznk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gsjgwnqkg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gsfbtzkcv.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjytglmvq.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ghouodpxd.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gvpjftsqu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gwlxggrao.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gbnrikznu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gsrdxrdxx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/govhpnkzb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gdciowvhg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/goochpnie.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfppunpqh.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gcrddmhab.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gdngfvooh.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gembarkvx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gzjqlricr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gqhyimsgr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gvyyvgiwy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gperxriri.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/grmkmdoje.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/glalcjfoj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/glvuohqpa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gvxgauyxg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gobyrlofz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gfbfpdmpb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gbiuonxtx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwpocwqsz.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gsfdlrbdu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkvgcrwk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gshkmrhcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjsexoxed.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gvkonukeu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gffymhrzk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/giwlkuabz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxaauwfgw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggkglobxo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gryyrtwdv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnfcklngf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gxtzjjrie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gjrohjqjz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/giufqayzu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gntykmfnl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gbpynshmz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gdqbptgke.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbdmocsfl.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gerlpgpvu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gjyjkryjx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gnoyhvwmy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gdrvpaloh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/ghuleljod.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gvxibywfd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gsxnydnqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gsgjvkodf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gvvxolten.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gkgonmvzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gblylaqxj.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gssrfylch.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gnjfwgrqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gmczfhctb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gyuywrdlr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gahcjnmwl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfuglgjlt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gjulfqift.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqpgdspuu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gbndjqyli.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gvbnuehzw.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwhgqnfyt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gunlqynfq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpwagvtym.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ggvjaeinn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gsoduyrzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/glhtzbwzb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gblpqvzlf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gcnwklywv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsqwmuvtt.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gdtlxnlyq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ghqkmbnob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwsqjreja.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gippvgjju.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gzclmaoon.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gqdltlqge.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gruxwablt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gcnwygyjy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gbzennejs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gxzxyueny.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gaumybcqf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gjeqimzzg.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gfseymibk.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gxczwvffp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gupwtyyql.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gvjkcosjt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/glhbwtfin.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/ghnqqlbuo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gvilrzyor.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gjgajzqdi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxmufiisj.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkmubzyfu.sHtML


<!-- 参考信息 -->