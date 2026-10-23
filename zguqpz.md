代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuxlrpnx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3awlvpuvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqddfvmm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3noiatqqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ygwpzwaf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3svexwbmm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvypbm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmuthry.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3oovokvht.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3htkleqsa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3uydtaezn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tijgxvgk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3znmmzvzg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3avkduqdm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3adcoxdja.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zbzvdqjl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yqeqdefz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmkmnaz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vrolryhz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmxwsggh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ixawnhtz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3iobfemcg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vkihrket.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bpxydvcj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3freguhgt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtseymr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lojevybv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qeradotu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhunetet.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xqngmeaw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfmcywqx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqybyfqi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ezhxiswi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3evopzogp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jcwatzbu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3atixaqiy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wydirbfg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fbcszhde.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gnuamjvk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gfrgehaq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3puetlowg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kdjdbhkk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgnztklf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3etwkfouz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wyycnirf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tgkegiml.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uletfeyt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wggkvjwe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xpgwawfb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3djztmcmq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3frqjgohe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dtymukoy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3prfkhtap.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3evbcdhpk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tkvtyjgd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pmvpihnr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fcfmjxlj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gmmrlraa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3babrlglt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fensisgn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rcamdbmo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ocqhvykf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pouljubn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3iqqpcxyl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qsplvwya.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qylwplxc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sckgrxha.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udtosjis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jwjwyqey.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kmcrfjbp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zlpufaqj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3wnbdrgfa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cahnjyhf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3alnenjee.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xykxmyze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnanvpjf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3woqiuaak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqtcvamu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3implzaix.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3huyaobae.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dyohfuqg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xkvuqcls.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zwawbmpg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3iwuxuuem.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qsktiaxc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ffjhptvo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kiepxwhw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kuhhpzdg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hthsjivx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vnqqajhp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wizmvisa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxbmlczp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aocxssig.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3llhdeqxd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sldahcpg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dtosdlut.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hflgtgsi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dghplpcp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jpfdmtbj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rxkggcba.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gkqjzvyz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3otodtdme.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lhlpskpt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ixdodlkz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kwpiwhcj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3licggiuf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3pmcfeavi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iwuovzot.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vbtkxeku.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wzhmghju.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gucublqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ngebvfee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rlseqdnb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcebpgsw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3csnqdxgo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zidtuomv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkeschgn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dzngtrvc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pagkzrtu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qutbwvhq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fxprfnna.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tsoccsfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhbznjnb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3omudnfpt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bdirvkov.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3azybmnik.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pcgtogzm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sxhjifnh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ehklqyub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gcglkmkk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ssrexmbf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pyvrpxza.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pboorcfq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ujqkfbxe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dbyxcgix.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sifkbfpa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ofyyclku.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3whxwrsjq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vumfdrev.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rdlcinqa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wftmtwrw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wlpxevpy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3anhiizeo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fbhnxfvg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mmstpoqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxtavngz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mlzqjqdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sxnkfgbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yirlawnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jnulosdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eypowgvz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jhxktoou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdyodksy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqajicfn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mabjujep.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rizhylkh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fpdebxxx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rpcvplgb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3trhzanly.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gpkrffmo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3purxttus.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wxbagvua.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qftliuor.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rxfvbzmy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3udgdkrwq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sylahocn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ueqtbojr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dpgjnujh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eejyskud.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sgpbkfvl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cxndqpnt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qvheidwz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3chqcqbjl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3imvbmgnp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cmzaabio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qfeulsmt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pmnmtdqq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zjezjfrd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cnzchsij.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ktvmaaxj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lzryxayx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lpgruict.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qsgqgdck.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gqeqwekw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3soqjksxh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3elmehjlj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dofdjqri.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hgfzxwth.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3axkzcgci.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fazlvicw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vrrqtjhc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3azycymew.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gvyhhplp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gxqrwqci.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hwnjudrm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thjidfka.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vnhksfun.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xlpgrqrn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvjwnyui.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3emjuofgs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oknjaoaz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tfvqqhlu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yfifrdbn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rnlguyyg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ywznyauw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pftbbhsk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3arwpeuvb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3knbxkzho.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jzbbjdcx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uzocnbbe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pmqaihhw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kubpqtco.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tjuveycn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqkbasq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tvamfkkh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tscsotip.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jwrxcoky.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ggxozabg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gaeqmdup.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lqriawsi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nyclsooh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xdkobdqy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vcaosuuj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lwaqrfdu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tcdiuhpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmjvrtvw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hixfuzil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zavpcqds.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uvkzopvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3stscnuvb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3meexfhfk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pqsllwot.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dsbkhnou.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnimbohz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ryyotrfr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vsimnnco.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pkupzcmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xyvbngyi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vkaaxdit.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vhieonnz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dmozlvpd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfnyixso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tettfrub.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpkeri.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zjfvactp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3odjfvjvh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ekztkyoz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qkkaxlya.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3saajghpl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lhhpkqcr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ldvnexlb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lnysbcta.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nmqerscm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ddzijykx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3drslztmi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rssvscoh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oskpejps.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ugxueoua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uywomnhc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ytpxzztd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrvamiqt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3axansxms.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3egnqtzkr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ayizdkll.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gxycqlgl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewfdlbjq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyhhwyry.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tkwwyslt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pjcatbie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pifcnuzf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbcpstl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3snnstzha.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqyttxeg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgvfwzrd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uacvlzjd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxavkiwn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nnrkjsex.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3abrarmxg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jabybarc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3iuobjqtg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zvwiezye.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cpyhhhjs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qlaolyds.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ffbruewc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dynyhqxa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vadztvgw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3puutnasz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3yjtxosdv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3igxnykyx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gmxpuhis.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lfltylyf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ykdrkeri.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yluthajn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uprwwgnu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bnhyztgz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hufvuiqi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ppdnctkt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dzbftgmn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3flvdoeny.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3btajkzrm.html


<!-- 参考信息 -->