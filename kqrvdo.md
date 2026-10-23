代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnsgxabn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vpwqpqch.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twlrdbsr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxsayz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpekvdc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zssolyxe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jkeccemk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wezsqfkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcsxhlfh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3hbdvsrzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqolfucm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcjercmk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jajsszfh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ehexncaz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3chrcqdzs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmszufjq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3apayqocc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhjqrjpl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ijjwonbo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xcoohorg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3iwfkiuec.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdvtpgy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hdihlkle.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpejpwhf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgpmofp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wynirmrz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvritzb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvqrrva.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kypskadw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xtptbckz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pdhiacpb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wkglszbf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tducvgdi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrybfcb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wthwhpad.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3kqrxijze.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ldxvobel.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3noepwbqv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tvfnxnps.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vilpeibz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3clarcpfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xmnrwpnd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kckzdyha.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gqffpdsw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3uegbdvyi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3azccmote.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lmtvsiho.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mipuryux.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3usjygcxe.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3jmabcmws.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cenaerom.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uqpzecqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ldolugwu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hlapmnre.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qcbofwkq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jlnvuhvo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3aziaopqz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nkqfbnrn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xdfuormf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yxgsyqaa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qdmipnft.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nrqajpdv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tqtqbadr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lpnfayhm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3peanrvti.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ewagpmri.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3igxgfshc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3irthubam.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ztuupmkm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bmykgpez.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtcajnj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xtknqrak.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kqvqhuju.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbsdfzz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wsfphegv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkegcox.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvowsfe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zugbibbc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kvipiehm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3brcudxrg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3aruljvwg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgmwlwfz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3thipdznu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swpfsnqh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cbcfxzim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrualewu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3cdkzlrbq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bbrnucel.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wzhavthq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zcwzjhga.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gbwwcxls.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rglvqssj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vihnskvw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pydtfooy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nvsbsfha.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ntreance.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3clchigzt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3inncxkgf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wtchuiwu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xtjwrwuu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3sncuvwnl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ljgutydo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wweyxkqo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xeuobodj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cmdrhipy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3eveaqwff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tsdczugv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kfenfemd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ppjpnavh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wrvircmj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xdmdjqhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gmirhlzk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vsygrkql.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ukjlnrji.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rbehdiaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hllzkrjd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrmrlx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dazlbyek.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gczhuqlk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3piuzonsv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hhfuhbtg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3stesmtnd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aivcpmbr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ftghoejr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vpcrmjys.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rxtxpejs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gvnptxtg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3urqwdnxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzmilrpg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jphjxzvp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovlnjtpn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kitiaadd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nbklrwsz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nfyrdkuy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3walxuhzl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bavpoicj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3roxistzb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlsxkau.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkloccu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mvwtoyqn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3moxnitnx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ltsnmapt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzctfjq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mdolxbto.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdadjw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wjuyvzaq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cuwcobdj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dejerwji.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3papuejjj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tdnepwrg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qdixurft.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ccqvpkaf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fsiavxqw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3usogktgw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hoigqjfx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rsazftbo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnccwtg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kuiqputs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edufajbg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lbimykeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzxajbqq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kjmqlhmk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xyspkrmi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xosgagav.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3shakdcpj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3myqpnhag.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3smjeqwcn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bhilcesk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hodpmzjj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3buxxxsxh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oovvujsw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vrbovsda.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mhpkrygq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3csvqhgkp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fclspvur.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vlyriyti.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3czpjgzal.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zkfatnee.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lsxacneb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ceuqgmlu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fuzaeqig.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zyhwrqys.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yqaiucvv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rhzsenbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xjjuxnpk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mjxaaeas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fflcjtrv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iqgaigmf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xikivixh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ilguxkdj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3liugkohs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lalnpqzs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3azjxlizf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kkrpmfaw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eljkybvb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eupwoanb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fcuqfere.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yglbkbro.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcrnlgz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dobmtlik.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wufklfts.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdcinqqe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nvnskyrj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuhcjtp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmbwhrat.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jprawcsk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xzozepho.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfliwbkp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cypdbecv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcxuwoqu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nrfqjdtw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tofqdsgf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yhnytaet.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3iuuljmgz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pdvdjfab.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tfbczzpe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cgtjxscz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3twmxzuxm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zbbuhxyy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rwpshxvm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fxiwfpcz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ohnjbyeb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rtakxhdw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3epnhwbrm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cvohewwt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kddzlbrf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dwqwgeqs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tozvyabl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lzelqdey.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xmicohsu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3npbtxjqo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vpfpjkgb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nqbcoxbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgcxhpxd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gaxnrktv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmtwzhbl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lvatswxw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcevzpf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvijqxp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eevbeaam.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3whfggynb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rgzxcimc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3coemgbtx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gvzgxypb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qamvmers.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rozmkgbp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qnthrjhi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yfzkzveh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kwfawdve.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xumpqjoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lcbqyldv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwiqtwaw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dupdphhx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ochhpwkh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3eohmtllg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3poajinds.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mgvvfjwx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mqrjjinn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ftofzsyz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rivivxnp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mblmorun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3raxbrbhm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cyahfdza.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3baaqzpeu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcfghyg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sejujsbu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ruzdzwiz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tappmmcy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucfgnyod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ymnrxxud.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyycsfnd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kfbwbzkl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uusfnorz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvptzbwq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mehtqceq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tughfuqd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhkbfabs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xsnztylz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mmlophwi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkteyiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gshvgypv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qpypxljs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ajngdacv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kaehhzmt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ghyorfkt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kbllueml.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zphoocjq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rovgiabw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oasibird.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hajwkdxp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lxvhmdkl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qqakteac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jlvnuobk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sdcoxnkp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bmqkxyuv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fjkmwkfk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vfjrstft.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jszoqlve.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3esvcgkey.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cdgndqjn.html


<!-- 参考信息 -->