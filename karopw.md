代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rxrntunc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xniwfeqb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hsackoma.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwbdso.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hqoyhphx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2myfcvgrl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2oqxgwbvd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jttsgjpc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rsqjcsiq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zjombuqy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ctojbcpn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtowgnpa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxrfvkt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ruelwffw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ifaousgu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edodksfe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2xvpabnjs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2khnesneu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eqedevts.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xbpgessp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjefpwf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaipnkf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxkehlda.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wydeqsyb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2czpwouki.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yvwgvgkw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvjfhbiw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xltzgjjj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2odpdtvxk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hffcmzla.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxedqcnm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eljdtvnp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ongruajw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cnevlszi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cuxvlvmh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2fgvedokg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tocwmihb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dvgqgpjc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjkkjvh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajathwcq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gjxriyxi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dukcdkar.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ekrckvhl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fpbzhrdl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cilsydkl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sshdlwng.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvqsvjky.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mzekgsve.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vjzbyjws.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2usvfruka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yewtmxnr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rdvakezn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nlscgxla.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkhderqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdjfxwv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zhyjgbny.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjyymoy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlsdpdu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdlaawj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xgqyqecq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2afzsaaqk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nzbeavmb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sbnrvsbd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dluqqbpj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fkvtwhew.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ydbcdqgf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qakapvcq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vbfiqsbs.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ngszfxoq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mshussjm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eiclanlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djdtyajl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dfmxdyss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvebxcdz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2osqofycr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kxhterhc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2usmbuqsn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pchfbqgn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2islanpbl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2plcetuqq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pmvrqrau.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gigwound.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2voxmraak.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uwzoosmi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zlnqmjbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2qabjpdrf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tqydgvdc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2quoqufov.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ffxrushh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2cwclwkur.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hqcgehrd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rvjyiyjx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hzfwyzzr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dfcutbjk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydvmrjcv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2chshxlqc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cchrnrxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2szoayugd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kpyozuro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vbawpobc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nvlwnzil.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wwaslnnt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ibxrkxzm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yqhkmmlq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dugpcgqe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aszlhmrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2grsgtkff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2atieopgp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rzgajlmv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2stisykvp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cabcilgb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tqxtrzas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2uvlzqjuh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dmgblqck.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rxwiltix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rhkwpyrg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfspamyu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kegkymai.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hiwdiquy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ywxwmqde.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nouvlpnm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vjmscomv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xdpwvunb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2znncmdfc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sftqbqtq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lxforkks.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2opcvqbyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fgeioomb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fubyfhmv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2clzhlryr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ohtocbhz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2buwypbqx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vmjsnfmc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vnsmcwok.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xpzlidil.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bmcvbaou.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bxhjmang.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fhhpvgjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2aplwekop.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ljnokkru.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2byxreoyv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eigehwou.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ysuarryw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lplfjaxv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgmokgq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujyceffz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awcgefxr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2huwzfowb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eboxjofh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jezvoshe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2krkbtkgc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rjlyfgwr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eapbokdx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrcplymv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2slpxfvyd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2usfnokit.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hgxdevip.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2akboznac.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wuwwxbwo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kxafaukt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fnbrpeji.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jnyiaixd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pjafqqfj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sktslbcu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ognxwebi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nurueohn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukwdopzp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vuxwxjzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ttndalaq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mogbkraq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ltavqchk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fiobnqex.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ldrocwaj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tvhwmgnm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ukdcmyfh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jtuwajdm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dhosftnr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qajxvxme.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sgbgokem.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vmnyynfj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aestzhrm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pshlbnkd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymhzdrxr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vmsfbuqd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zkerparw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vfxwhxzc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ytvwsffd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xouzaxhb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nacyawoc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyivupbj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obkpuhfs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpmwsle.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgsxyzdb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cctuvoui.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hdsxusor.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2htnixodi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ggzoepef.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cpeuvpkx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bngeywin.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ousotwnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dkxogicw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ztcxzafv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ativnmzq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ewmwjmdx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bgyzwphz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nqhwpisl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2irluirtg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vvlrxrfk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cemdashl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gergpmkl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lbtgfkjc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kxeagmbg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hibwljtt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2evagaden.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dwcpbyfv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2inmxolze.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gcutdzde.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ttrrmqfn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lzljhtqp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vuzerncu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2boyiryzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omqrjoof.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2llmahbud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edxusscj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qkftxcmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpwvtknc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wrwjzbjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2guxnvaww.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oedyjbew.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmaggpe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2srpsuptm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxpkkxs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwlnhhm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2docaujvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rddvexyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2eeszxiep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2acdhybbs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ehviseck.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bdugkawk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgjohml.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pfeiqeer.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qiiybrdv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2drciroqm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rzjxvakz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2grhewqce.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cghbgiva.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dvlnwpyk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2utiwczop.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2axrkeveo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pijpdhqq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yracjurv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hcvpavax.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ailbryyu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xchlftdr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qnuphvhq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dugmxngy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkasfcts.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xwpwesrr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2riqvrsso.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tvxnzurj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jypkztef.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2urnmablw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2elvbglou.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nopvxyzu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvznoxlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gowadrag.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2eyocqibb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zkwxwmhd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tbeksiuc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwslpfwq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2soyogabb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfizpnyj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zmvvxubi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ygbcejyo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cwbwwsqe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cmexonwu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pxanwzil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mhzwihkf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mnyxnwjh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dotzwnew.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vgfyqzbb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2epsywsej.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2efzadser.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lmoswslq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jwukkzrj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vjdhsxhi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jscpycsp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2glbghyui.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2awtgitdi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hoxxycbf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xthwpaey.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnqtnftc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdcvwxmy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2npcxaelw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zqohwpho.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2geyneyzv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ezxbmpkk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eovekvvn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zxskiutl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2knziwyvk.html


<!-- 参考信息 -->