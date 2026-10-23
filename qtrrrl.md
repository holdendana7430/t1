代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fqnmnlxc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzvpinwp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kugbqgkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3rlabzhtv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ppachbsr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gfhmseuk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xdqjmrih.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dkddoznw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdzumgs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bmcfdgyo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ardoqcig.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jxuaitcx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bldbbsyj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3osclbnta.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wxjpxpuo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzncgdr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awdyofss.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mnmbseus.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbnyerb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fswysbgn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ppjylfhq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fynxzjvh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yzdzzqio.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3oigewcmt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jalkmcdw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3krhlobyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wuahpuiw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcrfcci.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3attciigk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yowaxexj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpkryjvr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qxxxszgb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbksqmr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ozwlppox.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdqcfnok.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ybiblkpq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bvhezzpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iveygwgt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hltlopro.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3oyjgklwk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zypxqbdf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3csfmhggk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hubgyaks.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yuldsgay.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xhsosiey.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bqghgmec.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hwgvoklc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fhtbhmlj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3srnhhbma.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xdyqgqzx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xbmgppcf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vkiubpsu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyelhkxo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ufsevipw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wdoeiyec.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vjffvzon.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pyfanskv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kpplsekv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ewhsqppp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3beiajthi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3otiqjumf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cjrwmdcv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wtclxleb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3bqcvbwsp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hgfeeqij.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbhuhot.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gtmdwtda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydidiupb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zphnttkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clxdapoo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3emmcrddv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uxajgwms.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3czgmcweb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tneimvzn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqfdrup.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rpbbfjmz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jbcjmlie.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtxicr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3effuaawy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3afgbncod.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rgkzcsbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lpwlefny.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lwruypwr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lhcuhkrr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wdavudxq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3sdngzuij.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hjgnihrq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hnireqts.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ouepebmq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3imogxyso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tqxdcdyo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pheysbll.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iawkatlo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rubopxum.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xuaeqahf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gnszpfln.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ozuylgkt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3udexalpz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xpsvfkwe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iorcdbvy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gfvvpyct.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrcnga.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3awjngset.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kdytxifh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uuvirqzg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ttrxpcug.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kaxqoltb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kafjmord.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qrectlfv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3btwfsulu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tumfhhmy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ljguslji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3heiqmocr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bgmeyeay.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvgxketj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tnlfqpkw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3niimshpk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3luozfekb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rvsabhob.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jhtiufjw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xeelosio.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkulpsu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3txekhnoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hmszrxaf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3enxehcvb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rgwauulv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ffuseapw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jddytvon.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nodnuecg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lapuuqtg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vmcfrccu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cowdugvb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jauqivyy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tzebtvzc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qgctfeiy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hzodmmxy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3blmglexx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uwyqzndr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cewyjaes.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hedstdww.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jrnxfthf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kjyedbiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slslgmud.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ttiwbokb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izoknbjh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvpezyzn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3phnsxwkq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mdiyiuxu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rmsrzbbu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnrumowe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kueichhw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gccfcseg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pgvkxbst.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qwwjbwyn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lflfosui.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jehyfxqx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dbkoevyl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yimxeofh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3geyarlry.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yntazoem.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pnqtvlfu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iebujuov.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqxljfrz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lfmkuzan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rvcgtzvf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yprbuuje.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vgwirixx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yyfdtgzd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dohqjfaw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jwyjkedw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vclurufq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kyeesddd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sieoahig.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zzggkzxl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3piohwpsl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hgufyach.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bugzaalo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dvbwmdlx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uvzwavcx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ainaopxz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bjioxbek.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ztrlcemm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzuzwdou.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qymrexda.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvrwnzdt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqcrovu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ywnthcif.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aruyhcfk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3byxtbzld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mvownmmc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kjvqzzxw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uquzvsse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rwxkwgpk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cpjqrkca.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kubgsvsz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dfblttsr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qiwtimaz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rkcsdzdr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cnfkquue.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vryuyugs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bnzewyry.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jvazzvxo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3amainotp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oktsvgkv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3newfaial.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kpqkooxi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kkdqhgjj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3oietfnir.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vckceajl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gkoltehy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3safdrvna.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3klignsab.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uggrnglf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cdkbvjpi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jwyafsyq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dxyvszfw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xogniyez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwbqumfa.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xtmpwptd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgsnmqzg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3smwimqkh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3seorqqcc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pidharzf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jlztoney.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mzwplhxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxyfykmb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bljbjmrz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ytllsybc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtezxlcx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3umqxddib.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wvhicppb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3emfslgwl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ckglicem.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3caylwgwq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jttwfhac.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqtnsbe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ieznmkdd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3inrdrryk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ijujkjni.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rrteyknv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mgdkrltb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jorjsglf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fdjrjcze.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cvugaxbf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nliqvmse.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rsdsxqmu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ksyafbip.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dyhtshkq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mncdvzuu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxncugbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pbmnbwsc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tmjuxhko.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cgtxjcvt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rojvomma.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ptdtefsd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ycnulnek.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wevfbdnw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sxuinmga.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztanfzcm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewhcqdmf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3npyysakm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mtsaxiyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3rnkzfood.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcueyerm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wggtbcwe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsxtpjrf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3etocddjl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtwkhxfr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwxbdlga.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgmzpvwa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dgomnnuu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ihwkkotc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pflpzsfb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cnqxiklt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oegqdpxj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uhdvqisq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3septwmtf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dxokxodl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3flwfwmyz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ejczovpy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vyjmgkie.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3asxtnskg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3byxpbooy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3proyjfrg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqzpxbc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3irnbrddk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qamtdega.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zmsxxgvk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jjltvwnl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dmvzdqmm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3obwerihr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ndwpfadc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nuoiylxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ttxwsqui.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ssznysuj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mdbfhevf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3udqegfoq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dxnlxqwd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dxawhnfc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zflkgqol.html


<!-- 参考信息 -->