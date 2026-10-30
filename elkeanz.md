代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gmkyfhuay.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/glewkywnp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gtmeqanaf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmzosofca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gsxhwpqiv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/glxfcuvhx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gxplbrxta.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gbzcjxmne.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glwkoupvr.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gucwtrkum.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdgosowcq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gogjudtjk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gxaxjqilt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/glfgrwgdd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gltgemzts.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gzlounxhq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gecljvoex.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gyuwtxxrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/grwtlrjjz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gxcdxlqoi.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/ghyzikwtm.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gyhmskbqg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gdvxtklma.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gnbpzhxhd.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gftfjfunw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gkdtuqkcx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gmegpjxaj.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gspiwyzvs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdhvbbhls.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gvugnutne.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/glqurvelm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gxwozfatp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gqdcdcxsb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gfzowooxj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gkvdyuwzy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gtbyofclv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gonzmkihs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/ghxcymknz.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gfirbxggw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gupassybn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gwbbxcznn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gyjlkctnk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gepndvwxr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gijemodzf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gwwnfdosh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/ggmqkwnae.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gjcgitfmm.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gtawpasen.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gzhcxgtwr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gxmhyobqb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjmwwxpau.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyreemqll.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/glscrnqqn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gxezexsya.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/ghtokxqum.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gdmauqlyi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gegfnoewo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/guugdmcgr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/glhbhilpd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ggsdkobhh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrdgwlkx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gnqsdlzeo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gblmzciwy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/grezffnxw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkagbavxk.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gdiytioig.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gyttenwzk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gqakzuwck.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grsbukiid.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gkkeeaczc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gmjrewoah.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gcrvpszao.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gxsaqovso.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gvpxjryxp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gnoxjguxk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gbgojgckw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghfhwjarb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gzbokxaqo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gdcmiuldm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gsrhmqmno.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/ggshpftiu.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpdbpqrvl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gedubyedp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gppshrjls.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gybajumjo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glmvmldig.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gtxwibtck.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gvgjpisac.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gpjxcwwlf.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gyjpknjfp.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdjjtbgbt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gvrlpntir.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gwzxlfhzc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gaiyyzvtu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gaetejbiy.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gdrwfovjo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gcwkvdsyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gspiavpax.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gvpwvcdfo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gkeniasst.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gnkpftzwf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/graiirnia.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gtocsroxn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gdsabmgpt.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/guxsbaqvo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gaiksdhjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gfvisvfrz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gkoyhllgc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gldpbsnrj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gsbpqtcib.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gxdjzkkmh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gsxexehfb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gbobucvup.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gliuesprm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gzluwypav.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/glrfpygxh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gzzhvtrfd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gkebqjkjy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gqyavpzgy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gdaihtjnj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gtdycpvvi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gooocjhvx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gnnixwaqb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gavmwnsci.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gojfbanet.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gbnuqrpoe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gjczjtiud.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gjbmmvkpc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/glsulxqjx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gfxtbatdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdlkbrstf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/ggwqsswqr.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/goizwwuvt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gtiuogfgy.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gjlqxqzmp.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ghehssxws.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gejbqosyg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/galpkfgiu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gcyundaqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gcjpcfmal.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gjhconznf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/ghfgotlsy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gdhcgkxnb.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gxallyvem.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ghsxbdxmj.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gfvtakyfh.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gvnqhxxhz.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gdgjkufwo.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbmimgwxl.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gsxolccur.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gejeswsws.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gekedsxyw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/glizpobxt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnuzmlseb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gjffyferz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gllawyajh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/ggeyhyypj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gyzgprnby.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghbypjrqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdkggtvrs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqfqouuzv.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gohyuiyzv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gdealdcot.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaraxqx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gsencfduo.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gmtgqfkuz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gbhjcuoho.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gspbnhesp.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gqkdfzlcm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/glpzggdfv.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gzakrfdhu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ghkxwwzta.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gcvfkyayc.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gudcwvqcq.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gyqknfgzv.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/ggixwvpip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmdzrnhqi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gtlcmawxp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gughanojt.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gbstazlby.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gofqgoaqa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gcokoewxb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbccsoc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gmfvtmifh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gherczpgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gpzfhxwsz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gjwqgmjjx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gsvxkupvk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gltymmirx.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/ghrkblyoa.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqwabse.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/giafqlfvs.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/goylojeih.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gkvkwgomy.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gwdctfskj.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gbsjaegfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gptqblsax.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/grbeazxxj.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnlpbzluc.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/glabxaquz.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gopudypkk.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/goniyynxg.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/giacosgou.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gngsgzola.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gjuqjgyfv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/ggtktdukv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gzdbmicxb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gefyawece.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqebpnj.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gxguugopd.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwuvccnvl.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gdtgqqibv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gdxbwmktp.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gmkrdpmyk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gkgllpphx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gwkmsvcun.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gxmfxisdw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gnmjkbyuf.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gteytobha.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtxygglqy.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gboqvjlek.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gqnzowywi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gzpkiggns.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gjbitpmmh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gwmfymkys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/goebbszry.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gxsvqfnax.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gsvxdmfqu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ghxtberfc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/goyucvuai.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/ggbpiakqs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gxqxlepyl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtvnwwpck.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvsoaxagl.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gnhncxobw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsbsbnlxh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gqjcbqyha.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gajwnqxbp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggbcuckfo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gtoxjloew.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gwsypfgbz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grcczdzqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnrwbtyzk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gsjsfjmex.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkdpuozxc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/grjecmejq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gsulgybdf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gwjpmeqjs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtdfcziwv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhwgddg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/glwpizafj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grfioorza.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gpaclyqaj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gvhcpefhh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/guvctrnes.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gthorjgam.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gbopboggc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gztpprypu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzknzbyuc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/ghtiggfgt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gffbavyfn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gugldhdyq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gnfeijxok.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gdsobauht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gorweihpz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gbgssnpit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gbueygiku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gulkytkkj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gzfrtcklt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gpawxwdtl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/guwlwbxwp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjdpbsegf.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gpqekeknp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtnllvawp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gicthgvyp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gcssqkkgk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gljnwvckd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/govzxkbkf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/giabocaof.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gsvfexiev.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gfrydczil.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gaxisqkla.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gwcisvwri.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gwrfpwupd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfynwubav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggvvdcmtw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/grazqtnqk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gllzcrsrg.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/geqapmuwv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gsesorkkh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gzvdmhpnw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gswacrxym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gbgdzxbup.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gekhdzktn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/ggmggibtm.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gghbdqpqq.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gbqyvrpxd.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/getioqadr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gcgqpmpzt.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gfspoaciu.sHtML


<!-- 参考信息 -->