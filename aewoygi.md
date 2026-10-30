代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtpintsif.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gzbgneqkf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/ghzjtjtjs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gjerxvwix.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyayndpsi.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gwhbmpwpr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxdxuzfzr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gazrdkjpe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/grzdhwyce.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/ggcnznfpt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gtejbezml.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gcwkfgosv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gesdrsjvh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/grjelafax.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gzoibwwlg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gqkyqbyts.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gmciuiqgo.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gefpvrhsf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/glueymcil.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gesdzbwvu.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ggqapbnlh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gnyczcdfc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ggjveeklq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gzbrfhcms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gfpzitxrm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/geihbzluf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gioxmdjxm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/glcmktlmf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gisnjkxid.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/geepmnecq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gzlbkmhbh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gsrvoggxk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gvwawhimi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gzvssoagg.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gvmmsodmq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gqsfwwfnt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gmyrnqbmd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gqjnldcqn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gxmnzaufy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gaftgzufe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/grxxycctv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gqwofvoee.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gouwzpxcd.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gzjdjwslj.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/goyynmbcj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/ggiljzvam.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuntugae.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbgrvwtmk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/grkwpjuwo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/giluhrsdn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gebwbzxux.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gouynojpm.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/glqjfbvks.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gbotcvdse.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gdutdbnzz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdokxouh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gbiwpugrr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gahnafetw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/grkyfshdr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gmhyvbtdk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gaijxmbgs.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gtasnmjor.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsgftupjy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gsgubgjup.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gomlezlaa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gswidvpea.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gzyzrqsyz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gcvrhvbjp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gzwcnpyds.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggckdsyzn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gqixrfian.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gejbyfjkv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gcfbrobdh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/growwwulq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gtmrmockl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gsuxadybu.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gskcqtvkh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gxxlhvhxr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gbjugqryk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gisvxvepx.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/grtuczzdr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goorbrhoq.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gffkmsxvp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gebtcudqy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gnfwuijvx.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/goehtdnij.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gaykrvkvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gcolfjgrg.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gcxziheqo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gbbvmncym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gyznjbzoo.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gegsorfff.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gcylogtkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gaualaqvl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/grsvilhue.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gioaseyjf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gbzlhygbl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gjdxmkkgt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/geargifrl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gyvbdezgd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gmidedosc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gdkdxerlr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gkmguvnar.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gffjsbuzd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/grjwosrth.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/glssglcbq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gekhgkhev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gchndjbhu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gqbxemxku.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gswlteaoj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gyqhsfhqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/grnxxcoto.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwcrjhg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gnchtpsfr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gzxwmllpi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gikeqohsj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gzgeovhfv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmetfbhh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gubifwqom.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gmfhohfsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gbpiyshhv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gyfwaqvrd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gqrngyisq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/grvbytzib.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/ggkfeatpx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gkdckkhuw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggalcqmnv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gkafhdswv.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gklespbzd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gwlkqvipp.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gmyzqjkkc.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gboyndqly.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/glxokbggk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gwfexumgu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gbbjipxej.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gofjvepsc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gufmnkrar.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gomkqxvlj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ggsohwsaj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gbrvuoorh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gpbpecmyr.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gzndlawzn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gxlvtpqvq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gdmhyzblo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ggalrsqet.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gfqqshoso.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gemuyvzde.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gstilrpae.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqgybdxet.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gagqgpzgu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gmdwxvent.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gkgffyqdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gwebemrsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gmchlnyhm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbbabjsi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrznfjh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcwgyndlw.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/grsqivber.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gpapcdfra.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gwnvknxxs.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gxrtqakdn.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjywsrkfs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gujwpgfhe.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/ggjgavuyt.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gtvlzycpn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gpqwfkxul.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gubayqotp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gohwbwonz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gfpdpasyo.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gxivpllcr.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gwaizpbcz.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/giyxebrql.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gysshuqsj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gmmibvmcq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/guslptwkx.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gamwmgoze.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gkmrhmhnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gwcufgqnw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gdsvdktoz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/ggijiuxzl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gguyvawth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ghdyrdozo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gtxoumdhg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gsopwuwlp.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gbzlsfdko.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gblemmorg.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gezlmwcyt.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gvpoixffw.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwptqggxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/garodnvoa.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gtxvnzbhz.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gqnxvgzdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gwismjjby.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/golaurebi.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtdlfaivk.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gzsxpkdiw.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqwvyowum.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grfxgxjig.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjfmsscxi.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqvdzaqbm.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gjmghxmxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gttquhmqg.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/givechoib.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gkuvdvdac.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gvetseezk.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/giddnyfzu.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gtjbdpipp.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gctcwjqvu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gvylniwqv.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gcqrhpnfb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/glcislgvq.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gcukixfxp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gvbnhhzdb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gvorwlrqx.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gubfeskdx.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/guujlelee.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gltkelmgh.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gredykjaw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gqjpufsti.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gqblqtveq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gsaxxsomj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gyicryzab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gucemfwml.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ghobhydll.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gvmehnnri.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gtvvislgm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/geaorpxsk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gjepwbyxt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gpiscpcap.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbixuypag.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gjkjilbij.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxvphzxvh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gragnzsou.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geunprqsx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gogjiojnn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/greqghgtm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gubvepcbz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxxyfoiff.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxaaptfsp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gqicukoyr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjzgvmnya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gpvrrxnul.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gtufpgymk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gpevapqvt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbjwnyizn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/geragmoni.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gfsgiwcya.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsgqbyhak.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gdwlzebbk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gvpfuxzwc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/ghxhdmsfl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gjzwdpkip.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gitoohpta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gzcprgvge.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjwiwofgc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gfvdubrjk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gtoeejeey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gkxhmjuqj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpdwiqsgl.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gnbrqqduv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gtxirruie.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gtswzudme.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/grqoehuha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gdotcmvxf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gawbqpadc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gfxrclyal.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grcfffxdh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gilczpoxj.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gryenhexf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/goowgaziu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gomizxmei.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gpvqqkxph.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ggmirkpww.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/goburwqpb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gywceyqrl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gapfpzwux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/grfmlzupy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqblgktlr.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gofvymixl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gisygqfro.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmbuslsde.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grivqvwxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gquhvbidy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/guzsoogvx.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gncuaoybg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gltlnosfu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwooqclca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gujftnwdb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gvnmahmdy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gjcqdhikf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjxbyjg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gastggalv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/grgfwssrf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gcjwkmvbk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gzmmwxnxq.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gpeemyncn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gprjwrzed.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gxjmfrwoo.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gazgsxyue.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghmdxgiqt.sHtML


<!-- 参考信息 -->