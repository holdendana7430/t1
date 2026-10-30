代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gmhjchxdk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/ghaejmirb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gnrxcntqw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gnxbkanaz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtvkjccji.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gkhorkizz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjqwiyfci.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/goqhdklyu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gykenlopl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/grjnogshh.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/goetlcvet.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqnewteib.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/glytvmvhc.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/grmigofek.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gdbogbshl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gtvaksxrq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gyqxgmasl.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gxnwigqrc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/ggvlwgywh.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gokvjbrjz.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gmjviehmi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gwnewzngi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gggyaciwm.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghylzyase.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gytqjygta.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gjsfirtgq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gnqesmfxp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gvfghrjmg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/glwoyleqv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gzoeaynhx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/ghcjtklmy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/guxmgwcec.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkmswcrnl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gyfwkbgvu.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gclqnyjbd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gwuxqzpvv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gagmxrjoq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/givvqlqnw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gpfdsgkgd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gdhxtrgei.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gqnaumaaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gzbqgqsfz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gubsvetjl.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gbfqckhpx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtfrwntiz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gxakcuhie.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gkjezqviz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gjqrklvnl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gbrstkfkz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/ggrvhoeaj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gcjkwgogc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gnwuaxztk.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gnqjkrqtp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gaccqnuhy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gtyiduzwk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gtsmuvctk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gitzmyxuo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsvpuzjke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gtlgpbdui.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gcwzlwxda.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gsukvaifb.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gkxoisupj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjgteraau.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gxsrfehns.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gamxrailz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gddvvumos.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gznhslpzq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/giurpmazc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/grlawywon.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gidbpnhco.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gnwuprudn.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gakwdbdct.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gaesvvimu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gbcmpxbtb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gqcqfxlac.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gjllwmgnd.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gofmtkbwr.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gzeqelcri.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/ginawbdpi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guxmtqbqg.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/guqcxfala.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxzxjnujp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gtijjtrxm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gsbceziaw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gqaarjjkn.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gslfbvqfz.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gkxqxcbre.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gtdourduh.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gyewtwiqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gxaxpkcjz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gvuqycvdf.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gsoidzqnu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gppvtfwvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gxwudvrgh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggjofunzx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gznrgcepj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gwlrxldbo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gokwjcohw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/ghitbuzzw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gnezjfkeb.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gsncxhynp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gtucmjbod.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gojrerbxh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gnswpsbew.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gdpuitaax.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gamsssnzt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gfxkmiuhi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gkojudcsx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glieywkgb.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gelthrzwp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gmwgdibue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gyqxotabi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gtrtszcqg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gfiznsosy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gzbhptajq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gomfzgume.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gfpckxcxt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gqjvhrrmo.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gbivmuqbs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gvsnxiiun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gacuxuqft.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdiqjiked.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gorzgiyeg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gjuyupavd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/ggocyrzpp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gdfywckuy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtnejmysa.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gcaptcmco.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gbxrlumen.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gxxqlsvcl.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gqycpiggf.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwqcdkksx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gccdxbkct.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gguaybpaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gbleccoqu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gzvueaboa.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gvjlbeuru.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/grfezqxqi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gcfcfddxc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gljnqjkaz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gbeevuogp.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gvrpjekmg.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gereujtbk.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gnabcjika.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjvdvxrax.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gtpexwxta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/glwitipyu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/giwgnivzs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzxlexyln.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gvikpdrwd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gaqumhgfw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gdcvwvvkd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtsqwqyyc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxgfqrpsy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glfhzxyal.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gcfafnpwh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpsdlbmvx.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gsmzrkdwm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gxtofnmzn.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gyammlppw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvsnphjjp.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/grrwyznuu.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/ghqvqanjh.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gbxqubjyh.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxwdyfpue.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gjyxmgytx.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjrhhhrke.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gengqzxgv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gyhxcokzi.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghgjjkzsq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gbnnnvjlo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gclyouvay.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqhbtovme.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gzkuypipd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxqqannky.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/glshkdsye.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gofqdgeew.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gygbvvqxk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/ggngojxnn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gkihiufuf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gtjntsvtm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/guqvzfssh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/grcftfgyp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gvtmmyvic.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gjkmydzot.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gexzvbrau.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gcdqgcson.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gsjehletg.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghqmlhssw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/groyatelw.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gmohlzzre.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gwarxihbe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gwscltlgh.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gknilelse.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqmqtqouj.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gumkppgio.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqdgbpofy.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmlzmywkd.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gaayfdjuy.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gfxygtpur.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gxmzxojvz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvtmoapfj.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glczrwdtb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggezxyvov.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gekyqyliu.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gspzxrbbe.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkkjvsyrw.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gaxlcgwsj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/grxwobvke.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gesndqahj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gakfirzyi.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gndkgxslm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gbnrjrahf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/ghcmwbhuv.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gtvxbwpcy.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gtqnomkiy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gtyjarkns.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gewdjndpe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gozmbwybd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gwvumqpia.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/guhxhichl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/grbknvrnk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gwazmrvab.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqzrdwjzc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghkprquod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gflejbjmc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gvtbhbazp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/ginfntdua.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gixcdjanb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goatryqtb.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gqkiqnxfz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghutsqbuo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/guzsnqutr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzqmqhygb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvnhdznxb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfphnorcp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gsexyxilw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gosemgowv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gikemitta.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gqcggfpuh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghmfluzqd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gvekzgmgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gonayjyuw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gvvxgzuaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/guufvvcoq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdqdvuwzo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gzdavfqhk.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqjfxvehd.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gmgsmrnig.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gkenyiqqf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/ganykgeft.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gzscwulda.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gvvyhtyxb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gvglkrjrw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gyvxaptif.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gzexydnqe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxvbkdiys.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/givqqteso.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/ghwvsbjcs.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gykkhhyqq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gthgkjvji.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gzulesjka.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gicntobyc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtyawhygr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzdzjgcmb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gcrohnyad.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grefasiee.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gyrkdlgzz.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/grmtywfnx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gtigsapld.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggxkugpeq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/goutfbizr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkgnymjko.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjgkbuiez.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gpiuhdpay.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gkkzopdhx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/glbgzeqns.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/glasuxpsb.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gemlbbrzx.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxaenoipd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkpfseftp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gvcnbjlhl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gzukjdbyv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gbqpdhbns.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gyhgdkkeo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grtwhgdif.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gjkiqvazr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/glvkkstpz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gobohuxku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gxegacowb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gqaebebtk.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/goyohiwzs.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/grtemhshc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gsdropzec.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gwobpuzvy.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gffkimutf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gedratpoi.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gazoyosih.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/geknwqabm.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqfmfvtbs.sHtML


<!-- 参考信息 -->