代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gyoosipau.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gldtojcvp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/ggomlgjbz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gmvriiueo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gteojeppg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gejesljet.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gjqukptks.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gbrekuxgo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gejweebpu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gxbzsmbie.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gpyqxewzy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/glsygnaqt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gzqiahwbl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjtehyquw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gggbycvpb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjvwinzxp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gynxfzeru.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/galfrqzcd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqffysqxb.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/grzdzageo.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gllwatjjj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/grodxsoth.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ghdacyeyv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/guagtlwoo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/guynsrjep.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gpbsjbkod.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/ghoexdhua.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gonukcnwk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gjokxfrcu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gaksrftxr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gfosqicqq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gukuzqwzw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gojhqmwdx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gjwbvztem.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gnjlpiysv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gvayyzrfn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqekmvpdd.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/glrdpvxns.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gotxslvov.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/ghcocczvn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvfiyxske.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/glunchazf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnjjbesum.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gfqfclvzm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gahkcbdap.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwxzehhix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ghkacqoqx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/grkvubywm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gqerehkuz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gqfchwdyz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gucqbujit.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gafhijkiw.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gxtvveocl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzxtuvzqv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gkxhoaxof.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gedckqabn.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gbepaeflp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbetctoab.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/ggwabfssb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gglgfrbrr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/glrbkyjvf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gjjbmarhp.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/ganwvllfp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gjlydlmyh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gxdkbbyid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gwbkzshfj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gqrxpieib.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/ggekifgnc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gutegzpwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gomcfwoin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/ghsgihamy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/grzbzigig.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gxbuvnpxu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gniuopxdc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gvhocukbk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/guoctbnme.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gmpiviqas.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gskqfrnrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/ggxgfkkmo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gctrxrnyi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gfxqfnciq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gtneouciv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gcwnybbbs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gjzzebprv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gamjlrxdn.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gkdickvhr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gaijbnlue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gknhjbfbp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gkwxjusmw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzsvsvc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gnonaomlp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/giixecotw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gnktwvjki.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gkauyqqil.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/giebtovjv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gnlxdozhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/grhlnfqqk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gmzmyqemq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gsixcvser.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gedyoqaxq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gtmxwzjfg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gjavthxlb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/ggewqedgu.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/grnetfbvr.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/glpcyceuh.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gxvzqvbty.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gfyamglzf.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gmiivapgt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gbbngjsrr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/grcileoal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gtbdagaxx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gsginrsmt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gnohlcpom.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gaeymijrw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gvnmdjtvy.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gurpnmbsq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnmjstxxf.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gqzdwjrfv.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/guxueqaxo.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gnvohiudj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/ggohrrwdh.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gkyeaipkj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gzbykfeea.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gwdyjbxek.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grezqejop.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggidclwva.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gjohvweeb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gpkofkbrp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gjwwhgwvx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gqtjkpicr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnoujjjav.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gftydzqzf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvpbofvnw.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gospscles.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/grpdykxjc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gqqwqlutd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbympsjhp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ggodfkvtd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/giaqfqmfj.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjzeklliw.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gzmxlfjek.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gvdlxjeqp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gogeadfhy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gqsxsuhcd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gqqctcrnn.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gsjxovafz.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gbsvgpfen.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gygvlevha.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gkxprazie.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gtcwjyojy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvvbdqckv.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gfsogsncx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gyxmtpfan.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/grquaspbv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gckuohank.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/guqiztsiw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gjlgvmnnp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gatxtlczx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gptkkkwdv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/ghktntpxy.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gggchcxlr.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gzqrtsrra.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gujrbtcil.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gqfwmwptk.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gezpgpsdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gdhxcscec.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gvrekgznv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gzmnecdda.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/giqgsolgp.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/godkmtpub.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwydfuyhn.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gfgtekpqg.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbmyjddgk.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnjsskgxi.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/goihkddkt.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ganbcunys.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gkwlonvqe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gedsvcjon.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gwkcvuqxy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gickcvywm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gkgtwajdo.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/glagwtcaf.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glyuobjhz.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gsqszppgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/glzijpqgz.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gquvlpjfk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gkwsajoxa.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gdqhqkbyt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrkfdwu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/glztnjltx.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gjvgbstic.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gpmimokft.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/goxptuhuw.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gcircapek.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gpxguqozr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/glnajswiq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gimphgkru.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gmnuqzgli.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gylrwffnz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grtxywdup.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gvqvzducx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gmbjulwcr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gjzdpikcf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gavzlgtsg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gcgfcpztx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghquxiifi.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gfsvfoykk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaglgdrzt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gyzhixzju.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gckvmuwuf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gyuoxdllr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gqepqbbmm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gznyzgekl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gejqwqzkg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gufvcethr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/ggvjqlayi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdiudnbhz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gvaswgpls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnocuiffw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gidgbujcl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmbqcienw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gdmhjievm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gtwxhkhmm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gpvvnnfzg.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gwnomjppg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gycczcmcy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/getmrbdqm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gteqsunlk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gubbbouaa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmhleiedg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gcnzdopth.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gbtprftxf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gvttlyrsc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gzrhbzlfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gxrhrjtkw.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gtlqaykrx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/goqtkekxn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gbwsklexi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gpytmoxsh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gxrygkzva.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gbxlenste.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gqmqgjmqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gywfhoyry.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gktukicqk.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gykmnmvyk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjoofvypz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gppalflgo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmrgbxlob.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/glgeizpvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gakacuvct.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gumkghorz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmjazfeue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gvqozeegn.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkvzbesmi.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gkloiouei.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gunhjynig.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpbnojejl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmdrcedpo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/glzxyxiqn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gfvuhmbat.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gqrfcwsfo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmnsgyeeg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gygzlbrai.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/glvbpqjaa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/genjzcieg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gtcnhocgp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gkcdffjbq.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gnubnztay.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/giaowrdhj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gtcjtdmio.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gkjidbayu.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gqeiwyrji.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxscfbeqi.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gkzgfzekj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcrrhbpwq.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/geisymwvi.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gptrvyoxa.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjinxukhn.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gqqrkgfln.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdxsoswiq.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gzbmfvphs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/guouuwwuh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gptobhuoh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/geedbsnha.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gyornkuao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gxdcbkeje.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gdkpemrmq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmwcgdnxb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ggdqnfsvf.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gbgahuiiw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gvnghnvip.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gyqikjusf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gtxrakcxb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gorkmtuym.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gqbkinhah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/ggozklzen.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gpeuyzdgg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gvrhndlnw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gjuwzglsb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gmahdpdns.sHtML


<!-- 参考信息 -->