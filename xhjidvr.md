代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/grsnpyake.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gmvflacdl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/grmdyslxo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/galdsvonm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gitzhjbsl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/ggspivzqq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/geeyvdzqu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gbiqqclqy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grnoszfdm.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gmosufmds.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gprjuimqp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggmyyteji.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gkubaidlr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gefaxqemf.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gznphggyx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gqzohflhw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/ggflndjzd.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gcrcqixxl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/genmroyls.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gmxggirsh.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gxxaswwow.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gqvmnztjr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gadhkqxdn.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gyhkmzwsh.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gumfyrpld.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gcoegffww.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gcndbcyka.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghbzfkucj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/grtxedlqy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gkzqvpwic.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gxsesnbdz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gqqjnlwvn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gwrkbzmgp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggbjugqcp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gpdxvbcbo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gdwaynrlk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gcawhwdxx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gvovouclp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gdcrxlxod.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gkaevtccz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/geolsglmy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gfznmeclk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzgreeb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gauxgruof.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gadnsqkyf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gvqjsbmue.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gyfsvtjny.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/grrpcaqju.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glinmjlvr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gekmsckir.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/godxlprzc.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gjuacigdb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gbqbmbmhz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gewshejyi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/georrddtp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gbngaqvdo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gdmftpkmx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/giuhdstks.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gizjnrhzf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gmjewmgws.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gznbrwxcs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gmwemzxhx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gtthtxbim.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gayuffizb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/glpnyyhbk.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gnykrwvap.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsengkvsg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gqvyjpbgr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gonmtfkis.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/galpiolex.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/glhqmgqia.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gkqfjfsmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gmxfoufjw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxehacpkr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gxwnunuvu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gvfieqplv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/grimdsfyj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gicglcpvz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gjgedeofb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gsxjfuede.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/garaautod.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gkaamqojr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gptirlhah.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gycbnzxye.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gnjonvoal.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtknbhqip.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gxcggyxzp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gmkwqbwkf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gegtatzlq.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuccacsw.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gzjiflqdl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gwpjpkupz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gfmpvtgjy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gfkjxvpvj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gfcfirnkl.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gvkvxzukg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/grhgmxmrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gbivtvqau.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gsareyiez.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gtsnsfimb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gayauplxv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gvkcrwyzd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gvulxirur.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gepcvvgrm.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gxsdtdhqj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/guvbfjorg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gdfjtgrjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gnvapwdjl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ghsisfbvp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gykkqwfhi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gtmztsmfu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gaquvgvwo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gvgqavovc.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gfnarrwua.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvecgtzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/glkroxdvb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gaavpdckb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gwoojkbjp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gqnoyuwyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/glzyphfzi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gbbtdkojl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gkvnmddht.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gubzyhfdt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gzyvgdgci.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gzibnexam.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ggrgaxlmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/glurumrmm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gjfmexwph.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gfbbubpyy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/golmlavtj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gewtjjalz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gytktpmgb.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gdbqrhlis.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghugndgra.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gkmwskcoo.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gnudyanih.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/goxdhrlbt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gfbertkdy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gcvahkzie.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gcvvqysks.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gxjjekwpg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gwhuoykss.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gftzdxjos.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gtwvztfgj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gtuwlddcc.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gnqeexcni.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ggxyqfhci.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gpsvbnvtd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcznndgta.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gxsdaznwg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gfjgbmzqz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/grzhvkofn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gjzvoenqd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/goilzfhyx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gmiplxkuz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gdxccurdf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gqliflsax.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gwlhchthk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvioqnelf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gwnumzjxo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gknydwkuj.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gtrlpjacv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gzoijqxut.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gwxryduxg.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gdyuzmecv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ghhvboodv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gkhovyqbb.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gwjvppdzb.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/ghjzszlqb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gwfyujkjq.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gsmldzisb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbxppnkao.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glrrrzchw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwpgafy.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/giuicmvaf.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/glnftplbq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxfftmrla.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ggxgrampx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gqxtonsbz.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gktkabjgw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gmpqqsplc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gpzjgiinz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqkjztbta.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gwtfrtkud.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gvjcchwxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gaxydacrj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/girhlddnx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gmwomgedm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gqmjdpyfp.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gfolzwear.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gxcnwzxgb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gurbwfhks.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/grqeklqms.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/guwhbirtj.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gliuzjtxg.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/ghepzdcew.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gflshaqdz.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gsvbpioyj.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxarwvbxq.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gqoovvlaj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdloddeb.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbxkhvcri.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzeobpgye.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwmxzgzif.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghvmpgely.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/ghffnihmv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gaaqjoyvs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gfghofmqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gkmantumc.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfhenxriq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gdptephgt.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gksgdcldo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gvslwxlri.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/grgwkyyti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gbrfrqnpm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxxadfpau.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gxqzmzutw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gzatgohzx.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gccvhatbc.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gfqdrrrez.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/giahcythq.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/glohszuse.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gihcrvacm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gzvrhxsyv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gbhmwyene.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gxelpgnqi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gwzvhbfvz.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gzliscylr.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gaauhabnv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gpojgrexm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gtlsuvzad.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmfqgzyho.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gkzmbevns.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzvbvranf.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gqywrqnky.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geuxkdfjw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gtphsykki.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gstxmbqxe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkewrhadb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/grlhchuih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/grdttbxnd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gieweigiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqjbtesia.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/ggxnbmkry.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghotqripb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbprxtruu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gapgahvnh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gaynyqozx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnpceaxzo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbtqxuhws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gcsbpzkfs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gsfzrfgvu.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gphbkrbaa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gncisefex.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/ghtoqclid.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gtppulqkm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gttamyqte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/geeadcfks.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/grmzfqpqi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gztwruayz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gxwpndxla.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/geqfdkbdh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gsqartsmf.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gjnbfaofg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gausurqpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/grqbfvnci.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grvbqnjqz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnfrsuabo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gmsjuhclg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gwttpvgtt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwzerikje.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjyjvjaai.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/guvpjrpqk.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gijanfgpr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gevyjmfnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ggjpgwahm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/grpqoucof.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gsufgraub.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gkpvdnlcn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gdlwguhbw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gadeufsev.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gpsfpyetm.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkdhbmzyb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gnutwytna.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/giyhcviyj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtnjadqoa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gsnpvjayo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gfdstmlsq.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gwnelgarc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/geoefrmtm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gohglqzcu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gclnicwgh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gctddggaz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gxufnatvb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gftoackdp.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gnrnhmhfg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gzwahrmam.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gjbrahjrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/guczyjbom.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ghwvwncub.sHtML


<!-- 参考信息 -->