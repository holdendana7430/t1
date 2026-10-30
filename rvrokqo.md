代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gvmyqmxml.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gyhcajsie.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gdlecbfxe.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gwixfepzv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gkqtiybip.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gqwdjrudz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/getydwvye.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/glvqfxctz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gkscuobzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/ganrojldc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gpjjyxaxy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gctmrwgov.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghpccggve.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gljhztepy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gobhqkkoo.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gakzewxln.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/ghmaaheyv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gtlknmdwb.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gopwbjqft.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwujmzfgf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gybzckxzz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfhchuvby.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gfmnwciup.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gliqhmzkf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/ghkesrezu.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gjdnckmlo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/guohzzvei.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gkojnkxqe.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcrxquhih.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gnaoytced.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gnoxwsfif.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gojnkrdrk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gbwmiizkt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gjxhriwma.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/ggixntmcn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gfgaeclux.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gbxaibxrz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gkxdduwyr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/glygoplfh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/guwiaayyl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gesxetlkg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gvaegaibf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gzrfutpcd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gqsxgsmqo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gydnervxh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqnrbybqv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gxhwmaorc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gpnzbppxv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gcxhhctrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gjgfjlyzn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gjfmvpxlj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gsbwtdimx.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gvqtqngey.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gtcvhipxt.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gyqfjkfhc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gcislvxjf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/giowfuzuk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gkunewkud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gvexcqtnb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gceacmjet.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gdojfmcdc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gxwscbulp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gqoitckfe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gyfhgnoae.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gvkgczbrh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gvskurhvu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gikjtlubb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghqarbqmj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gqcurxeiz.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/ggqapkjnu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsfmsbock.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gmwtwssby.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gybkaryom.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gnwinhpty.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvxonizjl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gcqwpmbot.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gbapajejq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gpvaounbk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gjovapnkg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/ghwrsehot.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gtimdnycc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gqiembzmq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gssidxwqk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/guivalrtf.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/glyffqyvq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/glhkvoetc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gtorjdiwu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glfdgronh.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/guilodcgk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geupqupzy.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gbppokywz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gslcczhkm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gomcyfjpn.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gglxobqro.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gqutsqduw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gykwdxxep.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gyopexpkb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gqvfmxpkf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gcntodcxs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gwsldkawt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gfqxokfhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gxyopmktf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gkmffiazd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gajtkytqg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gxidoieif.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/glaoyaoot.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/goxcsgkxx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/glbhajmof.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/godzcnifk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gyxwnvcpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gqruqdwkh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gyvcpahsk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gwrequrwp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gjkbvesyx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gocntyevu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gdchioush.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gdskmcnut.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gocwlncvm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gcnzvlyco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gymlbvxno.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gayiyujfv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gybcqcueg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gdhhypdre.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/geakvfueh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gngmxbafi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gazicsagc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gjygtrmhm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gzirsmykd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/ggttoevdl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gbhtlwiid.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gbvkmwqzt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gujcnixzn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/guzmotnlf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gryziloaz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gddwjfaaw.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gqmlminmg.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gnmznpelj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gspbdqccu.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/giuqwjprz.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gcohjtqae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/glawzlyzc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gwzwzdzec.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gfyrzrpdi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gypxrscqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvhbakyag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gqerzcwbu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gibuigtla.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/glxhtmphu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/grvqfnvek.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/glnjtsqjo.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gzjvaemtm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gheiqqvtx.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gfyfabexo.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gzwapmhzo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gumaibvsb.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/grcvucums.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gcveftujg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqscxtqqt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gmywnirbf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gwaiwjwlx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzlyqxvnf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gkylqekhv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gobsntcju.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gqrvjrbwj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwmfjzfcs.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gugmmwuad.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gulbaodqj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gdjxmgizz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/guatglizk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gyovrsteo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gtwpoujwz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gshwvzlvy.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/glomfmhgl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gahaabmuq.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvunjhine.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvrgkfpjj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gihyunncz.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbcmedayl.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gheelfbko.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdmbpqgak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gmtzocjts.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gxizkvqqj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/givqkcowo.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gsqmilpho.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gafkmxinm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gnuleudjh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gbhtdyzfl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gryrhmmhv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gdwswdeei.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfadbvwqp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/glazgmztg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gvunsaokt.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gieldxemx.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ghnmdjnbp.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gqbciypmj.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/ghboyyaaf.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfkpchlwd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gnckgfnaq.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/ginhpwdlr.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gfzgwylvk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gvhhxjgwe.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gpfwecrvw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkrercznj.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gstehmioq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqqnszvxa.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmnfbvzkv.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwanavfb.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmmmxwcoq.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gfbnymoit.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gjwflkgcj.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gopgtenbz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gaixmupyv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/glhjxmrcw.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gcjhexueu.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gecczkfap.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gdirstxzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gkyjmqcfv.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gjraoplaj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gxnksrftq.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gbcaxossm.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/geakqfhkr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gweqwxgrj.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gayavalnd.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gxgkhwplp.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gnchewscr.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/glzmtyszy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gcoosiddp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gbjkrbxqk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/getejueiz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gfonxcxur.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/ggtrxgmwd.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/govfldqzc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gccdkrokq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gwkxoyrbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gbudfxzoc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gnasbvltw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gydkdfyeb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsmdcgxmr.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gpvmmmcpp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphfkfwdg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/ggpetspos.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gphpgepez.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gkwgzfclc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsiptjysm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzzfssakm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxoqzbivz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqxobmsbx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gplijbvci.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdvvjjklz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gawrpbwaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gpswsbihp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gszqfmnfn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gsgzhobtl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/grwjzahvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxcfrbdza.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcaxslcml.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gxuollrxq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gttemwaeh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gkqsthvur.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/grdfupcax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gxssekqmk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gqivvdoxo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggemtzesz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gdlgxupey.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gnarrxjrl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gqsqbbdvq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gpjrekckb.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gjnnfwhpw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcnneexbd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzsjibylk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxgasgcos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gsirbeqmo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmvzkiqug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gonciucpt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gsphjlsyt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gnojgduml.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gehajkvwy.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guqkleydb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbfusqkcg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwxhjmbxw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvwzoqevv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ghvfrvwdu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gjtnmaqrc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqkugwian.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gopldjsbr.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gkcfujngp.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/grfbwmzog.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/giboxshkd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gwfxdahsg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcprdmzun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/glszmpojr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gesglaegs.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkjdcetdm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gxsgvysvd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gkkxdtbue.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gpsdhwimj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/giioplbtw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/giutolvnr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gdycmkvfl.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gycpbzqtb.sHtML


<!-- 参考信息 -->