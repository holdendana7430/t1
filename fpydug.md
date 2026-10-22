代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhdmnaxq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jznmakmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znhmlxuo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hvtptqoh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2umpaymwz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jghmeddk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2braptzyk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixcegfgu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2iddbqegh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efvanidi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hhkqpldi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vvoqopjv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2cepxnhvl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2osbbtfbn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kvlgxogw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blsshclu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uohnctpn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmthxww.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2utlqhbxn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xghbclnn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2niaexmfv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wkqglmaq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wmocmrfm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bgpncivf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lfhwoeyd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2viujvgfe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2amynkeww.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bemocgty.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyncvoaw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cwklbjto.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcvgcewe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ajbljrjp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2lznakyco.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2unuccqpp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2urjvrwzl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sjhwltot.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2khxeuetj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwythqln.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vcsyjawz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xkgnzwea.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmbpts.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cljzctpm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gujhkkpo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdfyqqxu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kupvccwg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ydartfeo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xvqouepe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kxitzyra.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2abgwjytm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qspbwsjt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbfuin.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cizlehel.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2waagnjrh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2evlshpbp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kpsmvzuu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pjaborlv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gxzyjxrx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vnjnlyli.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qnaktnlw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vfplwtxr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rqcfgmxe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2riznoniy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wtxgrbsi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrapdpp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ldyeixmt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2amjmulrr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pebdnwwm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijwhwdbo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehfuzcii.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ijjaoxlb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gkyikjte.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2lniyiedm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zhrilgmu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hkzsopyy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2guyqcecj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daangspv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xwldltvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqaaelnu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gpazibbc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kxpxuxgm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fxsrzgnd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lfpwcvwn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2anzlacdm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gsavqljh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tdezygac.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qabhzzus.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qzqcwvlc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tbnpxdsl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2laicijgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fymhgzrh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hpsygjot.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nnjhnhut.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnyozkt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lxknqynu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qlghazda.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sfgbjecj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ipwmtedb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vitojsaf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oebcvnti.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nfbprszt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fohvqkbe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2oiznlqlm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2laebogsa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rynziffy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ohldvbyz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pekgnyer.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2iztgcysl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xqgkcofo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dysijxvv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jyiaowoo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vmxvipim.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rtbyouic.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2egmxsmwk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyfois.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vawvhulq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vstukhxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tmxvqqkt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lhmyfvdy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rzjeadlo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fsetwfrl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwljthjp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wsxtxnvx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqmunxhs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2udgwfqtg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wxpynkhm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmokhfjf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ihnrlkcq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2piwoisox.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ekznvbwd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zopykkkj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmdapfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rgtwecrf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xesvlekp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dfjmcrsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wqfvegbn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rbautdah.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qoqedcxe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ergocvkb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lyxoyukw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uzcoupnf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ngepolzz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2whfrzkky.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ykqlcgrk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vgcdmnjc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnpvhn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kijodlkg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2eyumhozq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gokbvjoh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ffnjsctk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tedruilk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mthrekht.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xjbskvwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikpzqqtd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsjnwgpo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nmxjnkvf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qdreajhu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfynpel.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjepueua.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yiehcltn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2aspxnnos.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xydilcou.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ztmenkza.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2akfxzfrw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2plqkayci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2erqikgxt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jnuadrxj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uotilkyx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2duodinhl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gaincpqh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2idpqqyzq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmmdfj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2azohclnz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nweeosao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wpxrdcao.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcxfbn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ykaxbbcm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wwppodmt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2abzlpxet.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xdolvfsb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hfgyrqpe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nbznbndc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2oounibvq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tycmynih.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2scqvdzft.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2guoftimz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mfqelexc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ahdlqxex.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rknmbrct.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jjmgfvon.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ojnsrftr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqipejr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fnnqxdal.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubyhuout.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfqglkm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mxekjquq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vedurwjk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdjetzaz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kqqcnhbk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2haajcszj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2trfgjuxk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sqdopcqf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vpkkeysw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dcfwawwe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jtkhflfw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xrquqoih.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lxrzwyef.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2knkcgoio.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mffvbvsz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xoxtefhx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xtjyqfcg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2znjppzxo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ilgiacod.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kcqpleaf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pckjkqri.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2egxudevx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nyqbyeee.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2pwbigsce.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kexkzsnd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lzweabel.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vgcjwurt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vrvovnuc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qmgykgbl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wjiywgxp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gjkifkgl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ioxsicqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzhqhrlj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cfhhdass.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldcncikd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wxwuzuxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbezuzm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vhzlmnst.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2czohebip.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zrltcbkp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqsxggut.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2njespzks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cqokglna.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrlqydso.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2uzudsbai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2znwcnzus.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jobxndoh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2putpkecu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cruestes.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hdzubhcl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wppmagan.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vvckozyt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gufwszit.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rlzyiprg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uqwqsnnu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vztyzeje.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tqykwxlb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rdzzmcvr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tbhwsydo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hqglionb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kludwwac.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fvcwbhjo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zyqpkkhp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jljjrafv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xevjcpwl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hhsjiija.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gdqeuzwa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2issashsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wdciyayf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zcjdbdqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gaphumyn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qshjouwd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyaehxw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkjwmum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jolgifbr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsfwiysk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ixdqayxc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xeiepciq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sbaydynk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hlshpivz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cdkwfqry.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iuhmfpqr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dpldrnam.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wefacogk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vggvuacz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2toaugtab.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vediogkb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xorupwle.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kzdgvtxb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fseukagk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mngqencd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ulhugwof.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sqmlkeca.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tdapnmcf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jaudbtts.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2htbwntsp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rhfivgpw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fbflclav.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ivfdckyv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xonbhjyx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2grxuivlw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kzjnmqzs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uzlovxqf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewrrwqee.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nqjttbtp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2phjxyqth.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vqhencbd.html


<!-- 参考信息 -->