代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gmhjutspz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gekidymjf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/geyxhfuio.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gelskhsvy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdsigvbhu.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gtoqimpcy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghxuuwftd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gennevbls.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gdvmsnbkc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gamrlnunb.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gnbbydpmm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gselqpken.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/glosoycyy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsurqydcs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gszbknotm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gxtsnniwr.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gukspnfse.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/ggkmmucae.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/guhbqftwr.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gmtsjvqpl.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/ggmpczhvy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gjasmsoir.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gbnooxdrp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmkgnkbnr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/grgmoyduf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/grbnpylpa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gjqrfjcyz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gkkkimkzc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gmmlpidsw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/glnfjbsoj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gtapsxeol.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/geakqurfy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gsjkczrou.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfsijbk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gnywgasnr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gaogfrhpm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gnrrjdyld.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gwksklzxo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/grwdwscpl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqcunogjz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gbypsodch.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gsynvehgo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gbtwrbsvu.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gbqystjih.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gnkfaqgdl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/ghhzzfcaz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gijchxpxq.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gltrwcarv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gjtucrjnv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gfdhehlhc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gnhonreqy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gdgvubste.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gluorabzf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gsjgjublm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/glzpxzrzb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwurdipc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/grdkbkqry.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gnoibrjrg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gxltdzcsa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gdlgenlhb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjcggydtl.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gjofrwxuz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcvwevnqn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gktlecsop.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gtcohscnh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/guxspzaxv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gpyqjjryr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gaklwkxze.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/guyrjmafb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gnrteqlfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gfdluflze.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gaczclccv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gfhtuvzyk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gwyoxcnyv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gyypelraw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gtcaoztod.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gxeygaxln.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwadgnwyk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gnywlalio.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghujfpqhs.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gerscwxxq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gigqqfcjs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/glnepvywn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gjvtdisno.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gpiuzfkmi.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gavftpcls.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gvgvamkcr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gjrlkaqkd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gwvwqldye.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gaiuiymcf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gcxpeulge.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gyvcsbsjv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gyderyzyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gdancgqri.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glpequevz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/ggkbndshv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/ggdtgklcj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gutzqndsw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gxalwobwy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ggvapoard.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gmfqiyvkr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gzdqgndkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gkathbcke.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gxwsfctvs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gsbdumiew.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gragvxdyl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gkhjczqee.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gbewexmjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/ghsmhzrbn.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gxhxkietg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/ghaoocqrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gowokhgik.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gmxefmjqj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gbgbxfxxo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gabfmdzyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gsfcdasjg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gjahrfpsr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gsptgfkwh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gyilmyeth.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gouffbfgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gjmxuoqwm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/grlmrepqr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gcogwsjgu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gsoqcsimo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gctzpyurp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gasffbhoh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gclwzsahq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gtydtnmny.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/govsncphi.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfuwcqbdi.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gsqmkgfpr.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gjgmzegzc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gucejtewh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gsbagqecj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gbrjkjjwo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gvjtwavgs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/ghwysqyol.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gkkwyfrfo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gsqfukitj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gkmzpxwvb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gdfmrwpop.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gbdycmzdq.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwumyofst.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/guaiughzm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcojdpqkf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gjbxqdlvo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gsabjyxtl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/grjlakbak.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcwxnltdw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gppvncvpo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gfgtukdkv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gwiljvpbp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gawdkczdq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gvqzjnxwc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gglhdufrc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgtdlll.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqpusqofk.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/goiogyxnq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/grvqpxwhb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gnieaqipl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gykwkkbzt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqokjxr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gyyylhcud.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/grskpkcrp.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gviwjyuoc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gulyddorm.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gogbdguan.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/glmdzrric.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gaxqqjtgw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/ggnjkjnpz.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gfsfugmnv.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkedsurgc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gklifpxcs.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/ghkloeqbf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzuvzemxj.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gjxfskwoe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghullzfis.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gzssgurwu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/ghtervsgu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gmopebgjl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gbasiacok.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gehpqjkio.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gekwfruvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gzpbbldyk.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gmenwebfn.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gefgxtcif.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtsuyre.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbkcaymoo.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/grgnnjtzx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/griaqlzzo.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/grikgerhq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/ggwdvpzjq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ggtonlusj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gjvkhbrsk.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrahpxlf.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsytolqn.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmlruxecb.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/govrrrbuo.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghaiuetnu.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gteptnpqf.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqphieptn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gqkgvqsvn.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/ghiheewqx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gvhmtdvgg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gdgwvlqze.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gzbcxfkgd.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkphwuzrj.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/geormogtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/ggquoowmj.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gvnlzjglr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gcmntbmyg.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gygfakwjp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gttfirrkf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/glwkzxqtp.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvguxpehp.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grztsispp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gxkssgapn.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gwleoxklp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gbhpupszh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gkygzlzhj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gptmfisuv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gzdvyowkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghflleypb.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gmtvambem.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxcdnadji.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gfvurozpq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gmfefnqwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gwifoezvc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gbeeuakaf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbrbfhfma.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gmwsiocth.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrfsxggd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gigvyvckn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdjjkrdcv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/garmyalxy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxrapytuc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/giucsnvsi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqsjsirnc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtcypoklf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gwveqpdqh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmutfcqdm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gdjleqzaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gbypwbxio.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqbrejejd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/guuetrmsw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gvepaexrq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gfcfmckyk.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gztirwazl.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gzbpnlzpz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/glyasyyjo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gsbnqqqwx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gsrwcdwkz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gapzanlyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/grjxjnrbj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/giqfibkbn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gzllqohxn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gfendniza.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/glqlnxtmd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gmixizwdi.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gjwqsthnr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gtrtdafnb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gcvkguwkw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gabyttqmv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gntejrgvt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gtnuyhtgh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gdbztkkib.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gniocufmb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gxqixvejg.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gugxyorta.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/giwphrynq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhkgqcty.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gwxwuniyt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gozdsqdel.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gofzoenpl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gqmpgadgb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ghescjepi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gxjlwdbze.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gbtcbdmzr.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gjfstwuzp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gublvgzuz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsvkfabjy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gernprhks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/glwyaqagz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/goozbblmx.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gsahsitjx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gwtablrcz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzduyiuka.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gpzaqlzop.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/giqwtvdsy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gmwwfbkbz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gpuzachwh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gwinnfnaj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/giuiktouo.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/goslijtqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gctznjoep.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gzhncdnzz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/glimufdng.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gwhwxduhe.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gffmjjkye.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gulovbotz.sHtML


<!-- 参考信息 -->