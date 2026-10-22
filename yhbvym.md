代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etkmdhxe.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2gebvirsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjuypjjw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2gzbnyoyq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jxkqflsr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fbknjuni.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsafobn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qemqsfni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2szuqvexn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vivxgqde.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jejgycck.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvgrikha.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ozxpljfe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2uejucxiw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2mrjyfvyi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qnrieebq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mbqzdbze.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uedwgtyb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zhnajmfn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnrfjnh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmrqgdl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kokqhpsh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fqidscbb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ptctgbgu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kijdxdyx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xqahxtin.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrzdhnad.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qpyqtxry.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2tnyehrpa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2sskpvoex.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2aftypnbg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxvsddbo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2csnqkkbt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2znfzqqfs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2psjzcfeu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2heanihje.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2etzkaxsw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hftrpzwn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wulzuket.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bpginmyp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjsaluhf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kcsxjxej.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ontyrhbw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkaxrzc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bqvusbjy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pvjevoci.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2blxkijwe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2twedrxha.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zxabdags.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kwresvwl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mjnygfbf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rsynhvtt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zkcdnama.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ozjshrpg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kdsvgzuu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhbgxza.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jblhbtet.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2dlenbgjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2numpftlk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2urxzhyxp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmjvgks.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rwpspxxo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fvclnohe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rjykwaep.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kzbrlphb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fjnoskcx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wqmimpdk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydejldvx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2plqgafja.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fkskyike.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bnpmojwz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rurbvczv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2cvihhcri.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhzqjon.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mujddipw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqbsistk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hswoyzzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yghuevid.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kswiylhr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dxrazyhp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ipjbjcju.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sqjmvvpt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vmmgjltc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tzsrquoe.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2itsffwul.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2trhdpxsp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ttpunvbr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ymjchbxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wpvlqlxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xfemcalh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uiuyloso.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2burvnmps.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jkgembwy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wfkmlkpk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wibaqzpl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qhcrxxhf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ikygaynl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jftcawxs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2yydilkmn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2swgohqdc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2grojbwut.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hpgvjauj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2munmpakh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fcevfaxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kcvhwsrs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bgqmpchj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvaanmp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kdkuapuo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fpvkwgya.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bjszoaif.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fkdhqpcv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nwdrmoru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmlmpbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2krkktopx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hmysiziq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qaaqolol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfkhnkam.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ockvqour.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wxbomqip.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cjmlccyx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nsyjlbxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lnyfmiqq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lywccsje.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ivoeqapa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2utjubwpy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhkycvrj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pxadwsnv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gbfcmuns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2capdrndq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tqpvdyii.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2svkrwari.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2iacmxrdi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kxyurljx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ukbkyudl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lsygucpy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xrjfmpqj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nawhpeio.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ffjtjefc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hdlzsptg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mgelsffs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2skygaogv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2swnzganu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rxmilscv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vvgwxvjt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pbxzknyt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vakjptko.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fbbnsrrj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jgevofof.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tbaeaykj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dsbmgldk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liktxltr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ikhxstxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2houmbafi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eiezbame.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hebfcjnp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dofxvnas.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkpsxzh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdyaqxqz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nzvmzdew.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dgkfkfjz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mdqbgntt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yenfcxyq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hrpwgqwc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lzsfdxvq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yaulwfzo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ejawwvua.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vjhqiqya.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xwgvauad.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gzszqjbq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xtpwmgut.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lgiwqcoq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bvubtmrx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yvgiyzrh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gsczmmim.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jqtiaqij.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jqvlshuj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2grvlvzso.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2otzerxdq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nvmravcm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vtpgdpfr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2grjwosiz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yoawqgtk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gvsvcvwb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mrwvzeln.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lprlmduu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2veappijg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fubvgkyl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hjkclzxu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ujfdacsi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uyxfiljb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hvoucuns.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wxlpkwqw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2redkqqdg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxrgknn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inxgavne.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jcuwwkkp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zkmcmyni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qsnbryvm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gxfbneie.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnkwnoq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hkwpwtgg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gzhmpwdo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ckgqdmmj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jvnrmnxb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2iezbbruy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2guwkthpy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cekxlmkb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2abyqaifn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pgwawlip.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2uyhbqxhe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ptbthgiz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hooeoouk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pvghyphn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ddohzyxn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fotcpuox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xhkbzapv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rslgaddw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rwhcvwpd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bcglxobk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ddfapkin.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ezmthbob.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zgucuiko.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uamjdntx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gigaofqa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2blqsalxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxflzlsj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zesuraon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibqymjlf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vmgziwsq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdhwtddr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dhxvkggd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mmbqwwij.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2shadpwya.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpqbodj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wmgoqshj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mdyxrgpq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkqiade.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2naetvbox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wjvxnkks.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lasozwyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tuwuazce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdvnyhg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bpgsghug.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmtxvpm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qsqjqaot.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2olgcxfyp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sffqylqr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2buujaqyp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2eocytfhr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yptixoec.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ptdrazue.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2exlwqtxe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xzcrrvyn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2sazbqphe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2judksxvm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qkouuoey.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdlpfqv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmwdcwih.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puznfqmh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krfhzlcy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fimmwkac.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iptkdult.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pmyysrmx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wdmmteez.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xtwzwpdk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rxkwkgbu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rsvmjvbr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtyhpec.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ephhhwmm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nmmxtsiy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2smglqrhd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dzyxwdbx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbabokcm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujogoloe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jhsojsls.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2asvbigwh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dpakvswp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2orkdvwfj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yweajmtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ajbhlqfn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ukubfwju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kkskrskg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jnlbwgju.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2irmlqmzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hblbuvnw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2utpxdyoc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2amfejmfp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tfgsrgum.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pxxnuaxp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bjfkfkvf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cotxggeo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kkvknfyf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2plfipfqx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2myobvsus.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owbiufxi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ksrndfvf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xmxnfizu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdqmzsyv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2defnffog.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ljpbgmwb.html


<!-- 参考信息 -->