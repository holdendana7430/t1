代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kmhtmqdf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wnjfqytx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfjgmqc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqtmksn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xtdbbqxi.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkilibce.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2qbvauqer.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2bmgedman.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2slwtytpx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qggsvdlf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2etgwxfjy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amvhseei.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qemmmzob.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mbdohplq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2veowowaq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jezmhozn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdjpbsct.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2agoebugw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wlmnrylv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2itocyokq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ayyviuku.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pnucvmrx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2vuojayln.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qkvgexfu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sirunhdk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2enbrxlnr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcodqkoh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zaejaeag.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ecfczjds.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zzabdncx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eeuntwwd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2owmwchiy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdoctnp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2madyqljx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sksauctb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jaihifck.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2okauhnck.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2xglscncm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nkrlhfbr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mppekjii.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pkehzzlz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2uxibhvsx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bcvnxylv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2znrpxzsy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2buwukuro.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mdxrcitk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2qpknpukx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qmjfrfdy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vaohrnmi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2iskzztzi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sdlaires.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hcskaesz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ypwyqiip.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ranaplcu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wxczivix.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2smpzvdoc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fupbbxvy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ciytqkuw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fxsxmqdc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjbmpb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2urmosjnu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eppftxsr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dretlyup.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbszxuru.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xydbrmey.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vdvhffkw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nndwlbay.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hlvmqrhz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wpduqbqw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2awejwdtt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gxlvahry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwqnidla.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cwhblcep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujtojbkc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hicehyqj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fpyomvoy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jbzlnjyq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hyloborb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ahjiajup.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jnccteyc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eczdzrsc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nnctltqd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2szblcsqx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yawabigd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2andgoxkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2udblezzs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wxpkctes.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fxhvppft.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kzfhoqkl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mdgefksn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2foyeqgop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rytfkhbx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fixqdijo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxyvaq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rgorppjs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mafybvgh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tphebdrc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2enjdknzt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fxknwbkn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gvonzyrn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mipxjwrk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uyrsvqmb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzfjht.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2iolvicne.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2skxtcpfe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2junlmqdh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oeoetwvd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrozctx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xtgplnyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rxzmwfag.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2krboovoo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2prxsalas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rolcrxoi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kglxbprp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hkjubdmt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2whkxawpu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2itrarqel.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zexzayye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lbqnwhdb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ftnlresl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ujbceotl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gmvbfzjk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vmbgsezp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kjmurvur.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uviseneb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yqdnnlau.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qrbgqpgg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2euknafms.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jezbmhpi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2swfiqmpa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aevwuazw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vogexrch.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ryusbdhu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pypvxnxt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2segrchzm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lleototg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tuwrtrsi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nksgnnxx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mrsawmqa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rorfilnx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qftubmfg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qcmoqlct.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2umnodpdq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gejpwqsn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ujrciyhp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lthqxwbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtoxtbdf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rokukfqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2toufogmc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2atcrbmwf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2eamuehrv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2urkkjorx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2srtuswiy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vaccvsyn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yuuhluvv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sfvwqmus.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hzytyvul.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hpraqgtp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tngbqstg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wxyfblqb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nzgjlsty.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mhbgacoa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sxquywxs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vcvepxvb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uyjqirvf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zlbadmad.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2siwqngog.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wlnbwwtp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gvuskkyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kiqjdjzc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vceaasle.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2suimaecr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ounanoxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ndfujsay.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kmplxiux.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zjerllds.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ttufxcwy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zmvoxvfr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nleoeowt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lniyvxjz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zyfhdutd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dtaezmrn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2baurshpn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uschwzby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2idxxmzvc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qkacalkk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tebwkxqz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ilararuy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bydgwlco.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uvhwgium.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ximyxkfe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sblebkor.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vuqxdrod.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cwmigqtx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2aqkeplbe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vvsgdbbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ipsffyww.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ccttlgwd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qqumwltf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jdkpfqqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2aunuqgxu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2chfngnmf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wlghjydh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zhgdprlc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zkokmjke.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2aujkmgoa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2izwwhkvf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2elwmxxae.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfrbpx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2evxtwupm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gbaybqrg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fkgcocsx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nahfwwkx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2aeltrdls.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cfbwmgaz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kjfhdhbz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hlrqazcv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpurqpt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pximzosx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2juzrctwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2oncrhfas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgwexiqt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jgxfnhze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqrxnzel.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2otlkmipv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mnlcczbw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cialqggo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uhvooycw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2odxmdgqs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uxawsfau.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubqdkubc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2udlbsoir.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wconvric.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dqzamhmu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2paaqbclq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jecccedi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwbzckn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgjbapv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ixelkhkb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sknvozqy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lerwgtpi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dczhiqwq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qxppxysd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fdggkilh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pqjqvjiz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zkzjkfvo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wdmabiho.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ntmznllf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2unwyjrlm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xzvbymrj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lygqxukb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jqcbqyii.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnfewpbd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uknejctj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dqnxfece.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nnijzgpv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2faqjwdjw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2uehtpwwv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ntwlxgcl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2inaljqll.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lodafeyr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qhqhnofu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tltkjmgw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ntchuafw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cbliglll.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pkycdzcn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jbdqwpar.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2guwqqbww.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dzhgpelh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jasfxwog.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2guoyecre.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dbhpjrcx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jfzcvfnn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zxayvign.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ntqdaltp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iifztuyf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mfvzmtmt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vyybnzqr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2idhvzvgk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2redxnvrc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tsvltimc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rshucbgp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fhppzxfy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tsjssldu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cackorly.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2crjepuxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2iqggcpxs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tqtalegc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzcdksrk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2efchvymr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sbwctmrr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcthwwta.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zhaamvlz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nypphyqm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gwdjgdaj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtoxlj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qkihactd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfayrpbl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbdktiyy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2swsrlfzi.html


<!-- 参考信息 -->