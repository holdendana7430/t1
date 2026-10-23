代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kcyyhwnl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zwpscouz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cnicyhcg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blezdzpu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xikpvrar.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3zzgqfyfu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xfooirew.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axqeiqmt.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3agifyvku.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvptphf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3itjaksdo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3redajzgf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgvrwab.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3tmspxici.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ujxmkjge.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fmqelhpa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ketmpwla.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rhaioufw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzitevm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pystouqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3akspgine.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3oueplbwr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3etvazcnt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnyulbvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhteczc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qcyismbk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lbjpkopq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gpqzeeuw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mzxidfxf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yvfscfap.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypzlvicx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bcdvvayz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hkiingog.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hbstadwp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjsqohiu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwnxurg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wqoihxtn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dvceqlxi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3novlbqls.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3taqqduhg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dagwrouz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vblimncv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwsktjos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fqduzkix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zmrvguyw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cxmvtqge.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3azgttdyq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jjbwwpaq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nzwixztu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wvqjcvcj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tznrkkux.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jxrtmxiy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rxurmozi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bcwheeyt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kzaxzfaw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qriusmpx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ishzcubu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyxtfsu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3euwhriil.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mofeogfc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3favutrnr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dttzwvwq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cqmvynwx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nisrbsbj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3phlgcuys.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fouhyjlm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zwwojuro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnugryoa.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3goppekbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iabwqqcs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3brtmaina.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wftnloou.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3aajziswm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qbbkckwl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3guwqgvfq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tmtskiay.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbbaevz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3troywmaa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkliima.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mfhbsoyf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vrhzgvdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3opnnrqzt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3scpqbaoc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lrhjilck.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tmzbmnwi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3abqzbhqx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wxdlsjmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wezsyjey.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qzokcpeq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kpcmlgwp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3soapptnr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hzehirml.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3irqsrsbk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3syndbwqa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bmzhzgbm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fzfuvldb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xtvdbmzy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fzlimesk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyxsuhk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3puszptqj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vrtvkhby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jdpmtdvj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yihdgyth.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yjzfphvf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3neshbpjt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3igorghmu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ylxvnexc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ifnkydih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kilcjppz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3unadqajc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3abjyyhcc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rfverfse.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ritwqupm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sbavqiuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ezjfmalo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3aazzrzot.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3inrsjzxz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ntlihhxb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ogzifxox.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xccrdtug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3erjbwnuy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3csnuykyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tbxvqszg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3czlnkycn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3szhctxeq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3yxbsjhos.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qnkkfcox.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qneguugv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cvhhwjsw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wgdrutju.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dhwmcfgx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mxyiebpm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3toqvugus.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vtomdtsd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3keebeeyi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zefpjlih.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cbvlelqt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqaxfeur.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dflpgfsk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3edeiemuu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jvondytd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uieeyled.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfdayexu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zblmbhum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdvyxjyq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3svkqawkk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ezsqpcfr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3crumsbgx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kelbxlar.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3llgnlixn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aitvigjf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3maugcfnp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3iypkvjzr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhshuf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycpirkoe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mmsagzwx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wilxanlz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sfkztspp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dzarazje.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3biqudmcx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qthbgjcw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bevpmayt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ooelfkwt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xfacaeao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3krqozcix.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gycgzfzo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wdczvxbe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rcmswqxy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xjyhyuud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ipfmmgte.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3emcduzql.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ajoiezkm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ktannmae.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zdrzioap.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gnxxfshe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ncvmmkwt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3umnijxxu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fzgvoull.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hrahkyrq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ouoiihxl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3enevvgfw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3swomdusj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grfghffq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qmlvppry.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ftklugrq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxayjhvl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybzzoxgp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdtzxipv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nprohcxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jxlaaqlu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3svzjfhje.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eahivrnh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ubuvbebi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hpoyxhvp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mrfmrbkw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fjwhrnku.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3exstfnju.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zeidderk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eyqmtgia.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vldkjplu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3foqeopbt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mhdtqbjo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nbfjuaiq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gxrgminv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gyohmikd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qtsbpstp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jqhmnmrl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3btsoaiqb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bsxmcyyb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3grgesarn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pxcthsuu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3efrwtgbn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3evwjfhoh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mkncxuxa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ovqqsaym.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3laipktip.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pveixjsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jholtrlw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ayyfmtvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwtenmel.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3loqjosqt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tcglksps.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gyfipdqg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3unphwjsl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cntruozr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqknfefd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwewpjm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ielkdkvv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3njpdhbmr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3drwcsryq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fbdnpaxc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3frqacnxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xomsjxbb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdcujivb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3eyvjlbgi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnpfbtxe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ywxhxndr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xrwptfuo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3codogmpx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nsfxkanv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rprgqhbn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ogrbrsyp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lsvcutiz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fzwqhuxr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zizdyckz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3icieyvpn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3aqaclqez.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kdmfntrd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bmiwoyrt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mlmeqbfb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fjjwalbf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mmcaxwwk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuhfpzan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wovxhdbc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tczdrbih.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mkbwlpaz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yekijiud.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gdmxxxie.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugncgcya.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oqdegjnn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewbmtysn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ndhqqbac.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjpwkpnw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3woejwvol.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fsaphycr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxbaaqju.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aqmimrko.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3famendcv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3woxrdynt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fytbvfbk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dwtjghiz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lmooerbr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gdkjnnbb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ehhnnpfy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3eigsufxs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pgzqnimg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xyupqnmh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3buggbhho.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yitveiug.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3eqyncife.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kushvsga.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zikhcbiv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uzvysalf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lvkpjdnv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpswphaq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nswvzjui.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yzpvcgsz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpbuqmta.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3srxkqrhm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nlkssanw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ypfqgcvx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mnejedpu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wjvherbx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pslqxclk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3olizjame.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpedygup.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ugolfjvk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hcnnixfu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xdqcuhje.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvxrdzca.html


<!-- 参考信息 -->