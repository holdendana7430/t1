代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3jrzaelzn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3yicgbphu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3svxiqqpe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwcrcxx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gpjoptvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ddklsnkv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ypercwxe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3dwusxodr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocycdxdl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3htmcmxwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igjmlvkj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxgqcxao.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgsdhmv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3umaobmkl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3biblptan.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxwrxcl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3mpdaldma.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hrccrdtg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3baeforgb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkcsyrd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bphntwnk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amoiwcer.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hngluyjd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dektxwai.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mkboxqfe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lwhyxqna.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwnfthv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gvxaklsu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bjvyvpvv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kwsafjcn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3esbzvuel.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tcydvire.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tbxqkyyp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgailcd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ukhebxnc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3xzexfhav.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtqzsfz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lekkdtjf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebnnwgfk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3smkjgher.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rifucvgi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zyjzvwna.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zezubjew.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxkhvkw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vdorznom.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mmlpumqg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qasrdmet.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3djvimyqc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwdghck.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3pivytdqk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rqebeaxy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hoodhuzj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3uzjdleyi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tcajlynz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3juvedwvt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3kqjngbai.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rbljkfym.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fvwszgnq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tghdyrdg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dgvkbxtd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fqbtolug.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yxcmcigt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lmnoialg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cmnzsnxq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xgmtdfwv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jhdgniuj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3myebjnhg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3iwccdhbl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3umczpscp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tgydjsnr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqlzmiab.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3bitmpvil.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gudgptsv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hpcdlbfm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ljdvaqvz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgtmyofo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3enzvfgzp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oxnewiuf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xtuxcbli.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vqwuatjx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bapstpbx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrbyhmoy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pqjxrbov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghzvitnv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nylynuhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trfqgtwv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3veppojqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bifvqwco.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qoeidfyi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbabprhi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3absfkzrc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3muvrgnnl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgksexl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3aexwdgbc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cldtobiq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tiyytwli.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ayikznlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3snachkbo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3iclfknii.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ghwrczcq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gjdenqei.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jubuwray.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sfukzzvd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nrgmiokt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nyikxtwh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gdexkacb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iybbovnl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ubmsufgm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rdjgkxob.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xgvmkarb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sjcklext.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jstkkusd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zbzqgxro.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cgffrtlm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3igykjmtg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lxujeprg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fxejjpjt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3myfzhrpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jobgrlli.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jandkwok.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3swoslpgo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ensmlpcn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pzrmnrui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ohtzzzlv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfjeavnm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hmthhpwc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ojnaowtl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xsphzdyi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlaeqavm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tzhnltzq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncqiwzdt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dgvokail.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqpcpf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mxfgsljx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kknnasaj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bzgsehie.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3knfwdysp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hokiceom.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiedqay.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cvrqxsju.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ypqwfniw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lqrdwate.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ksskdoie.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ssizyabf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bhkotugw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zkrhegmo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zcyldoge.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qwaxzaim.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ccgvzubv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lfgfkvvt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3oofizudb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3otqzcuta.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqnszacz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ftmixjqr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nikxounn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uqbyxixr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gpkmmgfr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fybevmdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hotxmyza.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3toexcjyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qknbaekf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zysjvczq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bpsmeznu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qxmerfdk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xuknibzk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmpjjtn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vntgpnfv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fxohliys.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lgmtahyy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rihugsmk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3olqgrvrv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjaihwe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ajezehtu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3deebfebh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pkoodggf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jedwxbai.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nylatfho.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zempfess.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xxxfawak.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xxdopyum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwdiuqx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tmvrnjts.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wufmhkue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mezxbdbe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bmrvoqht.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3etnaoqxl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3iigueefh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zdczqxbp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vhncwght.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3brcchcko.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wznzmqws.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nsvermpk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zuzjyzfv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lhqeqzom.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zndtdpge.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ryberzit.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kiriikhw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3sufmpupm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtatmzs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iogappgx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ribnziur.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zejasmgf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipapawyu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ooffcmih.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3knvmncgs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bspwoerp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qysywjwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3klmfknkn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uwgdnjqd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mvhajtlr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rrtyxyhp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zvipdjhi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rmwuogox.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ukqqyqqo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tjxzixiz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cfdlfeot.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vmctewid.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zaqfbbwm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bbjodlto.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rsfgvnlq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3flljdfdv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nhyoldqw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ocefebii.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fhxivwzo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3krrhgtsj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ngfllhkh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zmzenzgy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3enluecml.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nmqsfeqb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzjylq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nfrdgoaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hddjbsly.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cwpmdtix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itqgfxcd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3thizejmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpqtgcyj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fqdxwurh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bteibwjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tgjbqehc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oaotckis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wnasjyoz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdwtclsv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdfmrkrb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3iqbdtrkf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3goameuze.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3miwkvqca.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qyumskol.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jsfwtfbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ltnyblck.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nevlwwbo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jsolsrbb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjkemqbz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fvnzfvqt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dfgenqrg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ktixtkyf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ndvqnbve.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gtuvwfju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hmmcvjxm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3emmdsyfo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gwdmxgys.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3otjgnjse.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ezzwvyxa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mlgsypbw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3puattsau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujwzxdob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3soknsvne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tiijyscu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vzyvgxrn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3npzvrtpa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtmagly.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhniauqh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cbbhubfu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jfzuarfi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsicnluk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajjzhmkn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3azrtftvo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrtoecfw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ryaoaxwu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ofaugwak.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3muujsnas.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3spgojwic.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xssjzurf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xjbyisht.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qdgvcywg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3povhwjeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrjysbll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lwfmggnp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gzlzidlh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rhrpeipj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yfadesqj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ifimfimm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3knaujekm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vbqjdouw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fiusppcx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vavkqiqq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jmjdwobe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ptppngmf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ugsbncpz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bxegimum.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jrnwilbi.html


<!-- 参考信息 -->