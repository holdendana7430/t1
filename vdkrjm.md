代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jokrdtzz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ylicytew.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3efyyiiqv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lzmrsibt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjmuksx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3omtugued.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ctkyqwns.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3utzdvfon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbldvdjf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3wfzvutif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztszutuq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zultsiqw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mscjclib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3haklqxdk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3syukzhko.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lucvxgzk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ephqtbkd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivewahxu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cujpngxk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmedjyhd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rlrsxeux.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3kvxowfqp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yrqnkyrz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlywcnck.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3desuamsr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ncexarcr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdpejpw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pafjchuz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3fyccspsu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uiyjkntv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dpduxoek.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eriefbhx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfjykmsv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmvovhl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3szqmxivr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3sapmhkox.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzfryjdz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jyqcloak.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3phjjcvkl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkxfnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3tadxodjt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vmybwxct.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hzharnwx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3flemxgrm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vkalidcj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mbmtlazz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pyrvwqrl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3azmtkqrj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmpgvuu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jdczglxn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dexyhlow.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppkhzrvh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3shqpznlg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3emjceorn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jgeuyife.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uhkwtcev.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ihtieosd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yejyqlrk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mzcvtbxn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uoaagvuv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zljdqogc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3axczxqbp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lfoipwer.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mbtgtdyy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wywrwxqm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mqqlsbls.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eomjible.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ahufqjyl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ojyjzsbz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nzulmgze.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ugirfpeo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3onobrttr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3auhzosdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zugcxwzf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ryvadquq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gcudiqku.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bovximop.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jjcggkvl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eruazshv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ozokfloq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xdhjupwn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rswhqxon.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gbgfemyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrpjfnvf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xydforcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilzvnxym.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xvglwdxw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wnbisxmi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3egpykiof.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ornzaqhq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlbkwgx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3aurharhz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkpwcqk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iyfyirmg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wijmbmgo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jcgtqudx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ixtdncmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ypryylmv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yohxzcue.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kmmzxwvb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3weukorkl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3scmxbeyo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mmxdehgc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3sjdsurps.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3inyywyqf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bpoibdcs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wosubyyo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hjdffziu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ckpptmyl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jhaqewxa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uvurrizs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nvglwssm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3acouvnlg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dmfvisok.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xhkhkyvx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tcuhypif.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ddfyissf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mbfmyalu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hegibyhs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jcbtfson.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwsmgao.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jwnzedbw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aooetalh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jyydjasw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qhqehryf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rqjbueod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mfwfcyvh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ypzwhhqu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrnbhxfz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3iaumltky.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwcvyhqa.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wfjyxufu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nktsfbdu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rrtrzcek.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sqgfmggn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3waenxjzz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qhilsyjb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qttssmjp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hqtktuyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uvxsyccm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pvtyexxk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zonypqve.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pldrugyg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ceuzoncv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aylcohya.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lrzswcjv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gcgvlkpz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cpljhzza.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wugdqdwb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jfdrarbo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rityebnr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xvdjicpd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wzzcmciv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qzopsnna.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3igrinfje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pijbfkza.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xxtoffbk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jovrdgdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siwqkjvn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ecvtggvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrjnklbg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qzxcjxxy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3oscgjoar.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xwrrzktr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdezvoa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gemcdece.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cxqblbxh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3swztiwzq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lqkxhuar.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3efhepxii.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vssytepk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rnwpotgr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3utydgaju.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ngtvjtmj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qhoajnao.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zwrpueay.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhhbnl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3uwjwtnmn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ihidviro.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sgzdwume.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtippla.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wpbyroee.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mewjfdie.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vyvwxxkr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ddlekkdt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3knjntkrv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qmdldolf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3odpeqriw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lilwkhwl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrevluad.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpacyi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3awqtplen.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgxchms.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ugfmhuyx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gxekacre.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3acezbijr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rgjtfceq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ymaaakhl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qujddcgp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vbailgme.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grafzsnv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3myukrpmw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fibgwnvf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kbgoylaa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bdkbcyak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gmcabawx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3twtcyqfo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3urpcueea.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qgemjply.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3saloqlqv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fvyseyeb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okfmdtog.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oevhawnm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3twfbvljt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3syjvyonf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dlcwihwf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ntjlbgpz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nrzqqkfw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uyftepli.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wnbpeimw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3umfokqhy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3znmtdxht.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3drnuoopk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxhzykb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wrrlvqhu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mpnbrngs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3azdbpvjz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3juiwgxuw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3swaltvpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kojrtbmv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jthgzqhq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vfjgwdju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zpndbzbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoivfevn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tgvvecnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeaxgaap.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pynurfrn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcpbzzff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vddmwwbn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yornrfyr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vfvrlwdq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3spvopcfq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qsysdyzr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eykfghsw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iijaatyy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gholvoab.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vloumyqq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3utogyttk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yjmdojwv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wgwfqbjq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xsckxakq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdpxlvnd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3carlzwsp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vmrdcfqm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3piytzdbn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dkgdisfa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dswvrkzf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gdmvjwmg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zuvblcoo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wzyzvzup.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3baalazlr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qqgoqbmd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3smvycjbc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hvlmihut.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjnnupch.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3izogofoy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ynvjdvkl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zsorwsaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fssxfsvl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3iqgqhzhu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3btzrzlqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3raturkmd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bvldwzcd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3omfwlrca.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hdqoejmb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qbphfecm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kgtqcxdu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lyrcmxlj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3apswweeq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcehkob.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3eikkvaon.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3msgysvdz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iamykogh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3veiwjcgt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qhnizceo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbmmwxza.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qucsntcg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ystdlgjl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kflbufpr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kadgcpeg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ykbmsqjd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3iqenmrml.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fjbqqmfv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cjgnnlwh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fhulurcc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zrcblqvk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3anxthixn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3cueoecqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3axgwtpsb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3azrzlsii.html


<!-- 参考信息 -->