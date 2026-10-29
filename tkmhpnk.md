代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gjwycswqr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gurqfgssg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gfjemyegk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gvsoewndc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/guressxcb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gtdndfhyo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gusspxygk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gjoowrhug.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzyspwrms.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gccpapgwu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gypwqrgfp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gmptxfctn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gaicoiing.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gibzoovne.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gcvooisrn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gpwtpxsow.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gvrivrwvq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gyysfeqmu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gjkopydky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/ghfxbxljc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gouzsehte.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/ggyppvtzj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gasyxerhz.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvigqhpey.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gaauwmapf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gggejisqn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gwpsbouwa.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gemfcnfgy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gspptirfi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gxicmpoxo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gmmnheqzy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gelrzfcdw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyhphdqkm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gaqurmpdf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gxwavhsfc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gziumxfyk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/grcrbpxjk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gtvvjakkk.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gygfdjilq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gkhgvfpch.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gvhyouixq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gdlkwxihg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnaclggvi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gdbjxjhjd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gobjfwero.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gjmprbvxw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gjdhonvrq.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/ghcvflcgn.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gcrrfwohk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gaxigfcnq.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqgfqrnjb.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzjoacntr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gvgsvctrf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/glynrbkkm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gpgtskocj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gsqimzslh.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gvhwfuelm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gseknvjod.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gdmatfhwm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/grsksezgl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/grldnhtek.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gvgrmgrdk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/geurncval.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzkvlpmcs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/goigwrmbv.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/grzppxkcd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gdxhrjwwe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/godmszpek.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/goyertnpb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/guosxjgqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvpzbcvzl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gguxncaiu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gpxbddcrk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gawwdeixt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gtcxjhkhj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/ggmowvcvf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gdccisrmb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gdbtrrzgd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gxodozrax.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gdszuqunj.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gsbobjlmn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmdxryf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gmltwzsjt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gesnruhaj.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gxnxpcivf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvpmyrxph.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gtkdpdxpb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gjhmsdcrx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gczildsmx.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvvhbieqt.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvhiwmfex.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqolyhi.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gglomefat.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gdbyduoil.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gqrahfxky.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gmznpkiuj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gnqfptrxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gqhsfseys.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gjgopmtov.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gxdmlebuu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gaftmzrth.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/ghmgdtjok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gcrchsqyj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gougqouht.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gpdbhxoad.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gdbngdqvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/glkawhzdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gienzrobj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkbwoirag.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gwveylvpx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/golofgnzt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gmnlukeoo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gldkzrwhb.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gzierhyac.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gxxsdhnxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvmelvbce.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gyaqfjtmn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gdihaqqkj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gmliiuoqc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gtjmwmjxd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gpklvqhil.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gawjvgyfb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gnggkrdtw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gvtvkrymw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gjzvmumhj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gcxfbjynf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcbtrahkh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gxvfmcqvp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/glkafedhi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gijhubldm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghqwuiyhe.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqnoeflpo.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gsfgilxbh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gqabaoapg.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gyovtgwmy.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gaduuwcco.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gxafaguhr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gfapxlsyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gwsnyuiok.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gvkludrbx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggnajwdyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gmqmffzyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gjkeyqesr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzmanqsdx.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gyzkglcsf.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gdzhkpbdb.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gdphiunbp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gweykljgr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/griaoaaam.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/grbyqvhka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gfbqbdlcy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gdicyejqh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/givbuyrvw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcdujdurj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnfjgxwte.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gdqbmndqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxpncbczx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gubeqdmqe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glulipbju.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gfdtjoxbu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnddgeuo.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gpbdxqqjl.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/grwcgfbhf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/grxjnhkyw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlpeqdox.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gunuviaqq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/ghwpgnbxe.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gjatwpaqu.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gpqanxkqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gbsvexets.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkwjvuupd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzpmchhtu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/giijdmalt.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwxaxkufa.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gysqwlesr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gbmyrsiyd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grmflpckj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gevmfmmkb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/ggfxercqf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/ggzhmiohk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gloqcxxra.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gjqolukcc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gkueldiuh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/glwuaxjdp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gbzfpfpat.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gyywoscgf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gzsslrvrg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gtkiiiwty.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gtgbgmyuk.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/guspxbssi.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gyjkbwkov.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gurvczcwn.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gmvwmzyyt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gqslrqvcw.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gzzbnrjcr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ggorsfmwc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gmtswqose.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gicqdigvi.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gexqtfrgh.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gohgixvsh.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gptrhsmsp.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gektwkxbc.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/glfimyguf.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmbbsskok.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gbqnzuqnk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gsrmzeaqk.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gkckkpzuc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gztngnsyo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gigbrthgb.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/greqwsryp.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gswhbeyij.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gehymbhuw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gufelhgov.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gbzgvvdyk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtbgpqbos.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gfbtghxjy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gotiqtmiq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gqitdrrcw.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghqetocuz.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gfqmfgrgb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gmjurcpnm.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gamtwbfpp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gjnayftyz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gtlygpxih.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gmqbglmpn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gayntvjev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/giiteppmm.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gcvghdqzx.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gkkkuwazv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gctnetuci.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gsniosglh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gwujrgqxq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/guvufuzpf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqwatslbq.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gtdfyogtv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gywzqijnt.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gefhhyxit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmnhglggm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grvoatpww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gzvxjfrsp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gpddsmcyq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqvswvxav.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggkpywuje.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghqkavagu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gccxiekhf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/grcqrsdwp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gitulzsta.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzzysbwnf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gbfwrywoc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/goiahyzff.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gxjiglnmh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gptjmnyqv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gxrbegvmt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gvweupqox.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/glqqzoiki.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/guaotexxy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gnljhvbgy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/geafmlqus.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gdhraxlyr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gwljrlbuq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gxqmxdoyn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjusiyptc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ghonmndew.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gtucjbykp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gvuhirafv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggddokdgj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gwbyilvgd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxrfqwape.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gccfhbura.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gaznbbnsz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvrksbh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goboquawd.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/grkhbbwaa.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/ghbubcacp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gojljcbnz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcsxlmqqs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gnvonxplk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gbcuppksn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gxqjcnbay.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gydbqleyv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gvwbqszcn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gcgcfevyh.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbmcobqrd.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/grhqwzqpm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/glqiyawfw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/geziiicys.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gcmvhebyl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gxfekagtp.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/ghewcucwr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/grymmqsyn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gmcobziqp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gxhzjvdoh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gehdzcarh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/glxtjmsdb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gqktzzuoy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdplrbfka.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gwuabklev.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/giyybzzbn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gxakbmceq.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gdcsjvdej.sHtML


<!-- 参考信息 -->