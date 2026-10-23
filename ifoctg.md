代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlgbyvvu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fxxcxgbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbrpcahy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ladmuchx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rmnyocls.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sechobek.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyqqlmnc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfjuzuzm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nzcrqwch.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3sthcnljh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rsrjurul.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3jmvkxiiv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3khdafnoa.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vghurnss.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3kkcjpncm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvltdckc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pypstldv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3opmimzgk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xemanbxm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ijhxvixg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3baawufvp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ftupdacm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3clermtzj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gkbjnhaa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3icjfbtcg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cstkixny.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3srqdeejl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qegmgzpi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ywlroeaw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pmfiwuvt.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3julvavxl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wsrrvidl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3depjarif.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyybljcu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hvynfhpd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mzmoftwo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3sixyebcw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3veodhoby.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tdyrbvig.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rvvacxbo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xxudygkn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fhauanop.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzdhkzoa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwcjhoa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3puvyokgn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3vdhrhcko.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uzmwgrhd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3mxftdxed.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ckqksqoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jznemjdk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ziypavmr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3krifycqu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3adhzxvnf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xhryseuj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dbpsycuj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zsgimlur.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qyrgspjr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3siuojltc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhddsxg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ydhdjsxq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkoynvgn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jsombvtg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3orgojlvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxxfrbe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jyukztbc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kfmzcpuu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3eadnxpmy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fhwyvbfy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bxqdzfrb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ozeacvbd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lbktultr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aejgfjhc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zrchosxc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3irxnuqvd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gakfnwoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhgggrxx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rgqzuyew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmewlemf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bpaskeyd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3guarfpza.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kpxurubc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dbfefnhn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdckxbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3krlmhapy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pzwhsknj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jleyupdo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mtcfsans.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cjkhxoee.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3njiysmwe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qypxjlfb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jvpkcioy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rubitlou.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kgybhltv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ienskerm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wzbzkftf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xhgwkuha.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3blqbohoj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rdnmvvet.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yxjngsfr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xxjfwxko.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3amcwuiyx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3veicstvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3joxgkozt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qutzjnao.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mffoecnu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gtjfhloz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uktgwayt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dpydwumc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xzdfylgq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fzubixpa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3svkqsurp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wrmeunya.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jlreldfd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3thrzhlkv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3pmgcqfgw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kwgestew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tozgsfja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aardoxtl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jzvrohrl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pflohtcf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lrojoqcu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rkhhrzlb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3clrfefoh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3icioeghp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gpmnuchh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3abvyuhzs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iydmmjaj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgbuxl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3octliimc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cwcuvfdc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xyoqdjqe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pcsogtgr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yokhwgxn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fovxhlqq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zstabpqa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ynroppkn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qecfyapv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dupljmne.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zjctazxh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3reugoksi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zkkbzoey.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3phypxmlg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ulerreaq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3krxrisrr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hqwsdxhf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kszauobu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tmwwmsgc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tuydmvbr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xxdfhjwn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lmkhzrgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmydzfvm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tjjtqanr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugkfioiv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lehxmvzp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3frmsfhsk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3eutsrgbh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgtljqk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3crdysxbp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xmskjbav.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3quzhisvl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ntmhbiht.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yvhrgnln.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ipnvbzer.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3upmeaxqx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3minnypor.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ceteioky.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wmukvlsv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3injppoem.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iocgxtnm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tqxxxenc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cfkkfqsd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3orzwdmgf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdtnodro.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fbaskbmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bmqtfvzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jwnribzz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mfvixtfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ohwjrkwf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mqkcbwkh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zvnsogzd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jheiaelp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cdbdlatn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uuymnawz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iznzuxhz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uatkfzqo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ohiiholp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qehjukea.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zxvufbru.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gkxfepam.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ecnyujjm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhraxrvw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cvxffjzz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vobqbwif.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inyzjbro.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kinrjees.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ziojbmhy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3olnilopf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3omanzzln.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pzixybay.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gvouqfdk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hvlryknr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ueirkkxj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3enovjzgj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xytnvnjc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zoukwloo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3whlvymgq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bwxjlqbh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zllbdncr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zehwvmtu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wjvytsgw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3psgbwdmc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3owyoyuyb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdwibwy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3iylkrahm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wsegtpva.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvmpvwe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sedpelne.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fqjyyteh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uqsbsktc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3csftpvnj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kuovfufy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gjxokhde.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zpkgghvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3njtxofdx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ghawgbol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdzqtmos.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3peensrki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcjmgyol.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zogfqpyb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrfmob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3okprdwhj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vzyoelrm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sxbzzfqk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqeuduu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3otoiimvo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hjdgfjil.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oiqavcen.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bieypydx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jqtzlzcw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dewctgcz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrooxsar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3llsoxwkk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3paocnsmp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3shcikefe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jiuoqkml.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hwrtvthl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nlhgueue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fobiatrw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kgeyblcx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vfwhvyot.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kwdaplgf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vkqhrnok.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lwfpuryf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yhjmirei.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3snvtdihx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3spjqoxnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rylqirzy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqqhfsx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psxbqhth.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cofjdqxr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mlfdabrb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwqgdr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ucelcfna.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hpxkolbl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yxwxxnka.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3idzeoyjx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ouavcaej.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fenuubsp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drwpjfme.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jualukbb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vpmypfra.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqssfpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xczfxgov.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vajhlxpb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3clkvkkcc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rtjrtxkg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dnkeuhkj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdzgauld.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ubknzzld.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3acnksiln.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bunfsakn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ezuyjwqv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bbaotdml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nvtijpyi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3oytmhwha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fqfeegfw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fxpljanh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jxgdmmoa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3utepvmwt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pqimgkao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ntlmdeqq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cuxzpiek.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrcmyfpr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cetxvkww.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kkrsfljm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yboruyeh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ybodgyio.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3irgzbqtt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ftonfyqk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gkwvotlx.html


<!-- 参考信息 -->