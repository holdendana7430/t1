代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gzvefwwad.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/giidgltyk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gnrzecrka.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcgltkrrv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/grpnqqzbh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/ggptzmdta.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gndxwqgsi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gcbffxydi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvpolnkgn.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gjcjfardi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwqfkzyur.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gpjlqrruv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gxuxeymfr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gojdgupmy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqeyipitu.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gouhpkcva.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gykkcseik.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpipjmxil.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gxhhnojbt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/graadcqkm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gikmurddc.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gnuofkccc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gqdgefvzw.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gsglfkpmb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gechggjav.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkcwcwgnu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/grjprnxzq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gjgpwknms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gntpsyfoj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gskxrfwhk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gvybqgxgc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gofejeddv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/glurczuxu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gaqzoscio.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gwuaotdrg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gavbwbqcm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gitzhbkjm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/grdvnzasw.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gptreepim.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gkwcbfooa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gkigzyypj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gqiybgbvh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/goeavehzd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gjofpyqyu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gocpjwzce.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gbkbewsgp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/golejpsnk.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gerwelldm.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gmmeuwifl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gvdjsqiop.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gywyzupov.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gktjnnupi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gelipvfok.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gdtjjmehy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gmovjzpkp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gdiiouzfz.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gkzdgtkwx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gftgvutao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gyxfbtfsy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gqpsvhwrf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gulmzpjjp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gqxghjlpt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gbqjqwgso.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gnupyvaog.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/grakecklw.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gjxbiltvo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gacxpkqnt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gyoedrytp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gyretqwax.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfoxrxqdl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtzadgynu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gxwavigfn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/ghsmekrin.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gapwzcofj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ghjtkmmmn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gtswriesl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghoszdsxq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/ghexkbtpu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gzwdloxsa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/goziituid.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gplqidffe.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/guyvgslpb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gkapqxggp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpetsrimk.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gswkpqtdb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmrrgnngt.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/glzttambv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gdtkjrfnh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gwrufezyc.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gmkyelpbx.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gzadrampd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gzojwywpk.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/guedzhfjc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/ggonqzdtd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gsdteaykt.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gmbygnxer.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gxctcqaje.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gclphgjid.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gdmtjbfgu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gibziobhn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gzkfypbhu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gelgzfble.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gealpxbrw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtssmja.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gdetkajaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gpgyordfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gcggdqstl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gzunmehql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gvvnqktpk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gkbvkmbdt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gnffraucb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gygwuqnkc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gzgggtnoi.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gqrndwreb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gaduhdevf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gspwloxwp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gujsxzibx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gczhjaqew.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/goxtbvgfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/grfatmcfy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/ghutaizmq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvezqou.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gtkylakcs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/guxayaxpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/glaqyjtfw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gnosutxkf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gcfjocjiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gmngrwytu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gmtwabrjj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gapfoewlx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzzsvxnlf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/glrozupsj.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gcdkcvhys.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gclkkcevn.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfyjikecv.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gnhuthtlu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/goczraqex.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gvvnxvnoc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmnrwuqad.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gkidsadmq.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gpaqezfei.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gkcnwddci.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gbflxixiy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbzzqrbcu.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gwsjhzlkd.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/geuupkcfx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gtbwjilso.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ggamjrqow.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gfxmjrrum.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gfsbluudj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gheagfjkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gdpcwqxlw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/guvqabpih.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gitivifdq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/glcfezkqy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gxipkevzp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gbibwxmld.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gndqfpaco.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnmkcpagq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/grbgewjiw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkfyyypnv.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gqbyvbjul.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gsfmhaifh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/ghteaorej.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gruvvctmt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gfvyhjwli.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gvfuzyhkg.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gmaakbkir.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ggcuztvnj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gdhcuoggr.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gkistujsh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwobpzfaj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gglnltgts.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gczffpmiv.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gcvhqcwtf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gtluewzre.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/giasorjis.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gwmesbooj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gorpqfavv.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gloxfvmmm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/glwnlzbhk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gymqqfhbs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gymidzckb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/glaxnzocl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gpyosiyec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gmkqfqqaa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gmyevbexs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gbbgrsdcm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gsleorahd.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gxkwmpjaf.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gmbjejivn.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/giinopdwp.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxldpzvem.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gjydckxuv.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gmltgydwa.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/geknyqxno.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gkgqvidgw.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gxrjvupen.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvfmozswm.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/grzkulsew.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gruhdlhtx.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/glycofxyd.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gujedzlvd.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gluegepcw.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gfbrzryho.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gwuoipwgj.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gaacooham.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggzcibhff.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/ghypofuhd.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gocmunrif.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gkaczbnao.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gdowzybjy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gqpsmspzz.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gqrkceykb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gooqxzdma.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/ggndveqzx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gfnkzacnd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gnpqonoja.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcqezhdul.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gwwmmiycc.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gqexdganx.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbkesgzmk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gozqnrfuj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gtwteixrg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gtfxojkad.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjkezpu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/grlukonnh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gdooobjfp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gyagjcnvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gdixsugqo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gizspdlyh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gcuyezbxz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/ghvglrhmv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdkpxqejm.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gifcfovwg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdykqolet.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/grovbzjaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqmutpxov.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grgcdnhwv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gedhjnglh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gcvcwzrfd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvttsazdm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gufuugmku.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gpduhqovo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gepnnvfrq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gjxrtjmuk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/geteupahq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gfaazcpvh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gbfggcdbl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghsrbyqjt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gnrjettfk.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ggleccdlb.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gipettezp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gfvohgcpe.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gjhqrtjaf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxbirbkpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gdjiuiufc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/giraiwpuq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gatytbrmk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnlumyccn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gkazgryoz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gpsljyteb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gobrzvsko.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gldqbvdmw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gualyrgkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/goapynjug.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gfnvzqfqh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gvthmplso.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gwxdpmytc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gcwjzcpqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gdqlgjyms.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gvqrikhnu.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gzqccoewl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gomvvmipv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/ghtsqhner.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gbdrnbplm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gyrmrosyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/guvwesvkl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsuqccnbs.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gwwyerckf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gugzqxmld.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gxfghrdvn.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gbgyckuej.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gtoikltgj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpvksyeff.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/giovfqxiq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gywcjxyqc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/ggmcrlfkv.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gdxkzhtgi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gawanaegr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gecdevbim.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gicosbhmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/ggquritsa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/ghycuvikz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/goafnyhjf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/guaoulwde.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/giwordqny.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gmzmznjqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gcednrjdo.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gdvvgitym.sHtML


<!-- 参考信息 -->