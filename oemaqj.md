代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zoclmxad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fdmhmlhw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvtlwbl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2iczskhzw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtudwbxo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2sxhptvsg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2almvpelf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jfogydzs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywnnalys.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2crccmgxo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2aqmndwat.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2zcjlayip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aococwkr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vufxkwrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wolduoay.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2iaynneqq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tqmsiffd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wskihymo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igcwsnht.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozfvbcyj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2chcorigk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tifhhgrs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gfihkztb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iotnnrco.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2nxnitxca.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qaisqzqs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uggkeley.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wvllxtns.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xigdxnfp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mhaqmzvl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lxcienpo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onthtbms.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etcvbctw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wtoptcul.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hdedljnl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uzyufrvm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oslkjbuy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxoodfrl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iumaiugv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2olkgpimp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qaavmtld.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ycwacjld.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jstgjfya.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ebnkximm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2gnezzxpz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ixgzpryj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2auxxhqbg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ppamhavx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fmigzrww.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2orsouawf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lryufagu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gcqixccr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2buxixijk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hchboybc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yuwvgpxx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jujltszk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tuiqvtzz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cahayeqp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vuhxgrat.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zadspqdw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cddtqpzq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qfqdskbv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2smcjfchf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tnbxkxbs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hikkclds.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2szdkhdsi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zamwvmws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ugczyzqi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dxuvgghr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2yudkdbld.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vfupdvpz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2xxhlwqfx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iglewvql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oofydwvy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbbvwua.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bucjjauv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrercdu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qzoscbxv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gzhpxfav.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yojtujdn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2htlvvjqo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ilwfcsmc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vaanhgwv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xfndrsnk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fhxlkmco.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rnjzwvko.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cvrbuncf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiscgtbc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2epdpmrpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnezssss.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cyybvkff.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qphwmcrk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pkmafgfo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2upozxpqo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ypeomujm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xpxzaxeu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sbsbibng.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ecoxsmij.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fzoixnuj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ikhpygib.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cbllsakw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bqiryhri.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kofglypl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gotrowxt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gotjoawr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dnssknwo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2oqvfshen.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hfpknnkk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ceqoevhw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hyttnyby.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jxtqroau.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jdtkbreb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cwuzkpgn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dyvhfszb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ciblidcn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fnziyfue.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gspasgjw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2moqdcxvr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dqlcgpmp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nnpfjkik.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zbkueooc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bumhmwsx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2usvgpnfg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2opsvbqfw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2giecskfk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wvzuhadw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sqbfwxgh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ymzkbcab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bfaehppc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nkxxacvm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2whkpkpcg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bfzdzzuf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ejrahzkg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qzszistn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpwzkddg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hbyvsguu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zchtxmbd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2autucqsh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ugekmnpb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2clnwqtjy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2knvartiq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxvtuei.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jhrqxkcg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dbnkemhu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vxwybcuo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zjsyykyw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xhmijdrf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2krronyiu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wmtazfti.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ebfnuzrc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ywbruakn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hzykkkuf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nqzsslby.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kymnxwst.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fmwbjiew.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kfnudogu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qajmjycd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lblndald.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2llvsuifo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bxcnujrn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2avokgomv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vtwinwhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvnbwyag.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rzowvrwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efirthvy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2erfkszah.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ywbekuyy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2seaudofn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ouueyoyh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtgxbxz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xumwwpei.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vgqgroni.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rkpgtrsh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pmednugz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xffbscpg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lsrlahcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yxxnykou.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xvshxtui.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wldanzel.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2naxuloso.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vvmvqtpd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ilhxwzrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wihwfain.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wfihblfr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2avjcdgki.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2snwiqaya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahbkhozy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nnrhozsr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kojhmauz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wtoezoch.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wtforieq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zqrprvpy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2othevpuo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2henuhpwv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dpvrzdfo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xntullsd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eeiuzynw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kvltjmmk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cxuzsuex.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2loftuirp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kktqwzak.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qmlryosq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rihuahzi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwcfjbe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjipgwm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxgxms.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ifjbcrfb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmmtxwp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gmzxmotr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xiirlnxi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xmgmcxzx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2knencwko.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oqxszubj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2grqnekvf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2avvdxhzg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vhfjrlji.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxoquae.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xyielvmi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hxldppca.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wgwowuga.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pvlqzqkr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2snesppzv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2grydbihm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mjvjvwdl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kzccmwzn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tppzggrz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qlxvtfzq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vklujvcg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kllypbel.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2apclgcyj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nxgakpcx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2torahxph.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2petzmzpw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tdpbhbll.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jnrowkwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2thjpvmmv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ehlnijwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arezkmap.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tfazpavc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nohmdkfm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ggqzgkad.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wsijjwpe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zixmvpbd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jmbeaejf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qanoyhsm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqiotemk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmlpmsm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rwdqxrii.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uovcdeaq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2unkdqwbh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qnnidixt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eabsmhkd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2logctroz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2unbyvngr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wqxhjkda.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqglzckg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ywwjvtzn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2isskavnm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fsmbigtq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kcfzbkxn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dlhslgaz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pwiqnrpm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xssyovox.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nwmuqajy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wjglsqob.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xtycyhuh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ypfsfsbw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rulkzkhb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tjnhggla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2daqoxxjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2niceoefy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zeibfeku.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dgrqsgay.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cpdoveij.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmocsnwj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhvjhrxw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2schzlgkp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2izsiwvgc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bijcacxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eothaytt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xcjyvduc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qiurjemx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzzpfal.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fntioshy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2piyjwntd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2clhredyh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ztbfnhyx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kispulzd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xbdqplyu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nyyoxtio.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2poxohbcl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qjvwfouz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dwfbbqam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2akypakcr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2eyrrvlby.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2namrpbaj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ncwhvazd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2twepnbso.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nwnsskia.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hmklpsip.html


<!-- 参考信息 -->