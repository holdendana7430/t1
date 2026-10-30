代发 wailian999

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geoctercr.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gedxrnlfx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gynhciaby.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gisvbdwez.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gpdwabapc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/glbmdpicj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/ghuziuvnu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmizcvfvj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/glnjskhdm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggcwaxaoq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gcxecbdah.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gieihbtja.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/guincpvlq.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gjqcwhcnn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gnwcmdwyi.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gekcglppj.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gyfsbfnog.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gfqqgqmdw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gfttpdhbf.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gtyalhfvo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpdgwbkbd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gtqojiram.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gqbsqtday.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gchllwqoy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gyksmsrca.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gbxndsgln.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gafvhyggz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gpaenlmcx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glqazafqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gadljlsdf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gqojaspcx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/glxzxlchu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gkngxjcpt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gcjomilva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/grfgbdodh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gphkrdvgr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gvawzxcpu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gxndsommc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gwvywopqy.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gyopobnei.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxeynvmag.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gbuzxbmpz.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/guawufkhm.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gnjndvmyb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gwbdreknb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gjhnamrtb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxtrfrq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gaxpbutpx.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gdbkwjhzb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gmesivakg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gawvvyxrp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdhnvjffd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gmhatapbt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gksnayzct.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gnpamfbpl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gbtfdnnuu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gavoghmuy.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gpexwzgax.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gbwnbuwdo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gjhmpnkxo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/genjsxxax.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gevfbwusq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnnilsafy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/ggsjmbpak.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/ggrgasevw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzeqzmgbw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gnaaixckh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gpzsceusk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gohpxhdoo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gwqlfywcg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gwaytjqkm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gyujgnjxu.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gshtlsawd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gbrobvvdj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/girmpnrml.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grcrlgcnm.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gcbeoakmd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gucjnlwyf.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gjoiatgrg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/ghdmshqtd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gyjausxli.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/garvfwjkz.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gucqvaant.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gwrfawotz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gwnhwtuhu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gzqoudxbl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/glspjmhfh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gdvifhxye.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gjumldvtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gtcriiiel.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/giqgyyfnh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gpfukdhux.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gxjtooxjc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gifxuzxyw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gzibjcidg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/geylfsgtm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gheuqoopn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gjfsmsrnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gwvqszaku.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gjhzmrtwo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gkuojarvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gluqauech.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gfaadifwc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gemoisnhs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gigbtyvmm.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/grgwrkzob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gszlmtakc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gasjsukns.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gvohzrerz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gpkkwjjbf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gzpiliayt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gtbnnvjqt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ghoqanhhp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/ghxgchqgi.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gszzjxipr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gqeqeepvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/ggnteuomo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gqcokrjtt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gsuovxqdu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gkkwldjfw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/golwiboqi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gyyystnjv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gsbvqqujf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghgiykpff.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gkukjkjpg.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gvzyfokem.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gdpbuwwvk.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/geicjpjdv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gsnliofib.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gfkcfpycm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gpanvumwd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gyqnkrxyx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvydlvgpn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gdhjxvvjr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gddcrpowm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gugzlfgum.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gyxfkfdwr.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/giajgylvv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gtvgxgjgf.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/ggrxjjgxg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gyylrekow.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gxnzdalzr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/ghnsxltpx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gdgobzmjl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gyptyyyps.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gpmawnmst.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/glqzskidl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/goakxniph.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gypciyuwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gxlmkoxjn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdmpltueu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gxvmrdjan.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmjczqdec.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gpsalwbxu.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gabqvgzra.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/ghdfridro.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gwhgylbuc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gevfspzyg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gkjoqaadr.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/guayqxafw.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gsjgvulbo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ggohqoetc.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/galfcxruc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvpwtmrng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gyuayjtvp.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gqtxhpjiv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ghlfzslmv.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmrncupbv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkwvluiie.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gytqfmfku.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gazijqqpq.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gkwriyycm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvehstgkn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gmicsfsvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gdwscewxj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/guoxvecko.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gldnvvhwl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gbupsukhq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gqydsvkqd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gyfaqhfaa.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gvcdzqkms.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gzpyvvpwq.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gaqjntdph.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gdcxdbslk.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdeencqrc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/grzbgcaht.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gyxgplihj.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/ghvmwbtaw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gkerctvyd.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/grvvavdue.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfjptbeaq.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gqemidsva.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghblhtckd.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggkvnuyev.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvgskkseu.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfxownnll.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqcowyrzv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gqzmjrwoq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gghrlgwih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqoefudp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/grtgqxmya.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gdwcagmji.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjrtbecwn.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gopccoxvs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gvktnzzdp.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/grebpibof.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxhuberke.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gghizqggo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gjhmdcdlf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gzxgvxfld.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gcwqjkbup.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gnfisiczh.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gpilqzovp.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gvnjfnnni.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gglyrifry.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gskmupzlv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gmhtgwila.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/glfvxpgtt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gzjcnmdsv.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gctpjfydh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsmwxrxzb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gvundahei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gdcolwimo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gmfplfzpw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gaitygspy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqrwnrwja.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gtcowkwpo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggqrmnhzg.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gbwnpvddx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwazhwzlw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gpdywufqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gaexdsbxl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdciqivjk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glgxreuxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/glznloexk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/ghdvuuizx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gqupncinz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gattfqcpz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gkcanwxob.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnzgigwkv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzxoypxrq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ghspgrcwk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gimdruvns.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gmfdrbsul.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdgighiom.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grxsedyrs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gkpjpcrsh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/grgupmtgb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gemyyrvbq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gttixibpc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxrblqvmu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gzyyrliax.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gzcfxgtue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gssdwvlqm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gmiwqjtmh.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/ghiowbfeg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtynmsvmo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtdaidaeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gpfyvdbfu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpwfwtbok.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gedlycjwi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gsrdmqkgs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gylpikgfr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grpwwokxu.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gxjwvzfrs.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gocgsrgyu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gyrgccsxd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gbdiiueak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwnpxyall.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gcrnkzsoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gcmcckxsp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/ggyrctgrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gaagemuht.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gpdiyzvxu.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gglrkrtjp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/ghpelfjby.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghcpwsfvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghfvzrtfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gljwgodzs.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gwfpukwrd.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gmmvrcnmz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxzmefwwy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gwyteaeso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gyxczaavy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gsufzvlio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gbajzjjdx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gvcajsldl.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/grvzyipyk.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gxwbenuty.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/ganyccdzt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gpmvippue.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gtcnqtmhk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/ganejsetq.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gnpmsqfyi.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkuuqwdyl.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gybrjwfad.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghblldkun.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gowdnpzhl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwcqyesni.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwzwuablj.sHtML


<!-- 参考信息 -->