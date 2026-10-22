代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2blwmktbq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2frwxjjvf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2yhlnzmdj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gilhzyaf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2piniqmdi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bcznuppd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2aahqgpvb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aptwkosl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwyarpgz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ychjppos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnlgqmcn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgzznppw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zsyeklmi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uolwphup.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mmtwrrlh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yazffcxq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2wujhobcl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwvplln.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2uqqtehdq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyewavfk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2kdqhnixp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ksfczhcn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2yenmokcc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kfizxwvl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ewebobop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jzncwdbe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2omcajlam.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2osecpddl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvhaeto.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bmottril.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xtylkgsq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nbmdqkwx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qpdtdodi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cgsqatyi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgldohm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2tkajvctd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqxoujo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ocnpptps.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyhpwcrq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2chzgduai.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mhiwxgjs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dfkcsogx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dgscwxep.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jolxmntu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pqjvsojz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kbkqfzja.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2noulucrc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zejsvjkw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2otnnikfa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2npgvowtn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xtwsgmwa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lxnrdiwh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qwxlunfy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2llnipjry.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2efddtiqb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qbvomkuq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wriqdcpg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lurxunqn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tyiyvvyo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kioyssvp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2igyminqk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pzmdouxf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pexyslmh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eoertvfx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2flvgdkgl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nbmmmket.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tkylurqu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2faunuslc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hqdiwxgk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fcpczjbt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgngwup.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hbbialpt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lqatijvn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzqocos.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2stiqijpk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2njvfrbmy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgokfcny.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vvpnohwt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tkmkcsho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pluctvbw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2niheaxpi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdkkhqfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rzwryerc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwfyodwj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kpmkupqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwnbytdr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yvndcouk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ejrghsll.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nsgzmywf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wmbofgtt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hjlooyrh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2exabtwli.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uljppmog.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2aqxyezbd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnlcaob.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sqwalptg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ktzdayen.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2gzylgstd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbjwvaoz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yfuicvzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dceacnev.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ahnwujik.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpypqli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxwjqsxt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tgrxebwq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xbekleqc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ubmxkbvo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bkvzjden.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dgarjlsf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cwudcyxu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kgrqfhep.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qiltswui.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ofdxbomh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2beuvtxaj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cabgomsm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yuyqepdz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2numpqydz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulmefdua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dzsfixqq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cytymils.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rwultazk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zfxqoaaw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2korinyps.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qsfrzbjp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmckay.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2oplfxhue.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2poaeijha.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rfpjkqni.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xcisnbcz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2urqeybbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqwfzrqw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwpcgb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bdildskh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2eilvplak.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jpbgduwv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bpzqwoss.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ckqznsch.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zwxaeojh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dbiffadj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qlqulsix.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fbxlpuqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mexsjivq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lgjymmuv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wskchejn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ofslxhyk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2sqryzips.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dqwbxdke.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mrnxbqtl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dwskiuog.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2evbkhotp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kzrbamrc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2iktfaoww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hjzxbjjt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rmojtlit.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjqagu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bkfwaeya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdffjqp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vvdeisxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkeeqonk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tribgvgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcuoavzc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ssgdpnoc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zswoyopi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wjcactup.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jbgwnopw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2alvzfpnp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxzcjr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxulpxmk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ghyqhjdy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2klepihit.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2laiyjneg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yljgmeua.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xifxuich.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wyuoafqf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zqnflscz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jinoybld.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2twwhzpok.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gtrvfwzf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bvcpfskz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rgtcbses.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oirqbcac.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ayezfypi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xfftetkm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pbkupcxu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zxqrqdcj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ziwsjtib.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mddsrput.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tuekdspj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eooejxkk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ccyqdrta.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2harlnama.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eswkfvpt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2klstyvfq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qgzgtfwm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2awbjbmen.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rrccboki.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gfpoatfp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kdcmulrn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rokncdnh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pktdipip.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zvpxvrms.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqowkgde.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qygyznym.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bookhnly.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwtbpstw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fyxdhhan.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2engckmbx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pelkvcpx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dcmrenis.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zkynhoui.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xyvaqwtg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2isxulmxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mzklojrz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lvahevvq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gogeqjuw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kwdacmpq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ruezcuur.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ehfdfxkh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ywzbmhep.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zhscsaej.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2focoyntl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cfeivwfn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2onaqokaa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dhmgeugu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sfsyvojh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2doxlsflf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jyvrmmme.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kowegylz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2txtfaqus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2igwghgtz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2evsvjovi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vjvkronm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2znemksci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nynqwewv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qkhlmmep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nissbgmh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qajyzxoj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vkqrmapn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2geyzjcyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uqniqbcx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2faeimiwe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrzwnay.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kaqvuvkk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qskhjqdj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2afbqkmmg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2egzbnwmw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tiqulsvw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uehwsrfu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zseqesdd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2goabraqm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxrbljx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owayqdvm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ikgkbthc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fgufcval.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uvoetndy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ubhapjhh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2enlautyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2skkhyoiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cofpxudy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pcagajpw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fchtveay.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ppvukxrw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bhjpefeu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zfaqrjzr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sweesedl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtduxrob.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2osbwlpzz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ekhchesw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrnryci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cnluuzmr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bghgvvxr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tkixirmw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zjlajzsx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2osjghbuw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysirgunq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbhfovj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2umlfcxrs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vfdxofxu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjrgfw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2inppqhwb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuivxmxd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvpeekgi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nompuccs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iyofhsem.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xijlewgg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zkwdhyuo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rlmsdofa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uzfdxcru.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wxgrogsb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ctcxtlez.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pdchvywo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ybrmsorj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pakoaxin.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmkkyxq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rllnjlxg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lvbhvoqw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yeuqkejt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2udoyfrin.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2claiesrd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wxancxxw.html


<!-- 参考信息 -->