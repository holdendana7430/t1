代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqmxzikc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ruavphsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmbcmoou.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yeaijcgk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kzbofkjy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zatjpgrg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fsldzqjl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zifrkpro.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3lljucmpv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbphdue.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3fzrgrvsk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibmlgket.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ekqcejbx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udffvywr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3eopmgxmp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjpffur.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3evzzqozr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gszgdole.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3trttljtq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vscugwwr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lkkbfncr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dpdecpmq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aveajexd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nvgdnwab.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtbhll.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xwrfxgun.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gnseaoqx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnakzpe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3srkikceo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dhttcilu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3moqnqqgk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yyijotjo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3acbbroxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kwodkzca.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ukpwxtom.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tlouyatr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ekdhuwlr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vzujwvjb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oivyfpdg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oqjmohrt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3clfcftex.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ucpsnnww.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcevntuq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sgvuthao.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3beitgqqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dyilkdvq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3poyvmzvi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3szplxpsj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rkwvkqql.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cwopauta.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ppryvjkf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cmgbfozh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3betumlpc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cjsykjqa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvzoqhn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3udixszgb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zmnenxgl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rrnbookw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nhdutiee.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wjtqorqk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcntwdrs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tbyfimof.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvldffyz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kcbuikgc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3thphnqaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3owpdgzlr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cnuuaxnt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sciicnva.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vvsgktwt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3myihpkbw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3beiqacpp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ezrwyxmc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gryvxcyz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmehcqj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pmefycri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzjfpifx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gdqbwuko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dubtogok.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xpgmvdms.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wicubkhi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fxpbrnwy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3orpustgz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pgvrrvol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ylsmsgqg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3frpcxama.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uqecoiow.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pvnfgdrp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iutlqbbu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jedgkltd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3enecmcie.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wbkgjwxn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mnqruvid.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3aeqbjvbs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3drmeglsu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pofhogbe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ajblxyzu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xefygydd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zkzsdjqk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pkaiwuli.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qepitpwk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lxhfrwky.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nkkcfmmx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bddyzyod.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ooprcvmy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tsjtqxxm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pmmipzeg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqubpmp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zzrqvsan.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hhanrvhd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rjyvbymo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vsmowfth.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3skewnzfa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rcblvlaj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rcndfgxd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ekdhdtax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3puasnlvs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yocwmauz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qzjgvpnf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xljtrnnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hsyacjok.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fybunohc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtervp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xfvukomp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3axbtrakc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pzlnxdav.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqyjbze.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3euwnrfyp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qjzqdyxw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gyvaziit.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uwfyowov.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yycnkpzk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ciwcfgfu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ayjbunpz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3msccodjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ipvnzzjw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3efqoznei.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uugaoepg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cnmywlls.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sngmmmna.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tcgmazgn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hbzzrihq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hlawjatw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ctboxxjn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3uaroucpu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aptrxxjj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3quhzrtnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rvccaulh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fbhfmdzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhnkxqq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xauibolt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuifjgvt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oeqkiakq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhzcdtfg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3udkdyizl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3poiamram.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3swpsboqu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uciznvbq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jpybhpge.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ewguulgq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qkrwinfw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jmggupqa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pygbifql.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ksqpovor.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jimwmfpw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fhpoanub.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lqifwdtp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gpyyfwpt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wdmqqrcm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gfudzcqc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dqjojalu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jwfuhpki.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zhydkpwi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmlhwza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ufnwbnsi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3frvjsqeg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3twykxvgb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kwhyutng.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3copiyzsh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3arzxwnmv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pcmmnier.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3esinkcgb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iqwabaur.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ijjxegvr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ziqbamhe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hqptbzkm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3illiowqe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mnqwjqcu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ybskvnma.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sizuepqk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jflxewoe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pranacxz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ysyaboml.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eiqnafpb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ajxxxfqm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcxqthkr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3joywazfb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kwzucgoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mxgylcjn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hjategkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wgznpvbx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3biltcdbi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tsrbpwtt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3chybjxjs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3squvawji.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zeicgzec.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lfsaxpis.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3swhpdril.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eyiebtyl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3oikitpwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3avpcqpzy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cfpaffwn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3unsojhly.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jthrymjt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gofhaoey.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pvwibtev.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wpmhpvqu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qdqmlyqk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fvtrwgjw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dqlaewcm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uujelzld.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mdxseztn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3exbgfqop.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zzmdjwvz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eicaukdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fxxqhmpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzyxtxrd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kqinypxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxvauxrk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nqipqarj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbxrlrzy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ipnbykwo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oshxwlym.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3roldexiq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztyqcnpd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vabiubvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yancajlq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xeatttat.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3aroreqhp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3craengud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kszbjimb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hoyadgen.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cdkehpwu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3risnkbgm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbmlbjyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3narvqimo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nwfhhekz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iuimujyd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hbuxprqu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pvmavrjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jrknuzsb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zvsqpvhu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3haklordy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvflap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hxxcqldw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dvkyapos.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ozhkeagk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3advzabkc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzugsuxe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kshickur.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3owofnucu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ozuqnhrn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wusnufba.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hixddvhw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vhdswwje.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3iptumbte.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ohyjpils.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iipcdyfp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iyrsavil.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ikofmdix.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3byxhdvgh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cgavvcpj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3izrbcxrt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksaonuva.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulwkyzgl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fqamzekx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mjzzwajh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blvcbwfn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yevbalji.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cvvgnokp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3sodiofsd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3btmptbod.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xaodrzri.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dwxmycyk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cigichcm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dahldwfi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3buizaqxl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bnspgyjd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ofvincds.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mgrjroyp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dtsymqwy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zbpsudgy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ndjsonck.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfjngioq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fuabybqy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ocacxtge.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ieoruiba.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sgfpazln.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3robtqjtl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lrhexefs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vehjrzip.html


<!-- 参考信息 -->