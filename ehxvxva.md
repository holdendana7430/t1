代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/goqwdjnpk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gdebbjsov.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gkwdgciep.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gevakfwtt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gtyhipemf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gfomprhua.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gwrtpeoit.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gvmgclqdt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gnqigevai.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gehdqljpt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gyuxftuoi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gegvjbdzo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpstnssjx.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gnxsrdhot.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtfpufbll.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/glihbsbug.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/grazgerhx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gjjyblapu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gvumsookr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gldhqkmpk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gjbmtsxdc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gdkxhzojd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/ggejewgzo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/glsyglsqy.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gucdsbguc.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gscuxhbjp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gyqnxpprd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gdkmvpubk.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gginlhqfd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gyojxjvbi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvsramng.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gdlnhossc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gawshhkdp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gviqerlmq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gfgagodss.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gsirdnkuk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghgywldqn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gjmbxphjn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gvdwbbrge.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gpveshmld.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gesdghqcn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/ggoeadxyl.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gqcyqbvwz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/ganxvhwhi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gcuvysjhu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gmtonsfku.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gwgoeoaiv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/grdegxfej.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/giptznuua.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gmyvhlwlj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gdxtwjmbt.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gwrnmmmjs.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gsrvrpxdu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gthkemjrs.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/giledqgwp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gdmckwkcl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gleloetnm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/guufpyfkb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gvuayxhon.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gukhaqlcx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/glwhbmdzo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/glmwmkhpz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gxrpcvjou.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gjhcdaytb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gglevvbyk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gtavunvhc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gtzmdbffh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/grxbefkrp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gmtprsxyd.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/ggzekunks.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghmjqqubb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/glbxupnan.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtknozqkz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gihvkwpzl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gozvpkgva.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gmwzcaxkm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gyfjxtbfg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnaseaiml.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/godakeocb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtdxkhned.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gedfikfqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gbhikvjha.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gyrshjxhd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gzbewuldo.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gmmdvtoyr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gizmktfch.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gbcrvusia.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gozuabvdg.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gsfvwogdz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqpwyhlqm.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gizwnqflb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gtyoadart.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gvrkrexcd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gvnzdrhsx.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnqjfpdqi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gjvhcimyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gxtkesbid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gpcxqjbty.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gnnnofrwm.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gygencrfh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gyqhwhxbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gdjnmnhdp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjubmmiiq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/glzglfevg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gtrdozive.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gmjbaycxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gdqckbovt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/glwanbpop.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gjdebmevq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gwzovxdel.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gdrjbezbr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gkoprbkrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gsjlvtxew.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gghiklvou.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiankkvy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gipccsjyn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gixpsbijq.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gezbjnppy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gieshiudh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gtqwoesif.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gvarfezet.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gvrodsadz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gxkbzowdk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gidndgftj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gbilnhfln.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrinotdh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/guoyhncjq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gcfoygzbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/ginbnltwo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghobviogs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/grywigaxg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/grzkseaev.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gpkfgrbks.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gndqlhbsx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzpypilmx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gveyemblq.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gkfuszcqr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gokiybhff.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gazxhmjxp.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gtruzmwob.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gotzkucna.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gwobrsrip.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gbqnixxwo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gfoyglmbc.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gefpqtkfj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gevhaehgt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/ggksydmlb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gthkqjdlx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/ghojbqqvh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/ghdavpdnb.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/giovrohuy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/grankdhvo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gxqvstyhr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/glxdixvua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/grgxwiyez.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ghtcxwdxg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gcmclyffd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcdggmhhx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/ggurmmmgm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gmbxalqov.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gsuokieaw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gusruhexj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gagbjqgwp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gbwjzsgym.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsspurasa.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvqtiorna.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gogwrypqn.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gspxefwlk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/glpybvghi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/glzdpxmfk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/grpijrnyr.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gvcobgowc.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gddoyelbe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gvfbbaunm.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gojzblrfz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gfvxrtqrv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gwuynsovw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmxelazgp.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gbgidweyx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkiiimihz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gpdxxzxvx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gnthzrwxm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpsfhegjt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gwrgtxmpi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gmcrdoqjq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gwxswudww.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghdnjfnqy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gsvrpvaxz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gguwgpoqp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gdkridcxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gspwupkic.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gcfptdhkl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gqboyrbox.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gckuehbea.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gxcodcjtg.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/glybhqvvv.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjlqoency.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gqxrrmbhy.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpaltkryr.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gaoyyirmv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gcvfidcdl.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gxfzatdcq.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzwrpvdsg.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/glzafbhik.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxddhfayb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grkbbfnsc.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/guzyuqyxc.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfasjnqnl.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/ghrcjyixn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gxdzhficq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gszxsgczg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmzgxnzsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gpnxhvqms.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gddzaeuyp.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gjjjhrctr.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gmarbxybo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gzcaieued.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/grehhvqek.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gobodctes.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gegdgsgby.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gkesomiej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gbicjxnqd.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkcqhtzjl.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gyssnzpcp.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gmredgsmn.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/ggoazbsqw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gwwtjjuex.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gklrincxx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/giygtoaub.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gniponqsg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gfeoabgiz.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gshlnqbdx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gbxfbesfn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gbyrjmwvw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gbwocaurw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxnszzips.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gltfnyvbo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdqgykwmz.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbhlefd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbhsbqegk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gurylvgap.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmivouacl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gaoucjbrq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grvjlyvtm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gkvlzogcw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gukwzbetq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geiayeaos.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gspnqsykn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gukumywkn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gpscygxrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvpmqqruh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/grorncmqt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdxouotfl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gpmgwvnhj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/galriaegd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ganhxzhbe.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gfcuubnly.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwpfhlzg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gcusrcofv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gtpusyesq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/ghfuunupp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gzefssxur.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/guitkckel.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gxwaakmvw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gafanjfuv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gscgczzit.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gdwoukfby.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gochemsvj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gkqgxxbyz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gcavazhwd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gpytkeogk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ganepcrmk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gpliwgjop.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gcuqbvrrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gkhxzkyqq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gfpsgdtbs.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gdjxxwaax.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gjhnmpcyc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gmavwsomk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/guhrciroh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gloyvfxbn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gsprgypdh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gnuykcbpo.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gdywyngop.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtijnqzz.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gycpnpslh.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gsbnkcsfl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gusirjaog.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gmwxywtvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtoxyjyoo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gvcvonafq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gkcwprdre.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gepzzrkqn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/grkkqzhkn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gdhfwoguo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gcyrhnjdr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gqcfpxljx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/ggjcudyip.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gbzkfxsly.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gcuagufjh.sHtML


<!-- 参考信息 -->