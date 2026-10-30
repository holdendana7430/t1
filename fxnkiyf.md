代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmxaersi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrwvfgzv.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjsmpnvy.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxsundn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjxxarg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnekgsixu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/ghoetwjgc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsvyixij.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gskivyddq.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqolqwqen.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fanxiaobao.xyz/Article/details/guholxgmd.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbktybzrr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubeemhzh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpdwsxgc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gxvllzjxz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqmuxcayy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtzcnfppv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzormpkld.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudihqfh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gfjzuvggu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpgqqpqi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcitbvar.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujywubzd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fanxiaobao.xyz/Article/details/glsleckec.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grhitfgad.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcewamsns.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmbazuwy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxloglc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/ggruackbu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gczebkdjt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzandjqmt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/guptcwmdu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gunoafrxu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxctxyane.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gmihjjoeo.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gzycfsvcl.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gyadmchkt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fanxiaobao.xyz/Article/details/ghieyhxhh.sHtML

JS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdytxjks.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gznrnecza.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwrkphhs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gejcuarab.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxgxtjm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbcirizb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrsemuvc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/ggzokdcni.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamfkktkb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gdarfmmjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxafyvd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrmntjnr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gyleyprya.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/grsqqsihw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/grwelddbz.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmcgefpzd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzftowbr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrskkfax.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gkadlehrf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gvziiserq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtrkqftg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyjfamf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqlporf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/guibedzio.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/ghtaqzims.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gpqzolvml.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblqratz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqybzjbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gtuvmvotd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncaxxndl.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkuzwkoe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gebyicpjw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlsavdx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmcmmdsc.sHtML

L. 网络请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeoakvoj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkyiwcbfx.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/grgvarxrp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhycesgz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gblnqdogn.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwjejgc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyetbchkf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiqyyilv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslicwvha.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmuttsq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqupngezd.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkveyvsa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsyppiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gysvnfzwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/grzuywhpo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/ggixngmiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsatwkqu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwdfqfym.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtulvmmrf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gxealfgwb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/giobjlkwd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gebcbqcvl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gylehpabe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqkbouin.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbzvidsp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/guculegbj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gndzvbdtd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fanxiaobao.xyz/Article/details/gjccbotoj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvefngmfa.sHtML

[L04] 设置超时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvohsdesk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcquisoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwkgyxzi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldygpufk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulahydv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvvyxey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjchwphmj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmtbzrcv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gqsiutlri.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvixitzs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/gfacpnptk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnicxrxhn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gkznxnghw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/glapmwjlk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvjikhp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjljkhxwp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqwwrcqw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmcijotfh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glimxbdcj.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/graoicpcs.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchyyokga.sHtML

JS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gifgyelfy.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gtjolhmiq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrcmnsdv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gfperhhlf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fanxiaobao.xyz/Article/details/golbigqof.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gugmadfzp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaizgfoo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gymyqarxi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbaxowv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gchhlooqc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gesreykui.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoryzwmf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/goquppsoz.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/gybxgdttu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/geiswzrmd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzxkxgfh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/geyqvifyc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fanxiaobao.xyz/Article/details/gosyzbata.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/golhkqsin.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gfkiorqqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/glgmvkhoy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/gcxjafgje.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohzqibhb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmirvfyg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfcjptvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpicxyo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grmfpyfju.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grebuxuuc.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gmzlywzyu.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/gekuvuqyv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzkldemv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/glfrwrhdn.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gpixveyye.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/goytpnuhn.sHtML

Ruby: ARGV
来源：http://wap.fanxiaobao.xyz/Article/details/gjejlnywt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/ghmdixpsh.sHtML

[M02] 读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyizqronm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gevuklypb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gdqwnfneb.sHtML

JS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gfdmpabcz.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gzqkoodid.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdulyrss.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtotzelk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gphaoupqm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/guohwayuw.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/guysvwkcx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/goohncanf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaddhkkby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gotfeysek.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagbbzsc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fanxiaobao.xyz/Article/details/gwllhdszh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/glkmxzfsk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gvihndpiz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdawrnvas.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyovmhnx.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gvjvkstnu.sHtML

PHP:  getcwd();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgezlqla.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlpvezjx.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giekhxvnd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqkqbbme.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gkkafjuxr.sHtML

Ruby: Dir.pwd
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiagdzgb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggckaqiqf.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpggydjid.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpnvzgd.sHtML

PHP:  exit(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmvwtbmg.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwuvsewb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnaonegc.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjefcwpya.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqvmcbquh.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/guypiqafp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/gdygylccm.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gaxlxrrgp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwevmsjfa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbkrddcw.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/geqxfqgra.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gkgmnopgb.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkzozlgh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxhzbohw.sHtML

Ruby: warn "err"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvnqpnm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gdadhpkla.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gbitcvduj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewqzxwdf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxyifmp.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvgamyoc.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdybenmaw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjthvid.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqehwhhri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjenqeqe.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxdxsklj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmhzuzmq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/guecabnpz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbytajcxz.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gfriyyvjj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gpedifetc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdwkamn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwfvsvkx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gjbitneqa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgcuwveu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdifuxzwi.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaswykow.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtblfonw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstifkdhm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gbotyavaw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmbxnojj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqlqjfht.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gmuittzjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjszkmni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkfrxuau.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdannxicd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gzakdvudb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakqbjqrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjazqnuz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjkhqqxue.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvbzyxq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizygynz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxgtaiyq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gikggjkfg.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqsoerf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzadgdut.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwapdes.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gbqyssrka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkpiupjy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjenysgn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gutwzyqpv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gsnltrgwq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdhnrqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gnefdddsv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gpltxlrsp.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkarilcf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhsveon.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcxmcwow.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtqsbxip.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfoppwjgf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gaawwyqbr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gggykwepy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxuxgryu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchmepzw.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizktkcox.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzimzdwd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggxxotdfl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghtlswxyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxemsxflb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkylhqddv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gkyouhnvz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsxikaml.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipuxungg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwpurhq.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfxjzjiw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gywqajakg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/guwkpqfvb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guenhuexq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdjsacjd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzjmxzgzb.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gevbbveyl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/glzpvqatd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddczlgli.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/gklsrsqvy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/gdaamqswb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkapvcdsx.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gydztbiej.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/guzswmekv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gcyvovcxj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gessxrcex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gaucnuawx.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgacxzk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwsupefr.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gwcjehrgi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnujpkqq.sHtML

TS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gvfhftriw.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/goirfsmss.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gjvyyxkyb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkbmlnzx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyzfzdn.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdercvpks.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgmmztxz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/grojxwlab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfsgxffj.sHtML


<!-- 参考信息 -->