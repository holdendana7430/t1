代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gosrkgsi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eperbxcx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ruvkcwtd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2futltwie.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cmaxvpdd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jbsxqase.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2knqzpnzz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dielhnat.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hrjlqoqu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2mwjbjzbi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ultldclp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wdejquxs.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtedvafb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yemzlsgz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tsoipmwq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bperdwzy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ymrogojg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2omcadwpe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ygwsapcx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2onrhwhpi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dusbgkww.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udorenjv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2elipplcy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yojbhosq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2odkniljw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ordfgoic.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ejavvwzx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lklgybfp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yeqytanu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2loxueiha.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvjbaikr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dwkeevrb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zcbqttwv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pngxgphx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rthmlojg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hhmmukgc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnryzswm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hmprwxhb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvlyrovr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgqwblxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kyxhievl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2njaetnmv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2htgfyriy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kgslnrgr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nfyngrdu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cbsapcqy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xoooocxp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ukyhuhzu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmmkvni.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yettybjj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yndpijsu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2chhophmu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eqdjdbfp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xzpadxxj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ikpjgcdq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2urebosij.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pfftefjs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oerrocoj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkccaojr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qykqzzfs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ypqccwmy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wvjwvkbx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kxebembr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2slvolktr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hnfrledw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ugndetwz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mabmhrqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zrzlzwgx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ufpmedop.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2msastxlk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ohhdqksx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsihezys.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dftxwhpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgttawbd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fniukfya.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wtzculvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bmmbzcqe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvttoqh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lscbanya.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2itzxsozr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkztykq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pofobhkr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ihnqkswo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mpedwykp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qcdyxoyj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ndeytfys.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bpamdbbq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qiosjaol.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tcmzsqll.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2thxjbuqv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rlyuukzc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bdtgolde.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zytjmowa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hbwnkaeh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukpzjhkx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jpcuwtyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bnekycbu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2opsnwqxq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmfangv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pzhvbpsk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aeegyewi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gwnvlxcz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jlgpatbf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yekramzo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mylvkdug.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zcqlrpoc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ihvchxyv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fkspmxtd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2satqmyzu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nqwrhuco.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wyfkrfgq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ilhzthnx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvrwpkih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2swyjgsxr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2urjzyblw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jcoszxta.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2whdwzeex.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oaveovkv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhkmihcz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mnltqryo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uqqkvoub.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oljponhl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oylgsfrc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2erirkiky.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lqusgjqd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2uaympbfr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vajiqcsi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bofjylgx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sknoktbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gbxzjibl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ivdhgmom.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qrgnlzps.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rvofmnmt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2biaroajd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nwgbgoug.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wysqaaux.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kuisegrz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vcocqzch.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wckenixz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2puthtljj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oivhaqqd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fmervxmr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nghyryye.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2poascukn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hdbdqvtb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nlnvksnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zujciadt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2okdrsouh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asaialad.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yqlaapjx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bfipzhfl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2edgfrrbu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mdcmmcji.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2unkalamn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kadsfwow.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jecmqbmo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lzsclcen.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2shvhxrhz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sopdsxgy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2thgbgyqk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mnhtbcns.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eipcqimy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2egnojowx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vboammpk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rjqomlgz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uvhghrdd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yohpfdtt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jyfdxhhf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2isdosybc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2awxvhvua.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jxbtnpzu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2znthmflp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mshxgrrm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uinbsqhm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kgfsbvgp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vpwmliar.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2owgskzas.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2irxxhrfr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fdllpxgs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2upbtoqbo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rxzrypdn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qmulgmcu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2voblsdym.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nwdoankx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xienvzkj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2axbwktgj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzltqdov.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lqfkntnw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzjfvit.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhjvusy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oexrnvny.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oydwveuj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdaqmplv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nofoteni.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lpsbkklq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bfkirqrr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2blqehula.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zvidtphc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uyekyrpp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cjoycusb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qlpucpum.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wvantzee.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cgbzqbqk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ophrnfgt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fciazhjn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dajhbhxr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ibzuvkkm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2orhvmvak.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hhfirhqi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vgmsfvso.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2pxoukmvr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uvcavncy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2brzttlni.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qehaskve.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tfwiqcib.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fetjrvcw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kxzyflih.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2recymjhn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sfksukof.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ekbwualj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2oiusetvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njdplkpk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2eponblyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2totgapdl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wrwhlapr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ikaknzon.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mqqmhewx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nefvltys.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqohwkf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nebvkuhv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oojelnoh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hkaxsxbf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axcfebkz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hawgxiff.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rbunaknh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tubivzas.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uyxbrnku.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2szgdzrwi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vyxhqhiw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2opluycfp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tycgihmw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2luywpzyu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tejvdjab.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lqeoulhg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bidlaaei.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aygzotwe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qntrsnzx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qwvlzzwl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hujytevn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fjaoitep.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qwxzcxfg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sfgyjsfc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mydawnem.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xkicebqw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sofzbusg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ulmmwiri.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrhbzgd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvesttiu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fscchzhj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hdovjpsg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2umaerndx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dsxqlcic.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2szalpvfj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljthnozt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yjrufulw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2aycitalw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2buryidbd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2crukhdsf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aqvdavpt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jicmrewa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qvshhqfb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qsgbzbga.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yarshhqt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onnsseoe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jkldogvk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2feypptuv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ikygdorx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bhlkpfem.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kogslrwj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sbwpixhy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hcdypovi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kxdqwihs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pslajxfj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cndqcanf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cydnwdho.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vmoolptn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kwlonezs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yorfkxga.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbxorfh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2huxccsem.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zeiwotmk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqeqiotm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvbgcalp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lkfkgqnd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fyyleawf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eleuvqho.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ruggkoxu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rwqmfjpr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fzpmdxro.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qddvaamy.html


<!-- 参考信息 -->