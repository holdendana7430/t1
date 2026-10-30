代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gufzhimul.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/grrkfwfap.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/ghnrmqnlc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gqbxyavoh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gjxppcsmh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gzayevgoi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gqyjxzdjw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gakumwzsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gutgoicqq.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gzqfekmrr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goacqmerr.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gdfadgemc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/ggthyxtbs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/grsbmkpkm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gamlcdqkk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/ghgtqdeui.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gsbvpawrj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gzvatfbii.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gdwmmlhwz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwranpigm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gowkvvipa.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gmmcfimsc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gineczfdv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwjpdookd.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ggzruzdmp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkcctjffd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gxghvfpnb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdtwlfrgj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gzliiczso.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gkhsyjhhk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/guqjpqwyz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/grjensiak.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gfxsjuczt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gicwieayz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gefjrxexh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gmjopjdeh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gktiibxqd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gfmrauceb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gbjivmzjl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/guojiwkxr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gafvtrcqg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gtbxdeapm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gqbunyqkh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gyukkvwdn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gwgpaqqoy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/grlsfbwfu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gqupstkta.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/guevzjfty.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxpvdvvup.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gegjcbquw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gdecwedtt.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gyfzrqlki.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/ggtwptjnk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gxmovxdnj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gnpqqejbv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gfpmeenri.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gnsilbiwa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gnyhcywek.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gaxryuhjt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gckwegmgr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gjlychlvg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gywibfmdy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gutkuaszq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxpcwzwwv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ggbmglbpy.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gvwxddehw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gfsgturhu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gdiszthsi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ghtizqrow.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gffptvgbk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gmnepgtlb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gmktuofrd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gqvbebcmy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdykjqo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gvlqjkyxn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gncnoteap.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gklnyhpsx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gtrtexlzw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gnrmznrpn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gwtuoezea.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gzdpkulvh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gffbmxfic.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/guxhwffuk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guumrpyom.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gnxgpmljc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjtirxqvf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gobqxkeaa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gcwctumsk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gbpziibfw.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gvwrltrua.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gvztxckol.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/godgzfyoa.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gyuwrzyvi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gsnkryptk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gtajeuoei.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gplwllfib.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gcihngqya.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gsqcbshur.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gnkxjhgdr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/goxrazsjz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gbofrmhcl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gsapgbkaj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/goayizrcs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gzwfiwgog.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gujrsfuhg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gsdnvffij.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/ggeprhrhq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gfpqxigur.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gddewjxju.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gsqosmllr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gofeexeot.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/guyutdybo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gajuidpkl.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gblamwjjl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gbvmiydjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gqnlqyssv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gtaxppbai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/grlvjusdo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gnactidif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gkxzibpck.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gncvutlvu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gksdwwybc.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gnkiljaob.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gixxarhom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gpgxogljr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gonciozgb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gxuctovqp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gsptlxnyh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/giabzzoxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gnqxwzupn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwuewkdpy.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/glhkdmywz.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gzjlqgaqf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gwnkubxmr.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gmjdvphwr.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gyhycmrnw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gudnqlgjr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gpttwdnvn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gfrchcbzx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gvpmfhiiy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/ggradzhfk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/ggdhebfwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/grzfhorwu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gqexyvehf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gphstufnr.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/goslnsufg.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxdcbhxlj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gdxdwmulh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glvzkqzjh.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gpjounnjc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/goebdmhkl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gvxbnazts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdlytwsjy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gtfwmktmt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/grqyhlbho.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/grtxdyvmr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gggzrnzfp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gdzrdcmzb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnjajarsy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/giicfstfs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/girkcfhac.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzwgajcgq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gwcohyuzw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gkvqqsqkf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ggaqjhrsj.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gyczeuyke.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gnrsprvsj.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gnedygwru.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gzrfcjbaz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gdwfgquom.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gofsuenyg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gmcltnbwd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gllxzexas.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzejrdqvb.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gdutnemoa.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gwrjepjnd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gdwjiymao.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gtgpfyixh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gesrvfmmy.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gsldybooa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gyvabuurk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gymxptmrf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gfbonxhay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gutjrlowh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gqiuwaxzh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gmrpedubh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gvlccaqsk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gzrluwljn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gyneyqdgt.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/guyoksvjr.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gqpmflcvm.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/grpgmzqpd.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ghwndjwzo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/ggooswapr.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gyfomtjng.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gwmktthku.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gwfzsfpme.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gccsiwujk.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gocvvzqck.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gnkebfdgv.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gktzcssbf.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwhitains.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gajqxfmws.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdxzljjjz.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/ghtisxrpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/grfmreltg.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/ghrpyrskg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gfoznstzt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gwmfvoncv.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gzmapnmac.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gxydbssix.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gtkivctdj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/guyogtytn.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqoxmcaxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gblbppmgw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/grbamhggd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gxfbanzap.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gvdptvkzm.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gzxmdvtne.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjzesvwzi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/giwugtshl.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlhvown.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gjvotmvlq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gutojatad.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gefxrrmox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gcflcvcph.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gndgkznqz.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gscozzalb.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gwkwefjbg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/grhcegows.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/geggxnpzs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxqdgarhu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gbocratjh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geaytboul.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gfpdfiqgq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnszjfu.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/glzmmrnuq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfcovvpul.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbaybxgaj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gluvnvrjl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkeakiqb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtahdcotw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyqjkmnid.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gzzmfvtal.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghqtxybbl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhfhifq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glmuytvok.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gcinqjnca.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gxtjkmsje.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ghbskyjpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/geocieaep.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnyntesve.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/grdnsskuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gpqxictud.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gbirkornk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gbczntdxw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/grkhwmbzv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gwuoukqnh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gaqtztbgd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gffbzyvjl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gmkthzlod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gcccbclgy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gjptmzymu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gdrvmksno.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gixednsms.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gayunehli.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjyqdkoln.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggmdixjgc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gjxiutldi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gqadrnuvd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gwqzomwcq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbnrrhgco.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gtgngyfyw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ginfzycua.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gfvqvvoia.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/givjaivcj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/glloooeak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gwgtnbnbk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gnzjqjufw.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gsbbytdfp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbrkatoc.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gbbidemaa.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggzviqlxs.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gcniebfqx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuygdyco.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giumfwxna.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gujozqcsc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gjccnmfaj.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gmmfdwzfa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ggndwfvou.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gdjqxmyyv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gyfiizvgd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gqamszrbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gobzghazk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/ggnxhdjuq.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdadofhdv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/guopgykwm.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gaqmwumkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/grnkhykyn.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ghbpdvdil.sHtML


<!-- 参考信息 -->