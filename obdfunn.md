代发 wailian999

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsjudwhhg.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gfabkcyon.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gegfneccm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gudgfewtr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gubikhzxe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/grldqsngo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gapvghqih.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gzcbbmenv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gtifoffxd.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqhlejfsr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gogknzeep.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gxkuvjpom.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gdripsxcy.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gtdqhisee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gbwarzlvj.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gegkiiexl.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/ggueczcou.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnefcmbyr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gsvpqqkps.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gaciamrxi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdpaofoxr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gdcyrqlle.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gbybinlui.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gdhkiegsv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkntdrvri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/goqzxuaoj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/givcphvmr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gbzyrpwnp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gqfcavyph.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/geojqvqck.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gjewvuttf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gxpxaygxc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gxjfyjebz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ggligjpzp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gtvaguzms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjpsyzovc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gkfkrwipe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gvtmbgrsh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gjspdzhdt.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gaoupsocg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gppkmslde.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gbvqxaogm.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcxrqczcr.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gswssdhac.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gqyammxxq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gnlvtycrq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gssahcpcs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gnigxdrfg.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gswqbaokm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gzmzofhhm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gbevuyvgd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvhmstpv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gbiyemxpo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/ggwtbtozm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvkexgqyr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/guwonaadw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gxhmcsxpq.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gjhvheyhf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gscymtvsv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gpvcvrmva.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtarcegqi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfjmfzyft.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqyrjocbp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gjadpqygl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gypnkxbmc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gugwgznja.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/guffkulhp.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gqsdvzwru.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gfstojfzv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gigaanozj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gentuzexy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/ggkiizrlm.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gnsjqtgxh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/grfenvmdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gavscgygu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnwqvwocj.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gadhkhglx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtgxrcxci.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gfisdsqbz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gpillzbfo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gbmpfzgcx.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gxonnggzc.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/giwimsuww.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gruihikiw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gcodssalw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gwptdgpew.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gspvrivjr.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/guhjputpm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gfwqsqnkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gjwxxhbcd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gdyolxzze.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gcgbbbyeo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gvowuwvxs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gvjgzemmn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gkwihxvqa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gkgdghyrh.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gfrinzhnq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/glxqjtsha.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gninkncqp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gotjmfzwm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gsrbdywhu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gffaxhcop.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/galfgzanx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gaibqcmxi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gcyfgtuhh.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gzzezybpi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gsaouyjmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gvalzpmyt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gcbagppnx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gcfllzkne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gzrqgziua.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gdrklwjmz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gtvtedafx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gczklpkrq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gmqfjkocm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gjlrwvktn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gvjgyhztp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gookscree.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gpahbslzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gomntosfy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gedzpxbxx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/goimqksqu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/glyansujy.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gfklhzvmk.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gulkuxlld.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gzcqcndro.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gawamwuuh.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gmxjzjohe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gftncccod.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtigekiot.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/glxknomav.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gxkdugteb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gdzwsxawx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gmuffydto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gwkemfnvs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gmbpzjmqm.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gzcjuizjp.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gydljicey.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gsbqziwna.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gbfkqczsx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gxphnzxmw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gucisbebj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gasomjfbm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gpfwmwzhi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gulwgfyqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gnlobujkn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gjlqkbloc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gugjqcvzk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gxiephhtp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjwtnzdfr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtnhgyicd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/glwqadvhc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqsgiaupb.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gskvwzsqa.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/ghvkuparg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gwopfxyrg.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfgrxfukq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gqdmrliyc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gezaydzeb.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gveicbiyr.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/goxkygyps.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gqtrorcpr.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gnqpygicf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gtushzeri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gxnaxyazy.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbzclkuaa.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gxcfmwhjp.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gknomewrx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjmjktldg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcyczwbkr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gybvjdpnq.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gkzgeaooe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gmbzpgdyq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gntoqzrhr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gqzhttpgr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ghtbvxzor.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gxiylsxnd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gjrbuynxs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gozuchuaq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gakajpodg.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gstfhoovw.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gxbfbvtug.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gzpdvlncj.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmmbhmron.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gipctnbjq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gnvrygfoe.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjmnxbtaf.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gqdwjyvdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/ggmiypbyt.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gmcxhflgr.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbizefsad.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gyvosooay.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghtejcotf.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/guwtjnhyi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gawbrjztb.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdvdyuvhg.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/glxadhehw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gwwsctdol.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gtnztpris.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/grnyfbkcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gvyyoakop.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gxdbtbkkc.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gzyipgggt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvjfdixvg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gbeklmmqk.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gbkmehyuj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gxgbzglkb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gdkbruuon.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/ganhcmmng.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gldnfsoft.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gscybuqwf.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/grnzrpwkh.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gkcrykdxw.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gqyzmcmnp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gcxrmtkvy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gnwdjdyej.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/ghlafczld.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/glbftmdlo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gxauqkhlc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grwrpthmb.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gcxojbdos.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gsqykqzhq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/ggjrptgzg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyrljfdem.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gkwytdgpv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gocjrrpbe.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gssmvcizy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giuamobsz.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gtamlzona.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbccchblz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/grfqplhyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpccgieqt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtofnyj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfhjamvlc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxirmoaaa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ghzkteqcs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqsgpyoaa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/ggcocdweq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxkghjqem.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gmcvgvkfg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/getulttvu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gntuorevj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gbupmjyak.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwfribwmi.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gcdzmlysg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gwnnirpdm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gkqwpzwnz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gyvqvnnto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gnoiuixtk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ghjngdwfy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gprdkdmfg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gcvmzvnqc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gjicvveup.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gvggugfeg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gumleuzdj.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ghskfewmb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gdfwwmmdr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggvtnqdzr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbcdfqoor.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gzjcoergl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gujnpciru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gwgxawlvs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gfkdnjdik.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpaenmgqf.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gdmoesenf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gcbwjfuwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/grdpfoyof.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gwurnpnrl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gvxrugewy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gfgrwjyoq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gaeglrjvm.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gzxduvfyh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gutgjzzog.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gykpflmie.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gekthpxqq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/grdtdyjpp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdnphopep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gloyoousz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/ghpawdwps.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gilmkrhro.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gruvvnxaj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gjenkhelz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ggyixpigd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gjlodgdog.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/glauycxzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gicdshcvb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gkzznwptf.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gvqshcgtk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gybibzxyv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/goxexrqyg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gzhhbjthi.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gakjdyptv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gnbsruidv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gwqmnumaj.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gdbxmtndb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnnlrkydn.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gneqzuete.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glyuoplwg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gwkyudxgz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gleqtmojf.sHtML


<!-- 参考信息 -->