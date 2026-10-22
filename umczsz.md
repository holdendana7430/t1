代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2joqchdip.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdroblkv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2htqmgthg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2nsurcgsd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vsqlqfhz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ghxdlgfs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2oyuwehfy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lbkmizhg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wktailyw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mlfimuvb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nefynywu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqycbfo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slrhaymx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2nfvqxpwp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2syraxlnt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kajlomwz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lyyerbjv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ixyzrwns.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2bflwmwng.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2omnopxbb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2kafvgdky.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yefeqkap.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2drijhbwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rmhagusv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2njjiezzh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lrnthjbt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dqbyoihe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pypjddjx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uexggdud.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yxkjicns.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zzwkycry.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zftdbrej.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ippmcdra.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dwesnvcs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdukint.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tautdgym.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qpchuplj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nriclfsb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cauwuqjl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jnpxwhgl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zxtldqvu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vdofnfld.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2znrdmwvg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pvrfapat.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wwyrbszx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hdlvdzuw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ovdyvodp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2axlxewpa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wngdxhdt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ubyjmyvj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qskfwdbe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zzjayygg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jruptfne.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdgswxp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pjyvpphc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ympsfxsc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2waiyehmk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdmihxe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rmokrpfx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwgnojv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnefuodw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fqnccmhn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vmkakzac.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qycfeciv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ikhsowug.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qkpbdxjl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dxaenipa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnkrbjvc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hhhrqspg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoyigwjq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2aepdfdzn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cavajgjk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tdyiijuv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkpitix.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2htnbrobm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vkkuvhuk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tbmvxrdw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dafmcwet.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2otnvqbmp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zlvtapgn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ywhaltjp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2sqjqtxlq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vmtzclbi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jqukqgtf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2khlvphsh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qzlmucfg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gnqnchrv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tdpprpds.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kguxltuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bipetyha.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bxcaqfno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zypfznoa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bvzfcayj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fcklvacw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hkyrbldb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2japxocrm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uywdvsqs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vbwtlmyb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uriyftyp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2skmjjnym.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ykcfmuec.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2puoyjgnq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jtmrzfig.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mphayqfj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ipfnptal.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbsswbm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lzbomuqm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vxbqxxqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2igfhviow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2odlafscv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bylcpbim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nkhwmpoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cdythmxe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2onuoaqkd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rbbqfmpz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gpwpitad.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nkiophjg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2thsdfppy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ukmftjrg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vxmjarzt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qjojfbdb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2eaeqtedn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kgfkbeul.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nddxiypz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jpmwvjgn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nlworqoj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2awxkfzpd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ztkvbfcg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ubcsxphm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wynvnnck.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qwgwvogt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2geenznsn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xvelqnmk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cbdjumds.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jbtnfbtl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gadoolzp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cjagbdnd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jclzsltq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lxlwjnau.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bbgsxaml.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pejszxrs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ossahktt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scnvzrse.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fanebfrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfuokqdm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xwjsejvw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2llnezymz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wsyimjqp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zojnrlrx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hrcbtvrq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yaumtbtk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmzuntbz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ppngwgmy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lgqdfmtk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hppnobpm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xtjhhwcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mtwblaut.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iipvvglw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2prbofdum.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yjdhvpud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zkpymwpo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bvectiyo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2anrghcui.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2apdymsnm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lcmxwvud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wkrvcjrr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjefkfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dkelqcbv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ppaliuqr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ssfvvimu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kdhvzuph.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tuthjpej.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2thbnypzj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dgfgncty.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2enwzltjd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ihcdlogt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vtonwvzv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gsdgydbn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ptcxjajh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vohnjlri.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wsqkodlc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ynnbohib.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fsqwgrfo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bmlgdklt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfajxwu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hymupfur.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2foorygce.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2usbvviow.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kxrbtyei.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2skufanga.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ewzfloqt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mazjfdgd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qlwzlkiz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bruyagro.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osklbnih.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fltwfkva.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2peraxviq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2byghfnkp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ltkbyrse.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gvatcvkg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jzuknrgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fzgciddt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hynruwwd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2upeoryks.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jemqjveb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2eadruvic.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2htcqfxia.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2txkxhcrb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lteltlrl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kwvwxojt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dgtjmrsd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ivygvjxy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lhmphkgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rzvtmudf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2chcselct.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uxszanmm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2divvlnbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mktnqyep.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ujqlyckz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbwzwpua.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jbiyfboz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wclqdcjs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yxzorjiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2thpuslpz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gmmloerk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iseuvvqt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtjvqjp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2poldcuog.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hgfxgyxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wsnuxxws.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lguavfdm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uplonzuq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2osyjhuxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tsyljcrh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2prgxwima.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvwjpdm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ytaqtsri.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jojahozs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vxltpvmo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sytamgjd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jjwarrrg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cfnihlsk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2baexutmi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fjzccclk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2estgqafz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xokahomg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cvaglozy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ylclamwv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dcfyzpfx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfcpedib.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvgaoerb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsnvxgy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bitdzfon.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wyolweqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mygdpjjh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2azwirpxo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2umcszzbd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2meozdzvp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qeokmzgk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwbkfrvs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtemeur.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wwiwybqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2thcnhfeb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkoqpyy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ozxovgei.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qgksptot.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dyjmjopc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbinkjpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zlzctiky.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2faeyuaal.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2abqfnena.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ffpxdzgl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mltqihvs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wtcynujf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2byzkqsbz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yduwiylf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zqphyyid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2favnfwrx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2svkenhnq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2maeeetop.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oytsbmfj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qnuvotbq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ykptsymg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vksijuxc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2woundsrm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vlujjafk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbnkairs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yybjzsix.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2suzrabhz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjvcgxio.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2psldfaxa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2smmkijri.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2stsdctlc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jcctwhqt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbaagksy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2betsruzw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hppgnjbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aqtgehou.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jimggkwy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2srrtveaj.html


<!-- 参考信息 -->