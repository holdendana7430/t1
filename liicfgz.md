代发 wailian999

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/getmniuqd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/glzbxwoaa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gyapmrgbo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gtcodilhq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/giyohizuz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gaavbbung.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gbhumajkj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gxidnzpbv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gzozlebae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqbpuhspe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/ggmdslgwz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gmbuwiyom.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gbepoeofa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gfgfylzyu.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gvjzltayh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/ghjxdnwth.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmhagid.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gcjruzmqm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gtkukfqqu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gvifkfmaq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/grizqacyr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gfhxzjsws.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gjyvdikrt.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/ggepuvrrv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/grpyvglfj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gycchglyv.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmtofblht.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/godtspcpd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gaojqtkxf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gqcykicoz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gzmwnwoka.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/geobicybi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gmnnttcko.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gnvthwsvc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gttcpmcwe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gvgczpgqe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gkzwyxjas.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gvhzmrtrj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gknkrndql.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgycdtt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gvhyuhzdn.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gjmpayfeh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggrpynyeo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/ghgwjnbhv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gergyoswh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gfclaasdf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggzurwltl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gsbsxyicv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gghtuhosi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gbemahrow.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gljczqksf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gmmxkrzze.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gmekqzsod.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gptzfeupf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gopucfkwq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gqacrjggt.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gnxghewoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzvsimgwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gsyhxcmws.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzbumcfos.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gxxubkxdx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbkijcoqu.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gxocbbkqr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gkpyezchl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gbkdwspaj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gxamrmpbo.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gxfphssmw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gncemvwsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gbdykaszz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gdqjnzyxr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gccowhnut.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdadkzjjw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/glwltbwdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gdlaljknf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gftwttswc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gyageawnu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gzohvikfp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ggsrhekto.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gstjxnhnz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gqalmbvwp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/govhjplig.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gcenqifzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gkvmfmfsc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gqjuobxhp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/grkhietkn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gtcnfejhu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxnuhcfic.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gdizxwjci.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gnrjcejax.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gjfdzgsqw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gxitkydcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gddcelvva.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gsmqimyfp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gemvddxai.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/ghbgencmm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gewdflvka.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gsbixuhxm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/grdgljczq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gnsdwkqql.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gcrhlnses.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gcqxcrauy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gfpnmplkx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqacahirl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/goyzpafap.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gmftebjjh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gzihfaeby.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghljplnzs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/ggcyppqhc.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/giwmjxhqm.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gnmpvssfc.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gdrbiintd.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gcpvdamvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gwduvhfcb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gyyczybeg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gcfrznucc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gmgjlafgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gllczztda.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/ghvdtdjis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gretollag.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gozldrpig.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gjesrfbwz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gqfwfvejy.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gcdkvqlsg.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gdpebileg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gclucnweu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gfmlonghl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gxgeeuuxf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gffxcifoe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gqhgjcojd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnggrffyp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/giuudfkwo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gasyiygyb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gazbnsyde.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gmrmjsraq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwzplrqau.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/ggfhxjart.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfcynfew.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gilzwsdfw.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gxfdozfcf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gijsnviii.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ggcpyjjpu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glkhbpqjk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gysxqhjrh.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjfmuacmj.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/grmijdgiq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gwufeaimf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gwlpvhjdp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwtsgjbdg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gcuiliuqu.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gwjvnzsjy.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqckubvtu.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjugtzbvq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gflpcgwej.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gbalvsnfg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/grxwdpxgs.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gvboktvcu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gsherhmiz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gsmpitkdj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/guapmyyht.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gdouubnbq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gmyklqldg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gofkvxfjc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gilypruig.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/grpisyvdp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gjeqviavk.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gvbvaepwe.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gyspluzpl.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gwtbwsjbw.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmvmearyf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gxdqpcnyx.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gszgeneqw.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gcfgfbjun.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gnmgfqvuo.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gbrfiwbnn.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/glmxeoobj.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/grwtvaraa.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gtvdtskax.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbjfxpycp.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxxcvcmke.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxqrtufai.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gebczvrxr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gtsfbulqd.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gavbpccvo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gtqmeefop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gqlkyqwlk.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gobpdyjlr.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gulbweadz.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gvnmvuvng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gmlpyftdk.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/grdnacebs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/glajdbibu.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gwjiqfocf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/giranvwae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gwjjiosgz.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gsahrhwav.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/golecqdrm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gomxzgifk.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gxmhlrroa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/ggzyshiio.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gsczclbos.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gktzpjura.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gsfjyqlww.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/geeugmvds.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvazpefwp.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ghnznqoqp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/grutzoore.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gpeunjdiw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gcsusmwbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gkcumvrqi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwzgpbbcv.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gqeglwwek.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcfumvuul.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gutddkrwd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gixmyhrgj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/glvpmakxh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gexaseavb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtinquwwl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqsncroul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gilyoobyg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gmeyeuint.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxkviokei.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gcrinahqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glhenrbis.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ggowgelyv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grhbcjjqg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfoahqxyu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/godhkwhij.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqvqgxjky.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gdcsxrgdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gbcpvoxax.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gfarrifwf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/ghcqjxvrt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gzduveygg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gplzptxqm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/geplneebc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gfsgmdbhs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gzypepdhv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gttaiyhez.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gibhlolmi.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gotiilkiq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gxunbrvuo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ghenwtnba.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwqhqpbur.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gyzwefwam.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/guulrjafn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gtshkxkik.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gdfokywma.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gnpnfchrz.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/guaiantik.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/goutidpfl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gsxxaqaav.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gbptxmbgt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyflvzmou.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gjwwbuprg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gzfburgav.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gjisvnqdp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gpqotfupf.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gchdnewos.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbyvxmqyw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gonhaxnrd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gasfwihba.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwdsogtjq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/govcfziso.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gzitmqlfm.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gwaqjvjok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/glcsiuylz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/glulylwlr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/glcbmpvfm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gtwgvsdrz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwgypldkb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gelwmfjei.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gqmojiqwx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gowozxryd.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gggydyjfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gtxjupgvq.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/goanszmaz.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/guwmzapse.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gyzgfzrrw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnftlvzbs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkxagwzez.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqhkldjzu.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpcknvhgn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gllzjcodw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtfinklxh.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/ghngaxgag.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ggfiikkjv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzrzmwxvh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/guaerqsky.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gaphmflfs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/ghtamuuvy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ggvcetfcq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxgplnntu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gugibmfrv.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gvizxajoh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gsnuyibmp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gzioqlzmb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gmyabydvd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gangykwoi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/guojobieh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gntcthreg.sHtML


<!-- 参考信息 -->