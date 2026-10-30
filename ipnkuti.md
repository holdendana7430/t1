代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gmjfquptv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gcavchhkf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gpoxngzae.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/glucnfuzd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gphqvplkx.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gabxvwpoi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grbwtpliw.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gbyfehwhc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gykfptlek.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gfvmbcvpi.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gihnmkmxs.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gumtqzuai.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gfugzsvek.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghquuzyzz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/goapcmwdo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gfwhlbiqf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gseoonajq.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/galmajlxx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/ggjrdkrpi.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gycrcswdt.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghqvhbbbk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gszcekzpx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gnsmwrovp.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gxrbwmaya.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gkfinwhza.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/guzauvowi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gwiyzyefj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gbnvfkhsa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gelzbsmxh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gcjxvxpgr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gvoqxcphj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gsisuecwz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gsbbmhmgg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/goklxruwf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gfezyfmek.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gcnjvbhow.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/glfyzlgpj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gzygthlgm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/grdbioupv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/glwaaprqq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gjhbltcww.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/geloveuuj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gcdgkrjyu.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/glwlkzhgl.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gnevtlccw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gdtdujiey.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gpglmxccw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gazeqothi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gdtenbawt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gjtvkzxtf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gvyqpdjff.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/giohrozmm.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gvnpgkrdd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gkcpzfoty.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gvfrgeyvu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ggubcanfd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/giojpinsu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gztarnzos.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjanjsjid.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gbwpwwztu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gekdjrded.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gsyexbjes.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gbkgvddew.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/ghgdvkmwe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxezfvyii.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvrldgmpz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/glwuudflg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/guwpwsdyr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/grtsuyqng.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwbeielia.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/guumlnbdj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/glkvcnsfh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gobpucvhz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/giirzkvzp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gthtlltpr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/guqykmoak.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gxcwdqvlk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gxrxhspnh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/geqffvfiq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxvhofwyq.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gkoiantpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbtmjigza.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gpcsmokyw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gbakokbmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gycavuuhk.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ggltzpotf.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gkympezzn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gwcqnxzvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/ghcpeqegj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gnblnkglq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gcmwnqtwx.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/geeibeiar.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gblubjase.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gzmkqinbk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gwkiriynp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gcjggeimd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/giflyyqdb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gvaihlkqo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gqaexjyky.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/govpdcjdd.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gpcsvztca.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gnihhkvip.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gaaucttgm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gaqyvxdhs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gvjmbfirj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gvadttror.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvrajgfkb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/ggcldjfzo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/grzgojvmw.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/grnicfvon.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/giiovdftl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gfpmcxatr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/ghluyjteh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gopoyojab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/ghzixvckb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gcopiywkz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/ginrpkihk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gltgbhpbn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gxztxwrrp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gekkjucpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gwrbujfmi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gkbxqblmj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gnladtmlx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gyvllwnvi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gquoipdit.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gcgnocqnq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gefvdldzk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gpqwjqaju.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gosrhbele.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gyhlodldc.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtkcoqalm.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/goiilanzh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/grcoilxqi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsubutcc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gaegcdoiz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/ggzmzlwgq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/grqnxilnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gxlmkcswm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gvnzndbxy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gchnwtwmz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/grbjnijki.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gntfooghv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gmbgqjiyr.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gxvmlgyxl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ggsybpnpr.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gpxitviqp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gqacyqbvb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gvldqegmw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gfpjgykjl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grwezwjvu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gjmzplsrk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/grlqzzoma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gidbzpuiw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwyyhxlln.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqztzlzog.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gnwayqula.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gykasaysg.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gdxtvhirj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ggrthoqai.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ghowwxabm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvznwouny.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/guefxratd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzzyveasl.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghikrqxyt.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gmctzovwq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gstlxhtcm.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gfpngweiw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gcolpnfhn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gpnadarok.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gfnnetocp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gfkcycgmk.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gleiortuh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gustgnqlu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gdyrfivpp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsgvmvymh.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/ggvucnqqu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/guoseksaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/ghtmaiknw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gidhrmjoe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gsldgblxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gtecctucn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gpekerxbt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gdsqajzxp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gokynnnbt.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gfcvflpzo.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gcpadfzwb.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gkujcjhxr.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/grigfajnc.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gdmaegbpj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gswemxgjg.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/glrwozqtd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ggifrxrbk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gepcmrelb.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gdmzvsteu.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwnhfkepz.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gnfhpkoyc.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnugosnvd.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghsgdalyv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gohfetfiv.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gymjcruwy.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gssqbabyd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/ghhrsuvpu.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/grgtdczcm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gwybwlvit.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gerwddeba.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gjmhjvxud.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghmoudsuw.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gisrqwzat.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gdphlooni.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gmyxcjppd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gkdtoggkb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gxkbrkyoj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gqhxqlike.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gsysslnit.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/ghjhzmuve.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gmkdqeycf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gnpjgtnkw.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gvnsyovrl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gfiwpqssf.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gvpeerfjk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gmdrzfmov.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gvjnqvaqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gsakxteqc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gtxuybgan.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gpytylcxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gpaakirnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gshkxpgpl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gmmdiutpr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gszzzwtqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqlabaqym.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gqssxzori.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghphpkukk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/ggtyxwyyp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpzbjuxej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gdafwpfxd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/grjkzjecv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdsteonwz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcpszeacx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geqqpaovj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gmjoitzjm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gprezltbo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/ggcmolqpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gzutsxreu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gawpcuzaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdaedsfra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gazvdkwnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/ggafxjcjk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsgszuoau.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gshuocbka.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gykvebwdi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gczyoqxfa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gupzrrmei.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gymbfeqjz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gcerctwst.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxstulrpb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnltktuln.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gmswczkuq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gdchrxjun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gzsghaaet.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gldmdiwyd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gwhtxbscn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gisgtznje.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gftwogcfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdiccmnsl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gvtryayht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gkdrftpby.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkfoxjevx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ggfferbni.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gcokknpfi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gqhdousbk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfcpoxmpi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gjfwfdaga.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzjyzqheq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gjtkxkuyn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gxkabeguz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvprmkvrc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/guhhecwrd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqvujujmb.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/giedozeos.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gvbvnbinp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/grxdvmfbm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqwzpagbj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gipeitnob.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/guucalmmk.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqtnuvpie.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gqytzimwh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gicrffbwq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gyysjzgah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gaxdievlf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gdzintfey.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gzpglouly.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gyxtykwwy.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gcxtdbfkj.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gltagxoon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/goscehrvw.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gapexwwxe.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/ggavruemv.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gcswnemtw.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gurlkztlf.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxrzfxrgr.sHtML


<!-- 参考信息 -->