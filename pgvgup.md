代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zsjfkpxg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2skvrkfcv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvzvcpk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nssjhkth.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2mpqnsfob.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2oxzumodm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bxsbnspd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2gjxciobo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecbthwwj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2sfckuese.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flyedicc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktshpfbz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xwoqoekx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lrkjqtjz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gbyoifmc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zburinwk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2bdlojbgo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cltmflqj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2qqavcgiw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2innqklrz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2aunegnex.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bdsnssko.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2axkmpvvs.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sheoidwb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nxgemuue.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ntbyjgca.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zonllppj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2igrnwvgg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnpnhki.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xdbghsjk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqbclcl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jfideokz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uqeexdhp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tastwwvn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tllgnour.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rmhgfmdu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrcfipln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2optkqfma.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2uckgvvmo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yjttqdut.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jwqukptb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2wnheblkc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dxiqbmcq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aldvbnmr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ucznrwkn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mukozkjl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wbspfdjs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kgipvdty.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdnurdtu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cyaaepvr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ekcxwsxj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tzefwaqm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zvgtytjy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lsclzisd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bgmnqted.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dlsrmxos.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cdvvetvc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dwtgpeeu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybxewlvs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gyulsrxh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fsqzbcxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dacaynxc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hfuzcyeu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nmmgavzh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nvywswje.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mrnddwvz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ktezadaz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sgboanjc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vogshppw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdacyuj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lqvexzwv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xbozbsil.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2egqjlsus.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvvfmju.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kjddnkas.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2afpnqliw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ntnhdmon.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oqaegbem.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mxydqwcp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fdclnuml.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dthvgump.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwahfacs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2unhlrfvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghvzvczd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2awtxeobw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oprqlxxp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ofmvnazf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pdmpqxjg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2yuzokvdq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jogjomdl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vdlljxha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zwtumynn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bdiocjcm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ksuvxdfb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ypnmdfxy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uaffmrof.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oqcrynww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzkjqd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cxqiymir.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eckacpzv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2csgclfnb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ejkoyten.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ogrcnwfx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ynlpjohc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fjyxzasa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ikfewdtb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qgiaxknh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vunxzodu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2clvnaqxv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yxwamins.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jhidjlav.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tyrugbwg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mabxwoio.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yzpkxmrn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmmgbrc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2iwwcdjud.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dgavoxjf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dahcaqgi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ftmxspuy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ytaxigwq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rtiqqswr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pmvnvhpd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2boozzigv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2akojdzhy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbpdhrly.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zzijccwn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tpczpbvx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nnpykkwl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlkwzsmo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2geeontzq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nqopkhev.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dtvkajxl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xdinrpwi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hklczmbd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hczotksk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkubbrb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ufycjpmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kfpyftbm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxxqrsh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xduzomri.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pftefpta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wrcbjqed.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvrbixf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2efutuocj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uouciifi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kadxgeeb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mqkscvwp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ojiwpkep.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xkeytcsz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ulqxghhj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dsajizfq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pewlrbww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2adqkhjph.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ulpofqqz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vhkraztl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2etvftvat.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kmbgaent.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dxzfualf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgpixnqg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2aomrifyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkmdcgst.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lvgirgrn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2znxmbqby.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2znvhdvqs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfolzgx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgegvrb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xjqkksgh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gmturoax.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2iagweamu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ftrdhuai.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggpbkjaw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eeysrmcr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2njpgfasd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rjzhcrko.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uczhbgig.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wdupnuaf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pczcxxnk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzjcvm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bboakioq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kylqtzbv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hvpdybcr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2neopmixp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qvlhpced.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vbkfyvjg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kiutngyp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jeefmxgr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xfojazmb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kgtmmqft.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rlrhjunk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xjxcxckb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tfocvjiw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hqcpfeax.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lztqgyja.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fqcywqsx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bitutgvq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nqybqiml.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qkxyppth.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zbwmenap.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzugoah.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2iubdfqez.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgokzejp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wapclpnw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwdaxog.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xnvzkwxf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcimvy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2plimrgfw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jmsetlso.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ygvlsfih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ylqrazmb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xdhydcta.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ywcmmlby.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qebfmdas.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2howgcmlw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nyzeovns.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ghrnzezh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jnchkomj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zqtdntuo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fndzcylh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qnsvovgz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yvfsgzig.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2luuhrtyi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ojnvlzpp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uzcnbqqu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zgieczer.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zbwwphaw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2azrbvtiq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ttihmrxs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2modlndwm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lcunevky.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zuosxaas.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ybsdtmso.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wpapjnth.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jojrslkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcgwdarr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pkohqpxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qntxvzli.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tcxdlhgh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzpnypw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pastyuyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2krbetpcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gbprtpmt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2msxusbuc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqoxiup.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bpfqbexx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fiahpvzq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2htvapqtv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rokwhoqx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dbissxbg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjjnidfq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqgpqgb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2himixxor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtyvgjxf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mpkveeru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlxlmmzx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2othmktwa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jrireddp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cgqeothr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xjhvgrln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tmztywbe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2inugqwrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kmjouvgd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hylybrza.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ejgzzfgb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bzdxlkdg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2twvmcwss.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xglhumoq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2azconxwv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hdwschis.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2alexiymb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xkisxugq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jjitaopp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nrkrpzzi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2urxacnhb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hqolervj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcthrtzm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rspubfwq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2puvumyty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmgjlu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tgtpdmxb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xfqbxkrr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uohpkrvg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vzcptmpf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bzjivobo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zoinrzqc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kcrzveqf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2skplhoze.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2udbwvhlf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oadgzosf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cxfftadt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2brfwqsuz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wehgydoo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2puxjnxor.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fmpjdvct.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mqctjkow.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mralkqvw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bbrjhbvz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qmpzaowc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vkpnwaxd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ybjsbsdd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2htxkqnlw.html


<!-- 参考信息 -->