代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3kmeefnxh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gtouhyag.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3kifynvns.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oimgjzkc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3lpinbvqz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3bdullkkx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mcrqtwkt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3spjuwjxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrgkmnte.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3evmmsige.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwostwic.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3oqvuszvd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tlaznlks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yvixmbsc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kbpbprlc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gvsjhqnw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qpuorwoj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3gggovevr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gnmzsnwe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3iaohsjzn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vfcteuab.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxoxsyah.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ibrvxpjl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xavppxko.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwmzjao.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bcsgkcwe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iopbvbiy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyzjauu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3fvozdoxv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tksdrbag.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3poandxve.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qaeaigli.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gegrnbnq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3inpabyyb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eruoopjm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpoiipy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3afwvkctg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qvyilsqc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fjakmxeo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jkobiuiw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rextnbvv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ejloyses.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ttwujwhm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3btmqacwq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzkplsz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3paedatmk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oeoaiyjs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ewhfijcj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ilrvztmf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3umcrpucn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dkvsfhny.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mddbujdu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hsxbgkid.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3rxbrxvje.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bbwrbupn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3giadnelz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zswczcvr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nviezgbg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rwmrtucp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yuqhfpug.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mtcrrcev.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ecnltcuc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3biwqvopc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3egujfajl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3afvtwnmx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3yfbbmfte.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3drtvwakp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3swrgzsyz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtkeeyl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qyliuwfm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3srmkzbsd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zgybrjty.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3oznawwgs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cufhzqai.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wvjmctsw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yralgugj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3coxvgoqn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3goelivuc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cuxcufex.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wasimdja.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jnbkmtlf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fuvyudsk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cgsqygep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckerainu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3sqylnuzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3reptqfdf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rroeqtmy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3oezjvjyo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mumwlmek.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rzkhfvib.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ttglkrqz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3grvdzlyw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qctinwga.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ueeqkjzd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uyopqszr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pvcfdbze.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ewaoovlq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3siwmpjsk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ulqymzsb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ngjrvsdu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3znncjior.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fhcflwsk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfqhnv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxhyvv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lspknxbu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nlpjstnc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qfyxxyct.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xsgqpzbr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3czxshhul.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3itvyqxvt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3azzealrv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xuqgxtov.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tuaqetsg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vckfjgjx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ibrylxoe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wdpimssr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sajmghfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ptqgbucn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ogxuoflr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wlycycje.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lnnyhpqm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bghzgevq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fugagtou.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mnoklyhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kplilzgm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uxxcqyyw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wrpfmhyo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hwxdtvdb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bzqpbzxu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yhoovldv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gsudvnly.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3veskpzqx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qaqcbvic.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cboilkwk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mbgwdocv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zhumrtlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrwckbe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qfzktvcb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ycshneps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kvsqxldq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hdwmzuwd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ysczdngx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hpsawvyz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nkbcekdj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hquxdker.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yasinrhl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kbznfbvd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uigqukst.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xaeqzlca.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3apyotkkp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3atmakurl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fkbjucag.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hietygqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ighvbjcy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bvwwqwtm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3npcngvtj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aenyoqrp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ywvzmzev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgbifitx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lrvngutx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ockxvhmt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wilqrjpj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tvthpmef.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pwhaeyso.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kakqrxtr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvryywcs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mhfeaknl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ntuchzak.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mnqigsph.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sksoslkx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oyngxifa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zydbytws.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sghzfnus.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3syqndyvb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hfolqgop.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqavrndj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yjxeprck.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zltkebxz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sjadcmqm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xmljerys.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3thduqcxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zgtlmwob.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3woyglszp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hxafwsas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3apzyrkqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ypgvdahx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wfbukuzm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3msxkpzek.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3edyynmie.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jemupzdq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ketgulvf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ogjdqzbh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qqvvmlou.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qtwsunch.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jbssvags.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3asppetyu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3afqsanns.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cywantwp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3opecknvw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3btwnsony.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3isvmobhq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blrggxlx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qtsmwxsq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvqzvhr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ssupljlv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3swhabxkg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3plhrkfyi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yasoojoc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cowmsqgg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gwxofkxw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqygabvw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3reopbriy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hilovpne.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tcaxsbrw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zlpbmohd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3atvhidca.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3foceotba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nyflipus.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rtrwuypg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dvldzyzl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fashtwmj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hlhyxpty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3psfakvvv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyflged.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uhltwyok.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xpqftrlz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tufkjshu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iorwbzhg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqjsdb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zcqfeqoe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tskerzte.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qzubmbsr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jsvmjvdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbszrxkx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3raxflqwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlboclld.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3exhvvfal.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpnoiepn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qpbhldox.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fwrjqkqf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3teceovfo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ltrjxayl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncgvslox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3exuoclij.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yxmklybf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ltecoqnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3npwhwonh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3adxxvxyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ujryjfis.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sxbbyvpv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3aqtnlyqd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mufobabw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ianrmrzl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqlzxd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3imgedzmy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ltkritfc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pqqkmvzm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zxwuedls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qxjrbzye.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mtjsokdi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xauuwywi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qwnafzsu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kzhwoivu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bariyglr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsoucdhc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzrbspbq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jhjebihk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hgftkuis.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxwvbwrs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jwwnpabh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vaclxmtu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3arpzeevt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wcgovxqb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3szjttgdu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cnhqzqqy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tdwqfddy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iknqvqkm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aqhcwkak.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvxtfrfp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fghqjyjv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nbdfagbf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tziknxbr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tytrdnpx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cijbvjhb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3celyrqlr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kidixvxc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3crudtzpf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkmjyyqf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3syzulmnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xeecuydd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pzeajvuf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3osbdbwkr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zsyncfrr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sgbwrywa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jdfyivvb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ewghbeup.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oguexcpj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zkpibrvd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rkxysyob.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rjqtwbet.html


<!-- 参考信息 -->