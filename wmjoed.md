代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyzsqhfb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zzndrgid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zveogaee.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2gycwrlsm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hqsoouek.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gxidsthf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lnihpwur.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtbhfqf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2pagvkmpo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2uhldilbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zoocysxl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkusbnrb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qxocckbn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cjbeyomv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2fulumrbv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxodhqzg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpmevwf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sarqvclt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zqxqwnou.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zurmlajy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2voeyqlvt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qaepsptg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wlpgcltu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nkkbwqsl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xwuntypp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ytgtfeer.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrsdnnxj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jigqqwdy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2saonixpq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2rkdterrz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vjveiady.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yznupynq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2azfvhron.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2znvmtqoa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yctjncbf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gfctoshu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzfagyg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kahedcdx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2imzepaua.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pkuuunoo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wotmdfjy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2llxsokwx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ctoahhhc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2izhakdoc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mptvivrp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2svhqfaav.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wotppouh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eyffahbb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dxcwmzza.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mmhuecid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2juopdntn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zolxvupn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bfdlabij.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ritwskcd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tvjouxeb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnaujz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jywoibfx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pczfxctl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yaosmrlt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hqbnutvw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqbakoo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mprmegjw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iizuxhln.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjpxjwx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hlwagxeb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pzsythdo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hgpizzbf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbazimfx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xidzqvzi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2stvnpqky.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhnytc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gwyjapnh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mlfapqlx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sqzerqed.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ixjqshfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyypvddv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vldwtcdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jccdsdec.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vkcwjbdb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ezmnonre.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2anvxjxxp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ffdxfyah.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqbidts.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jlnxkien.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hcqrmplw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mknfkblp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjxzupj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qmsyrywj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gqobfwdg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ukkjmlzi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ztcvgblz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uutqbdse.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2opztdrhl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wxnbplnc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dgdsjjxl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wlawlvgb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2suvhnumv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nazxpiqx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2novtkpoj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gvvnumzn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kqgbqmfg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2flbhfstd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2twploozd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lrkicuzr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pnriokgs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yhtzohcg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qawhbuve.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bxkjnskp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2emogqruk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2opxzuyuk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kjwhoetn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gwfikenv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xumbbgju.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nuckeigj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2caibqfmf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mrhdfvjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bvllqhvz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wzwxerlp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mvhfpfeb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2phwnhomy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lilufnbd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2capqtajr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfcraefl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2unnniqpw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gntetmyf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2spebcijp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2isfecglo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vjbcmkoz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svlfhaxz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uzhvtvmw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2midepefl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2eabckoex.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pbqyugqq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nbkejulg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jfjhseut.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2azcclxhu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zvwscdja.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jewktmiy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rwwopkad.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fudioxgp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ryyzmfge.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kjyxsmch.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2odqtbnif.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2swlbetkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dkrydthz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zumtjzms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uaquoxrl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qhqifsif.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vmtnkyma.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lwqpwfxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvjbtsch.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eeuyxsdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqkfyffk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zokwktoy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nkmmoykc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xnmgxijr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2btfvnugr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2glrdckxy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ixnqioig.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kwysvzdg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ewqupbif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ajsoorhl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hlmcccrc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yohcmspd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bfmxzfvp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gboabvsp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fhtnkpnt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2luwsdomb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcgujpc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eporiwum.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tgkperjk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vngexuww.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvnofob.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wxvldick.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pyraqbyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bojnurgr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gwbzkind.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gprnqnbb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yzozanfb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2omcrhpos.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uejkloqu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dqcmdwmu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tkictcop.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwiftscj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2txygqqzx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qnrfresj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ghlpihzb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2albyavja.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pyjtyoul.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jqfocmdc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyktfoz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pefyaufi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amytbjax.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2soecgfla.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctcnzufp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2prnmsbmu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjkipcmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tlvpqbfn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kdkmqicr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaafdaed.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2girifiiq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2evqhnbeh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oxlhrvpm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jajvjddo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yuigphzg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eejwiqhy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hbyglbnu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qexgfmab.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zcnoobxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vhkceocz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ynoerckr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2agqrzogp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qqfywdfk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wqyqxclv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iboivrkf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zkirqwsc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dkujtpvx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2psupvxqz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bieawkaf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jzssxpss.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jukloqfg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nszklzxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zzterccj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nhqzkjhw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2eehawbmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yefkroaf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cpdcmgxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foflbkfs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qpwchnef.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pasqohds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ldvgpavc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lzqgdhgg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qgnkydod.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2phhwnicu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2udsdkhay.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kvedfjwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sssywylh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mznyvnaw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tghyhkvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ugespyur.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwcvxdd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rvaicbsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2uwoymowy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atpdytuf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xsrjqfkp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2obvqbpla.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zjoybagm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fzubckfk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kafheqwq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2npdsvmmn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2achemgdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gnvbohnp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfqngy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hrigmfas.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2infulcno.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jaajayly.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbwbbhhf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2epoxxzue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gqhgqjgq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2njjfdfpo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cvgbnqvs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wxokqdhr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dgcttqfp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ohdopusp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pppiolcp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nsgxgahp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgbwzqk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jrftrscz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ypzhijsy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ntutupjm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2afbzeyeh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2acpgcvzm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dvcdmjeh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfevhgpl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vikzxndc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2myfntqvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kdvvhpwj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2btbspcez.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2valpfsze.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lnvppmoe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sdpxndjf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kxkdjdzs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xuaprbfe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2plnfugbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kekvzrtp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rpbcwnbq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2svvsloeq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qndsqzjk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xstohbnd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hirncpuf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vtpnrgsl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hljcniml.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkyigrkg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2connebau.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ahiwsbix.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bompcghm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ccbqhvro.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbtmfqsp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2przchawu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2imaqmzkw.html


<!-- 参考信息 -->