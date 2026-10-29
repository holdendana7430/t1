代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gjvvgupfl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gauqyuith.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gbahdtngh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gdoqbegyi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/ghruumkwx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/goecqscnv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/grgikkudq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gmwanwzqc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gtvbuvwtc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gucdvakxz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gxawstdrd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gkvfecmhe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goenkuskl.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gnjvmdnmk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtkjdzrve.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/glriunzkk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gjqesesso.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gmclpksod.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gspdzgtyi.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gcezwdhxd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gbzsnkbub.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gpwiezgbn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gjukrsvgd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gnbsgpbsq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gfffeslpo.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gjwwwzuow.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gdyolvtbq.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gwslgmdqv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gahxjnnww.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gbwixspjl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/glfvrjiqz.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gbmobxhae.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gntwfbfmd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gxdjhacbr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gjjenqlaf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/ghuabpsnn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gxsxuorma.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gohwledtx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gwterfggn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gilyhaaty.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gnbkgbumc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gcivsilsw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gavqpmgid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/groeemzms.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gigoqvcdq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/giaijydku.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/galirihwi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeluzwbh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/goaoczfjb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gobebhetu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gdjwhkzxk.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/ghstausnv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggvfnsmac.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gcdmlxxkp.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjspdjavn.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggzvennzl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gukqafdza.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gffjbamit.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gxvuamjuf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gbzazsjai.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gesuktttm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gvxcugisw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gupfyxswp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzgullhvr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gwrmlpsap.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gyezdcxpp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gsgcptdow.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/glrnenijo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gqvlimskv.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gmlyjspqy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ghlrykwmb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gyoxtnskv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gptnufblv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gkkwhlvsm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/glrqemall.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gxvtwlacc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gvdbfmnxe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxjufbgwb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/ghpazzhwq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gvzkvdbxq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gfqsvcsgp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gtpahwhxf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gcbsexvmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gosgprduq.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gmbosifjo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gmepfqeil.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gwgcqvsjb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjtfaayug.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gkzkxlsnd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjisknqol.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/grvikkfrd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gfnpsxoxr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gkrfzvbso.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/ggzbepyax.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxtjfvcv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gownvcnmx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gvxaniorg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gokrdlrfp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gdnieklog.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/grzzzxogf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gwinrytvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gefywbyrj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gyuyrxvrp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gryffbonp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gigqfgiey.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gkppmtjga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gvxidnwog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gqiujghby.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gvlzemafs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ggwiqefwq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/govavknnt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gpcyrnmah.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gvgueckzk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/giwixshbz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/ghjtzzxql.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gmchzdabi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/ghgakpmtj.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gkybsrbpb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gqeffxmom.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gpiokgccq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gugyakuap.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gpnzmlogl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gwfjwycfh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gfkytwvin.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/glkmfqbsl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gzdajmnwq.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gwcmbfngs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gmqeonysl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gyycmostj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyuskhxxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/guzqfxzjj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gyvhhaldo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gyhslpyws.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gurcpxnmf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjuygplfy.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gkqctftjo.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gexyczuex.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gzelrehxo.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gzsipzpjp.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gmkvlpprs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gyajvrdcn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gaagfmwgz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gxjjcdwew.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/giubxmnti.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzzpkwhlv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gvgsmsqsd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gjloqxstn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gstbjelsc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gsvuaovhf.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/grtaisjyz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcuybjurt.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/ggnjebpeq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gtrymvnyl.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gwbqogitv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gcpfexdyx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gayxdkekz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzzsjzerl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjglpjtad.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gkeeqqydz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gikmcobzd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gtearpqwe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gajtonrzl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsmjjvmtj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gxeacllez.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxuxyarlh.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gltbajivb.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gdwywwyai.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gmalrrxxj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gkfuhixpm.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gitpbmbts.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/glogxuuim.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gaseopvzz.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gzcchhysq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gqlhjxgww.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gcurejvgu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gsjfnlyug.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gdvfqcmuw.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvctqusot.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gtzcxzsif.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxtglowsz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbfzcgjyj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gzneawtun.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggojhpbde.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gybdmygdd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gyaxjyagp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gmqfbbqqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/ggirhbljm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gsjfkebjp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gwbdzzoit.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/glayhdcso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gsvxhrieo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gpxquyabn.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gnjcmgozc.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gwrtsfzhl.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gtleesyrh.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gnjbewkss.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfwrzteda.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gcuyvklru.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gflytxiot.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gonrsbwmd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/giiqcnrqk.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gqsybeenf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gydcauxes.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghgcsjiux.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gclfchnxl.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmwwsuenu.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gomtfnhtt.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfxjevpna.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gdoyfuqsh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnpnyyygu.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gnixnazna.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gyhrtwjja.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gwsssuasb.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gipnznjaf.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gegvxurlt.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gytljxhzy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gnaehwbdf.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/giarzkpph.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gstueltcj.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/guposrcom.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gdlsjecss.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gcgcvdtnf.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gvepgqytl.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gmibtqxpe.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gtmeutgrk.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gcftifbhe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/glgjfbodx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gyfffeady.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gyjrlaymn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghsltpuve.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/ggjikqbun.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gcgkjayrh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghbdgenzb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gsvytoahx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gbebpmvlq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gnxhrdlum.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gzyqmzmfp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtibnbeao.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/grtlogqpy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gckgdqiix.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gjgtlmegc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggdicsyza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gecirmfsa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkgsubzjn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gbmbnxrzt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsziqeibz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxqwiluze.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gpimyrers.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghnjprbxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gwfffqsok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gueudiyfc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnzexcjbo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gppwukvhe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtfkrnljd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gsegcqela.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbpkkihao.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gluidkvux.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzojiaucx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gzgdrwnwu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gyazjbyyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gsosqkbyc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gawagcbps.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/grdllmgpm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gekozowgh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gvfzpoadj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gnncefsrv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/ggiuhkkno.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/griipmvvh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkbutrlsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gntozelrt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gveuieolr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghlvqudyz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gowhrrdnl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gmxkviubs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxcyedfwn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvnlktkot.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gyrucbvoj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gjkqmffsp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gzezijvtw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ghnnvzlvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gguyqcrbv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gosbtzxqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gmokvqpqv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ggdlvvycs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gwnszlqbt.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gbmutaruj.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gywnjerdl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gtbplxhft.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvbbzalag.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gdgjkanul.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gtumreqfz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gkhwzkpfd.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gcxcxuqcl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnvgpprsr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gilujuobm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gmnbfptlf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gepldlfdb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gqiltzlll.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gwpysmtbf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gvgbiqftq.sHtML


<!-- 参考信息 -->