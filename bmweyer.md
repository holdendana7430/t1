代发 wailian999

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gesypjvas.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gyhgywgkm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gimdpockn.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvssmkobp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gztmjyfwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gvounrzai.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gibsrfvqe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghrrggdrr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ggqysksbz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/ganuxexvu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gkoesnule.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gthsglitp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gibzebgmd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gtfrhkwti.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gwzoqiwdr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gburwnvgu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gfbfukaog.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gbgneyyrh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gkyynemnj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gklrfqhef.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gckphumxo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gfgzjmfei.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gtuhmnyoa.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/giatctxwl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gtitliatp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gmtiypfsw.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtjqhecqw.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gyjyyxmxs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gsjvexsfi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gxaeoqzam.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/guulcrrit.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gnynnktfa.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gvitaukmt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gpcxrdysc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gnlhgmrzx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/ghvkbitjv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gqhmoofhv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gvdsjnmyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gikczunwr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gnksjmhyl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gquillhty.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gxabpbftn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gnfkjpkqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gintzjjrp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggzopzbnw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfyefzbxp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glcbfhaip.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/grsuawwxc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gpfivgpgy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gtjrujpwp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gcnstzkxt.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/grqqqlyyh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/grzzocqpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/glsgrykzc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gqmxwkeol.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gabuuhfff.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gnnfrgtgr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gtdlyqdbb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gktnohiyv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gybcllfjv.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/grhulqocq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaykrhlat.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/grxccsuvk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gzctwmogv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gcgfchkin.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/ggwuufyxs.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gptqgttpt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gishddain.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gajnjksab.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/ganbddkbl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/glovxsrly.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gtayqglit.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzdifowjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gevokfmxy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gawadgaum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gardqgamp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gewerglto.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gtizvcdov.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gcqvyeivk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/grvxfrhha.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gtsqefcbe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gpavjsbzv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/goylhlrsk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ggolroyft.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ghjgrwult.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gnaqhtgcy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gegugyjll.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gsfolfbwz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gtjdnnvhm.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gyqkvkjzr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gqwiojvjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gejnmoqhj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/grdtpkacc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtpdtnyyy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gkxjpvuiq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gioxyxjhe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/ggebjaoas.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gteufjuvq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gurzygstw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gzrtbzqik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gbbbzmmuu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ggpjhgzhw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gcihpcpnw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gxwpbgxxu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gottaavdf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/grijsvsfh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsyzirxey.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/glvlyfihg.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ghasogykg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gcohccgzt.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvlujauuj.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gmwvflkbs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/guwljuunj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gpotxfoxf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gxltavqee.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/guhbvxtlj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gwadadpuv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gafykmzvb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gpqtnycqy.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gbuutxsjd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbatmxzny.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gevrxfbkg.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gaggfuzuq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gkszamwjy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gqvxkylsx.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/goafmgppd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gxxilqjse.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gudbuupjz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gabtinjdz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqbxnbrkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gsqfbpule.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gjvmtsbxn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gxvjmfppd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/guotnxill.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtnohearz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdeshfxsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnwlqqlqm.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtkjucgkt.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gqmjbehah.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gbwebbgtb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gtjcyqdfe.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbmrtzwex.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gxmvxazai.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gqddnjqyl.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gcbgupcsr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/glblhxmgz.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gueoagvcl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjnpnmmyy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gpksyutra.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gekcjukmd.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gooazbntx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdmpkazqs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gdatkjbzi.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gksinkqsg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/grawpkrpg.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/guxpzqfwg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gbztlyefw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gipbezstl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghdiruzbi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbmgrlppn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/ghkwczmuf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grihbexcp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gzqdxxcbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/goztntyjb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gifpweknu.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gydomlrqf.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gunvduyyr.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gznneokjy.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ggdmscwgk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gyakjnysz.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gfsntezdc.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gthxtfrto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gscwboaun.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/giancehur.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggqunxvhz.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/ggzibevyv.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghavaigqp.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glrqgmerg.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvhjwgzur.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gbgwqddnc.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gfumgaaty.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gzwbqcfkx.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gwisvrmul.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/ghjtlmsbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gcqlxygxe.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/govoqzbmt.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gytrqwbwy.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/giqvygfkz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/grbfhfcbh.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gjmgkrlom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gngwnjymq.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/ggehoairy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gnwuuqhbi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gpfakgyvr.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gebtfulay.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gtlydfdhh.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/glrfditnb.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gbhohwdrm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/greoyrqvx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gzlloprhq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gafgrotzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gixgzzgzy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gysbupnpl.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdejcxify.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gyamdrpka.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gkwmbrzlp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gdjbpnwmf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gtnazspgy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gqyfkgobs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbqdsbqbs.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gidsgebuj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glndcrvfv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gypfnvons.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwsliufpc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdriammwm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/girbfelwi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsgqnatul.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbafwbsqo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvsdyiuvp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gibbbwhkj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyxhwyqey.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gtljejgxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gunhqbvpo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gjtbaxawi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gteenouah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtjdjwiod.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsagjzbwx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gzljndnqf.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxnfasjjd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ghifqnxqj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gldufqlon.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gwyxozbap.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gfzgbjxqa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gfybiritb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gyvexnguq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gniqvdwot.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gyucurzhv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gypiqmnzf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gsrfothkl.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gfvqtmfft.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gmullppzt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gaizzmshe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghrhzwmop.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gmrgyokzg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjehzayly.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ghjxmvtdu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/goevwldyp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/goklhzopa.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/grmiqgypu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gkkaiuysr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gfemlbvyg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvjxjvivr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gjpkzibky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gsgyxedpn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gafrhuwaa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/goffspcwo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gkeehuzkl.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gizxlmzau.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxlevuano.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxvitxcba.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gppjzvxiv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghnpkvlbe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gnovlmtjl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gkcruqnqk.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gwtmqqacg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/glxahfvsv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gwktqdefd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gxxaztdqg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gifwblnfo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gqlyrhsep.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gmegcmwwq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gzwgrnxbg.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/glupocwtu.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/govrwhsro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gfsuwznmx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqsmgzgae.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gwxhvmlnh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gykklesui.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glivcdywm.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtgcxqmze.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gblypbhfb.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gevyxlyyk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqvldsxis.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gymthwpzi.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gzfipfppy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gascuihnb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gohqugjur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gknwtcrwv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gxpwkajmv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gogakqcjv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gdqbnkhho.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqshdnpcf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gevcrpktj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gdsdfxhrh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gxpjldxzc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gziyftbsg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gcpwnbqjv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlckolkf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gfmnbdwep.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gkzzhglwx.sHtML


<!-- 参考信息 -->