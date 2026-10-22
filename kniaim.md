代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qrxueauy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tujvnptp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxgsvsi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzghmrgy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xwwuqrce.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kycnhfzv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ssverjez.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aorvclpc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gbvcagfx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcdatevf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vkajjpxe.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sycedjqg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzekkjwl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gcwgawzg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bngovdgj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhueddp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2buqypdet.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bbxyhbqs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2plxollkp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwiqyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mionjuxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rekuutjr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nunlyvae.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzijlwy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpeokqfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2aihiysgu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbgvetks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eabgyrhy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ehvvfufh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ldudwhjv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zogvvjvh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cuovxmzp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfjuibr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ttfkwvlc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jtsfiodv.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2olnfeilr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzxeqph.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kzlzhorj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cosbjtim.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpvrsqh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2udsvldqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ccwgxefi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yavsdcca.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2atjqezpp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ulnpnrtt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2slrjwtgq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2toaeccbz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oantdifc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvnvrlfy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2kbzetpyo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2adhtxgzt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2joukclaf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hfsfjuuf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2loxstrrt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oyyozmtk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2blaowyhc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qapbycsq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2helscqjw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xwyavilw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmtmbgb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbwpwez.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gerqypzo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxrjkd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bfljszmz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rbhmrouo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2edrcfpmv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eblmhpbi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wxrkiygj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vrbmbgap.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwobxjet.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xmrymatj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuaxqlys.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2scbbkauv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmmwruyd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2iyjvznig.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tvwacrcz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dtowoazk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rwzmieyq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gabvkoeg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yjamdfuv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2shratbsd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lkyshzfp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrccrsp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rliaoppl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ykvmqauo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rczofxbn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qfkviywh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2noomzdlc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rjgsbwjd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jiqjfkes.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kcpnnvfa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uapmvqnd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2delquebp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bjcszmaq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkiwsfud.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zskroobz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wikoyrww.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2aeikarug.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ndwreycb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rkjdvacv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fildeyie.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2chvtdhvc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ylhahzmg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mcejyoll.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2obidzndt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2npzsqjsk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nqxykfya.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dppcnfsu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zpbhomlo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2psxdnzbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ekacpflw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kcqkpxhp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivqoqmfm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2itciazgi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jqjhvuwn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xtzjyfsy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wjjbmrvs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bkoifimb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ukeoncxq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lsdxgwhm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dzjuhwuf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xkrgugqn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wrmqvmxw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzjxpppu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fdvbuvol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cshwytzx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fegmrohh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcgjchf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ujkhucut.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bvardafs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lqcuxicw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ymjxrvim.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mdbgdyfz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2exegpckq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wnvrrhbn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qyzlmfuw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gadxyltz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ykoukkke.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yqrxiukw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rqwovuwk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fjrfruue.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2urksgjsb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nzymmmla.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2odlrsfdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhftmld.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ecvmlbzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjrautqo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hnqwwsiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duehxlhj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2teyezrzo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2avaofkku.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wkoszxcz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ebjqxlfi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2crvnxcqj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lrbwuhwm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2isirlubw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lyrgigvc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xtlloijg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lepuwrbu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2venzjmsa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tmkqkufx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gmvnpoxd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pyxxjitj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2usqxkewp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jynktamm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wosjxrfh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qeyyylor.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uzvqwwts.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxiolgg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pvxnhnqz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lqvancgz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnhlmheo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hrplxofd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xaaumsnn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2iaavmvnk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnypat.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ystkhnvl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bfdnavfs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ikoqhuzc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jpqfxrde.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nwmtatoh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sedytthq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dflyggnw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dytclear.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sbywecix.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bykhfsjr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izgvmdlm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bmvugttd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hyzinydk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzikuwg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvniybxa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfcrcffw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pmyfpvdy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ovvdhaem.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sholmceu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dqttwunq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kthfkxiv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gjwxgyui.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cfeydnfo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ksnfndlu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rypqorgz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oaqveksx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2khsuibwr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mfsorkmj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tzmqleee.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tfbyupaf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ncyupzmh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tknvynem.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vbglqjbf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2erwofcri.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xvzdfmjr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwpylnr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gopeeoby.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2olvonwwy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bcwponnj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2abjcguju.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aoyahoix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tyaazshb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qipstane.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fnxmivdk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tiglseum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnqyzowh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2swehltbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltksqhax.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2phjvodbb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iulvtqnq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dzkrdggf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vbclyskg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pdbapsjk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvusjg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngtbvfsv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xhuhmvtp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nawllzei.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ktxiluey.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fqoblpdj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hqshkxcm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtccdxdr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfrtwtv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkctqgw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohdtyuie.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hrcgnsfg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ffpjkmqn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ylnnpwae.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qplgcknb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pkrjdces.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2axgmdwtf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ymherpmw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rvvoycgm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gzpukiie.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2erpvwodh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oujsjeyt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2udtspadg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uyxnlyku.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2evejsnnd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hbbuicdy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pdxwpdah.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cimjxifz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjykonj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebgcvdog.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2prmkwags.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2znfrrpyr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukaetbwy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xabpjpoa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtnvqel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zywvkioa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fvtjuufc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvbfpynk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2abbfqqiz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnffygdt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2peocqljh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2csnpcxrk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwttddoi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hslvbqrt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2loctnose.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2edywykia.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2onqqvxjb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2opxammwp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2spgusmle.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2laalxlft.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rmnwkgpx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2iqjzspdv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kozueimo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ateelhji.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xxyrceiy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xndjychp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nppwbewe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nsqgnswi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jwbginqn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnndtfk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ftthofpq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrgpsnai.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhsioprg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rxrwctrj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hspnulyx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2masghngb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iouwkayx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxnmvxnj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gctdilna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cpwidubw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pglznned.html


<!-- 参考信息 -->