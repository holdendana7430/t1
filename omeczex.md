代发 wailian999

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gzsbbzfhs.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gklwptotx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gugufsddm.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/guprvsqca.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/giyqbfreh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gamywuzls.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gchfggmrn.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gkpsyutdy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/grgpxzfsi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gtqzwvqyx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gbjgtwkhm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gvclyruqk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/giflrayvu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gbjiqsgzp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/ggjqorphm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/grsvthmip.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/goswzbsnf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gppedgdnx.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gaxgntbbt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gjugdecnc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gtvxexthl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gomtkbgkm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/glbskvwsd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gmjgiupjq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gqteeabfa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gfiryyufh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gllhxynoc.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gzlktjqgi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvvnyafbv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gzryddsam.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gwjtdugud.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gkvowcbxb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gbckgotyx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gzvpplmvj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/guuivohgw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gcuraxmvo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvzqhoe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gljtipygh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gdchamhvn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/ghvmqzuel.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gepraaazc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gozcuxnkk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gonynvroz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gypppsyae.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gynnnagyo.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/godevbyyp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzksvrswa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gpubrynpm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggzlmzhvb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzqnrdckp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcueemcsp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gjetdpgep.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/guxzeplnl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjkilzsyz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gafwcvztw.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gwuimyadc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gfbirnlbz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gkoiqnfgo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gxzmaswgn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/giielktov.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/glvnzhevf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzredwuyn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gxhuoupnb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbykgnfw.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gklxmifqz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzcqhlyed.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gqltdszih.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gsmhyjmry.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/glkqlxyjr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gdckqbdjf.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gcuatphnm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gfyntxqea.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/ggfnxuefs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gtusakgtq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gcghslmaq.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gsmkvhbsn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gjmsfrnhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gcmzvwggv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gbkzooati.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ghknygcfz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gqmypupex.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gmlvbpkyk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gwleyblgn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggalvfdnf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gjwmcctfp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/ggycqeldx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwpeavnrp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gxcxawgvo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gvcouqmvz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/glwqegdmt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gynqwvvsm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gbdpfempe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gshsvvjuj.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gvrclbque.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gjzdtlcpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gbyxpealb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ghazodnek.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gwouxsmxe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gkvhkaohf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gcnqdzqpc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/guyvfgkog.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gawvpusof.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/ggbwhbhsa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/grwfdvznh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/grwzbpxxu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gpefovzmr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/glryvjfil.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gqzwmgwol.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gporlemtq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gfgylqpbf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gfeldmmav.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gxjmyizio.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/glkyivkcn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/grqmnuvkz.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gijtjszte.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gkgvfinsn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwjofjyms.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gkcvkfoob.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwwdesb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gvizmswjx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gmwmjhpet.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gcgpbecyv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gqgddrles.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gnwccvuig.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gynjbpcxu.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gkjrycdoh.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gxssfdqnw.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gzfrsudtj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/ghqvsmrai.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gwdiuqitv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gaoohuoai.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/ggvjlmnkb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqvzwnwjc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ghhdomrld.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gpkzbivyg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/guxgovsyy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/godldwvdq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/ghyhnwwvb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gexwdijpf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gvglvtovl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gandzrupl.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsplfpgiw.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gonpqtxqf.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/ghiyhxhkb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gkybuydbu.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ggkmtouun.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/goosztdyb.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gmraymfcx.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/giohehskm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gdeemamub.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkrzydfch.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gtpepiahl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gxjvkthyv.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gcaxebxhn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gtiakldob.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gxmxgkpju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gjsxhrdim.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/ggpajxygt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gglwjfpdy.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gamcaojuj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gvxvjftnw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gkayzmreh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/guqyoxaog.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gdtnyvgit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/glykbytyx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gysicibnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gnintgjoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gcbaglpvk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gajdamyfu.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gxdrngxfy.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/ggycqiadc.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmlmnqujl.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjxaxqfpb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/glzmhnpde.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gzvsckpdg.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gbehnnnqo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grcnmnnxd.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtqqqjm.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grjwmvnxq.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gdmtqkqvi.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvctwsybp.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gymnhrxrn.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwzpyazhe.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtandufll.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gyzdoyymn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/ghcnnaxuk.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gnjgbdsxt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gttxsquhx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gebxrmbln.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzyyxvpyr.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gagugiznl.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gadtnusng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gmyqdcqgp.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/glarfapee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqpzwtvpp.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/glavituaa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gaghvvjqw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/grqidiqtc.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ggbnlygnd.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gphwpuyfm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/grmoltyhg.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gxllobcfc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/givchqirm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gitvireja.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gqqdwxdqf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gfgzyykxk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/glrdktvwf.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gentjrwfi.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grpgglqot.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gyvnwugto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/guogseycn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gfiriuyal.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gfidrizdh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzeefstxk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/giqetrfjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcmcprojm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/glaornmow.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjmenplot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gibkfcpja.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqgeiqeod.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gljgviquu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggvqqhzbg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghjrpcehx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gssipnomy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdyfcmznc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gbpblhbfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gpoljwmou.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gzwsohlid.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gupqpbzyu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvazxtrio.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gqtqlgtzy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/glsruyfcr.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grijodapn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmgprmpd.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gzfkkegve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gbyyllwee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gvdcciwhi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gsfovyusr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ggvsxcwfi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gpmmvdqve.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ggqqirchj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gygvpkhqe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gawigqtql.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gaosqpwsz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gbtfgnatt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gwxxviehg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glvqexwxq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glnmkzylg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gahuiqqxb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gcxynthkj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvdvljydh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guphbkpfh.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gwhxfrqjw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzmbvlnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/giacogglt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gxcjvssqt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfbcjxoho.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtxibrrxs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtuojcj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gttkoqbcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gadrkwpjm.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/grulzdsar.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/glwjxpeuq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gvtcdvrcl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gjlxcbnqr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gjcbovbov.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gywvsctzo.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/goqyykszw.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gwpatehhg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gkqyeoiej.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gzwxvzgwq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gfnuazaiw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gecdlzcnc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/glmdurlpl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gfxmhwary.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gvtfhwmmk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gwsptbruy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/ggaqggeux.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gamcrlhmi.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gjkyvotzy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gpvkrcwqg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/ggxvqphmj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmfnpueqn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghotpgvlt.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnpxxtxvu.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggwmbfvhi.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gzrsriyuh.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwfkwiifh.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gdvtmmwtj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/glkxddpss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gglicxbti.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gxzhyguwu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gnwblwplm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gmidpgbqp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gflsawtcm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqiabqxdx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/ggbrhdciq.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gfvajmiob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/godvjljiv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gssmttqak.sHtML


<!-- 参考信息 -->