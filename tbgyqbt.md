代发 wailian999

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmwgngqm.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gnqoqkroq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjktdrmre.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gclgykzpl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gsrenctjg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gphyybwcz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gjebrzceu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gnyugqnwl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gvbjtlsgn.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gkzbhlnuo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gjfoejrtd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gqbguqtiy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gwjhwtmqr.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gctdegvwd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gbphjkdoz.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/giqeoysmd.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gjzigiqrk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gznsxsyus.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gjoziwlkw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gkrjqslhr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gghpyqplm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gxjdnhlwz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/glinktrgm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gckhpllza.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/ganunqxgd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gmtadmbwn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gqzorxwzh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gnalwpjmn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gawcnqcpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gporoboqk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gawvvrvfa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gjubfwdiw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gnayskwrh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gflhkkuyy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gexzlphzp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlmpnjz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gpjdhzfjf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gaylhhhvu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gzqfbdszd.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gfckivpby.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdmbrcpgu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gnxixgmia.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghfnbaakf.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/ganybgaev.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gkjyvqdee.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gonlvrlqt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/ghxtbavrr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gdflqjwws.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gyplcgwwo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/grwwgcetj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gludthwpb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlszxxyq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gjsawlgdw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gngyxztno.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gbmkeuyzg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gvgayunat.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ggkscdytm.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gehshvhyx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gsuiccota.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gcfjmmved.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gesgijqze.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ggmbabeuu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdqsxtwrw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gzbgunmic.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gowuvctpm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gkivbgmhs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gbuujlmku.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gcapnusxq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gooifekdd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ggvuctawn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gsthhjvnw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gwgovitqd.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gzzzsbvrm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfgnxtrhs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/goktzryiq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtazneirm.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/grfvwtxge.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzcagwid.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/ghojvqdao.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gkidxwyms.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gsjwxjtmh.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/giibtfbbe.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gmfgdwxsl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/grmyzzddi.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gktmgjfae.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gbmnfbxlu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/ghcpzdhne.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gkusjbqtr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gqppvmpaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gpqnjlhvg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gwgrmcgse.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gygvakpfw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gdfrcmaly.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gozwjddlo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gqpdumcjj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gbpnnsuji.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gbnsxlqrz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrqwnkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gvxrniuwj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gdzxvbxqc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gdlswates.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/grtylupyz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gsrsvnuot.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gsfsnbszk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gqmgtvcrq.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gxpdiwhqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gemrgmmzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gkqhtvrtx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gyugqfhjp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gazomwskn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gtvtbbpqj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/ggpjnitfl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gixfqivns.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gypvfpsbh.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/ghaxfyzvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gzuejsouz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/ghhqnrbds.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gpjhgmcwu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gacplgzwp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gohqzhywg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gqqrusfly.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gojeoziap.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gehuitfar.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gsmjmeqyd.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gphbtgkyy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gjxclcdaw.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gjrnazbck.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gwuzwhbrn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/grnunoxrr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/getukpmnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gykfnekzm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gxhdnwsqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gumuiylab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gyjuafmod.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gbsuvyeiz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gmmmwssaw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/glrocqgkr.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gsxpzfrjh.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghcuufocl.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gxseoovog.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/guqkhankj.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ghssmlphx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gtqmikmrm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gdyelkjmd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/groxevtmb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnifnjvgi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/glgerbgbg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gwcvkcken.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gpbhgrleu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gldugjlau.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwuvgygfk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gpqjqhjwn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggxutcght.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/ghgcdmhkm.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/ghmjtzgtm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gzwfrdiae.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbtozvckr.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/geaezxgwm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gzywlvzvn.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gvbhfeuwq.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gsuluuarm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gcvfmdspf.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmtpnezub.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/ggqkqfkuq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gumgcyfje.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gssmofjth.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gbipljzrr.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfmufrhki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gxmwayogr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/ggzkaigzv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gixeohezs.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gpqqlzeyo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gcbpyothm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gaveemvgr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gcsvhcynt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gpgmaunoz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gfjpdyplt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gwcqxvtxx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/ggukebcnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gyaigxsyn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gkisvlcda.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/grkcyonqr.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gkthssrqx.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwmajftkg.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gqjqvvgha.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/ghekxuoop.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gploiesvl.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gcilxqlzf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gcnauhulg.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gmhcrgbnv.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/grzgxldnx.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gmnroamvc.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gctlmwqjs.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzxqxbhlf.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqzkhjkvn.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjrwcoajv.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqmzkakag.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gpjrevtku.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/goodgggnp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdlynuhro.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gepwojnsm.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gduqlfkdc.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gqbrbbrzx.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gilwttlxd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gkrhwgfdf.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gdifnfmju.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gedotjnso.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gjxczrzps.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ggpdhqkar.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdjptswkp.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gkzdknttc.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gwmohorjw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gsjilykkl.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gzloapwyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gcqviqqet.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gxjtenndn.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gbhttodqq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gcebvotsi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/ghybmwkvp.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/grrxmaayn.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gzwbpiqdv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gbszekjpf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gnttgwgwp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/geeotdsgp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gzoxjwcyr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnbsadppn.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gqjprqiun.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxhlgdjrv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gzvfcztyr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glijufshn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gwcwrayke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/geuwowcov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzorxofub.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gykbrfqfz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdjvacory.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gntxqemrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzkcaknqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gzqqiiehb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gifaquqzk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/ghhopzxkp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/grefndust.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gxnucwfky.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gemwboqxd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gokydzaje.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtlvdoybm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/goysjjnxl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gpjjftpnf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gwksxumpo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gbgxofqlh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxrclkqtz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gvybibkih.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gitdowaho.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gnxpgqibw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gdfjbwrsz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gdlhzafnn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gednavijx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gzviyoewx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gjiuhkfkq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdpsqrjlf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmomybyne.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gxbypjpth.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gddyvyvdb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbspldznr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/genmgujif.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gpqeqgfaf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gboncxqhr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glsjefbdo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gkypzewai.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgscuohk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gvemxidqm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/ghwowtgrn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gqnrfbngy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/ganmojhiw.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gzijpfqgj.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gqbotvpji.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gkpmodval.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtubwiyzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghdopjwyx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gjqkmmkal.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gqngitcyt.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gfyoqqsqy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gahxeqjdp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghnhsvqur.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gkwrybjiz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gqylegzdc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gmzorbdln.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gsergrefy.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grzjhange.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gjohewvlg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gtumettms.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/grqqbwace.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gnmacyeiw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/goplhipgi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gdrwydaof.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjejugzld.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gljpyttkz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwacgdaif.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfipyakny.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/guwsntfgj.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzftbnxmv.sHtML


<!-- 参考信息 -->