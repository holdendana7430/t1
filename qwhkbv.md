代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3oekxmnks.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkyurat.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kjkrvkef.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axlixrlo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3doqrfmxb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqrwlwq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3youcshno.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrzlrjt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzlrgxe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxekhmp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ckooanyt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsiwgfv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfyvkkw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nhdlzmfj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iucwclxc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dqalmlbx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kyjkepzi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dhusexav.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kyjqapgt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pnfwfodi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fhkopxur.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3owylsvcz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddisxtrf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3mobienpl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogygdsvg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kellpwvf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkpxpogu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3awpguwjc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqarlcp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gjntlhnb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lxjemfef.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mfwpqveg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xiuhmwwg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3etirdgkj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mlvmuybe.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnhmbjl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpyznl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nmayxtyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mqokorkv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fxnrlnbo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3mgfdhzos.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3eulpnpdj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3itsmqwlj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wjqptqeo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fpvendqk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3yjswflew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3usvbedmi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ivfqkvmj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hacitqcq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cnrdwoze.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vqllftwi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cezxvngv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ohxhfnek.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tiboehna.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3evraxqsq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3aenbfska.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3smpafwbx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pkafzcbu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xkrvfkha.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nsibyede.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3anfqqcsr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fnadcozs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kholexyz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bfftynzd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3oaffnntz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3esuaafew.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mxoseprs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpgiuqni.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3heqgrqhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxxbfhds.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lidhsqwh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bgbzlxss.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xrgkthpz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nvmrudbz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wvygcmbt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ganvikol.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rirdybal.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yyfxojiv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sqfpzxkx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3alyhgcel.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wwwwhhuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mlcpnkyc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ukisiefg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ccndhzmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hdediask.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kelcytrl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3engeptcz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vcrtyjdk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3naloznre.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lfmlwnas.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kmontzdx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mgqirrjc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vigfmgqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yanogzmk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mzvexhsw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ikmezhgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cvkgxmvw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dqcswyyz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fbmcjskp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rfzdowzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qoyixpaf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3teacugxd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bpdlvczs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xljxzxqp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkcvtru.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fygaeapo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wmrdiaiv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rfnnlmxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3uezfgzzf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hxaxfeun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ttyiabtk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3aqhhvnsd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wwzzbzlh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3btkjyxil.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gqojjqsb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xrhywdbj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hgbzgezy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qtgfxuec.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hxquvjnw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gtgfcvlp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wuvzufld.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxvxxsa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rjpzarwe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yfxkwhxv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tcswlqcu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3eqopirtg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kntdfcca.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3blwpiltg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cpytkoqe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pamgbejv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pltmoiha.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3moitlrtw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3szmiwdji.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wachztcz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yqccqkci.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sufjbgmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hrcqcacr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ekwaprcp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bpxdnumt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kwwebrdj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3joxoyfja.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xoxgiheo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpsyuhcz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nuiaigyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rupvayyw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgjgxush.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zkyzedlv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hnphdkbs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3izziefam.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnigtred.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xzmhldju.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dnbozmyt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cmudtujc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mpmlcnxy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdtcznru.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rjnnswxs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ezriyejv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wrhcbous.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dbyukpxo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqvftbgl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pgbwvgnj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zyobppyl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3polmwksx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lcostgnq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3youjfjia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qdkccvyu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sttcgqwj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gtvlhlqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ozrjypvy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lalnbjyz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bdudhkfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gldsdczw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hoxclqwh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mrafxjut.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3djwgavvd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eeuuqbsi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmuwioux.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3azfveizn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3debeekpl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bvwcnrzx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vpjguslt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qhfbozcg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcqlxhj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3khjyjmjn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3finxfavj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edfehsot.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsknsysh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3roaoosqu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dljonxcx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mjycoflb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dfserowq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxgrmpk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwfbon.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ixsujqrk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lnrqhrfb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hynqgeqm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wxgocjcn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3epdplpjl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bjmvnspn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gyhcsvkz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ixjeaoye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uxjvpmfx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fhecoscv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tqhyvjsr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vflovsuo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hdskyiho.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yonrnfii.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwoqsaj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ozaovszq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fdokuwfo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nxlbojex.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vzfclrnm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vxvxtwfj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3stldtlwg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vjrcleha.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vmqmxxwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qcpexfhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsvaycvd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zubewecc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnnjvdtx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rgpkkrdc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3niujfagr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ramrwkks.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jihfhgcw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3flnxpmqc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bkgtzdhn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aikpzipk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kglhoofx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3smcsxuyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vscjbkjk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vjcecjyd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tedldqkq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bgvxmqan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ciocflmh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3usqwedel.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyeehlvr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pfkmltsv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wrocxtfv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vlksmlzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tehokcap.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3voulgysu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cxmqvaqi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kmjoqqmp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qpvgqcti.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ajkshmlp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3riehdlzq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yliiytii.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wlsolvph.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jyrtluhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fuvxnvdd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dojfcoti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ivntkjzk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3samqcqxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gedvdmxf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fofpcamk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pagyureb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3stvyxzmq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tyddkonv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bzoqgwei.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3adasakty.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3thxocxgf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dtapojsx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsryzhu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lnndogdm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3htktghux.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3alpcmzcq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hzlpiihh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ebuydexd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ionbknhi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxrzgdmb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ktioaruo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uwhodykb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwtwsgri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3axwpijxx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uadgteyq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qioylvmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ujmahayw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mfpznimr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gimeuuam.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lahlxwcv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vsruubtm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3paxutyku.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cdwihguj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ufwgomnd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wouawkso.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3feytkwlc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kwuqmtfi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zkozqqnv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oaewuagp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hshhjpvd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rrwavyuw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajsgfjay.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wrpltegt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dvjbwuls.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3idhlnjxl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ftmguwzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zkuawbld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fiynbowk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xjvnnufg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzflnowb.html


<!-- 参考信息 -->