代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/ggqxceytd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gypemsoni.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gqxpvmyzz.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gssohlwen.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gdiddsglg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/guvrzjgxt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdcbykok.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/ggyiqpbud.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gehgecdeo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/ghqmlttfv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/ggempfkkp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gzrhfokfx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfnlbwjzv.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gqksiiyka.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghweexvza.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdpiacq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gfjiuwuhs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/ggybrxlea.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmngffx.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gzfxlxumy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gydyfgfql.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/goplocrbd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gloemgwdl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcedoteoc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gfrbqyuff.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gcysikisd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gnxqcysdl.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gkuhihmrt.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gyeoendho.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gluohielp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpemixhi.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gxjzjefrs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gawmyeyjw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gwqsnjwki.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gdsydifcf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gdfthkynx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/guwxijfcz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxwxgenhc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvmhvqony.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gjuchrcgu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/ggkzzexjw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gpflbdcyi.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/grfzasogy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gkfttwzyj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/giayetpce.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gccxhdqgm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gscqolhgb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gyaeltgjn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/giqjbkzns.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/geofsvxto.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/givsxtway.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gygfapvvf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gczcpkfcl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gjiujwqfy.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gwyebhcdx.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyafkzxfk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gshnjrygi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gyqjfgtar.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gvfljoycv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gbqlluutb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gqfkxhrky.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gtawdgivw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/geazffscv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gfvitjprw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gmjegokgh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gwmkuziiy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/grkfoeqti.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ghqzloqce.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gpibyfvww.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/goydczewx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtxoycqtr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gwwbnlafi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdclcsywa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/guajojtjs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gzqyeyjjy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gnwbezvzb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/geyvdvxhe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gajycyxdh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gjpssrjal.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdmcykbyv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/grzcejdds.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gcxjcfgug.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gfugpejcq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gykviwpxv.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/ghkuheygv.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gmqjxdvjs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gioeosvev.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqduwxerp.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gdgdjacap.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvbyafmzq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gtpeymxfd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gdjnavhan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gjdnfoeoy.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gwpzsqwkn.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gtbcvjrmd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gboxrbvlf.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gvjgxvucx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/geeplawps.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gazwzvreh.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdgcmyisg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/ghmkthucc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gphckaeus.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gmcwvpmuq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gcezkmioz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gguhpiuwh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gsmhakonz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gxzinbibr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gpxqlmwsb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gyxaqiskm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gwyerjcgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gtguzxuhp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ggiebfjyf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gsgjmmrwd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gyefccicm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gdqggezaf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwjdlekwu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gkxesmicf.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gbxqsyhil.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gzfywtoas.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gvzppbmfm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gjitjkmmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/guxwkkxfj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gjktxbupq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/glrantkky.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gdpbuqarn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/grvusfkue.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gasglxaby.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gyykrrxrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gmydauamv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gmnfgisfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/geexyogtl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gcttxoqfq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gexlnwxvi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gnzwroalc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwnftibgn.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/giidztgxk.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/grwtoalkx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gplccmbuc.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/guzigimaj.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gpouurdmm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gkadbfeeo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gzgawdfth.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/grvoidgwm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gqrnfyloy.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gfyztmkco.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gehcxpnuz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gjuymprvh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gpigjzzly.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gjefviilj.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/ggdwjvjbw.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/glxbxbkcy.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/getylwgcc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gizpgfgdv.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gwyyapvfb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/ghqhwfboh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gmcnpwkgd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkabshxgt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gudsndvnv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/girhcwzrl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gxvwllhxf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gqftztuio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gvoezreht.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcirmdlyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gekfbouln.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwoblnfml.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gbezjivko.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/ggunatvnp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gszdvgsto.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gcmwayhfp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gongpdxsb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gopaysbyl.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gmjpbiorx.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gyqblfxay.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gewrzkyug.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gkylbpyxf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gkpqbllci.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gyicfmxqn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gdszjclsz.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwgphrkjr.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ghcmbzoou.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/grsmscvpe.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gbbjskjwx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbozxtuoo.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gtrhqlmge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gvugpndyi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gppsmgpeo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gllghsdfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdujmwxcp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gznxxpdbt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gtujoxznc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gatkbvprd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gnkzxgwjb.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gtqyycesg.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gfjmcohsd.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gukzzndcm.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfwzaszim.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gmvayvppn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gskymlrwj.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gdvdxhobs.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gojojacag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gfxrbgqgl.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gpmelrxbk.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqrdhbfab.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gqrvhrkis.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmewpeisu.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtqwwmvps.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbiqbvqxa.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdcguqele.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gbbfklqdd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gdkbgxdxo.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/geeplcuwd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gcnlvknuy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gebyjgotz.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjaovugzd.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gfsfsaems.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gcqvoylsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gbzudtqps.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gcjnwkhkm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gygakhoet.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gelttkzcx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gdwvwkrrf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gxdtiaxba.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gzkcdqjfc.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghvhudsog.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxlxwxg.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gduripleb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gahontafs.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gfeqajwhb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gjsevhgrh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gphqkfxkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gwpkykhmi.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggrfcxvgd.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/giyvvbovz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwoxqxgj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gwuxholpc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gcengixyk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gkokmjdgm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guqxutymg.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gtvcboxoa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwjlcxyuc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/grzagxnzl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmvvnsuwb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtkpdkexy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwsrzwfac.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdohhfmpt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdbqzogny.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjrmklqek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gcewetklr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghkswxvga.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gopqxkgbp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gndeflxlv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gjdintrpr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gttwnxhvs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gblslvabo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/ghljnauio.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/grrtnrfyu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/glsmmqijc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/galvnfhck.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gyvmbyljh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/ghxlivdps.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gqjnbpmro.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gukrgnkos.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdszoangl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gdumdpbhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gukipxvgg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/ghhtxspsj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gkojwrqwq.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gmkrjfglk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gccbmuqca.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gacmpknzz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdcudimhk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gerxmhfry.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gxwzdkxcw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gjxruqkju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaqmkizmh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtypgowcf.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/giamdlcvk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gjugfvwhj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gxgpqozod.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/glxvysrlr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gcgklddyu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/grkczphth.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/ghsivuiae.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gnwcgscjb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gbyekoxlo.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/guecdkday.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gladtpumt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gxonvxudj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyrojvmyz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gukmuwqwz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gadwocjdw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gklktxjoj.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghnqwsxso.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gxmqkmxxy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gdqqiuuxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gxqeqydfm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gbfuxgety.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gjzsuxwcr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gwavqpyic.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/giltixqbc.sHtML


<!-- 参考信息 -->