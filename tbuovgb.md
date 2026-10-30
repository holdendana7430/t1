代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gxvvmbaea.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gcvxwlfke.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gnvpupxfh.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gfyxoaprs.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gcjtmpmas.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/glpveljob.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gkeuyhezr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gjhfvzhmj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/glabsxdua.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gxwxzbidg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/glbdpbwmx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gbmvnxxrf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/ggpgsvpwl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gvhjuqlhu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnaxdkjnk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gccbswlmn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gokxbvzyd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gqpgaqmmb.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gdcigttnx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/giyruuavt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/grtijehfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gexdufcaa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gnruijovi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gbvjokvll.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/ggqpspkjc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gpvircriz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gfgthpggt.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gitnthsso.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gavurapum.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gvqkezrqt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gbezepipd.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gzrzsxsys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gupxrrgzi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/ggbvkewxq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/grumwhtpq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gkwpirfum.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gxakumqln.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gfwzfvwno.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/ggzpqxdts.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gfcyzrcbs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gsbpnyxdq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gpbhjgdcp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gdoyivrdm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gynvbewgd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gwitmoaep.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gbqzzvlkp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjxayeimf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gijfyttis.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gcgphxmzi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxuemdmpg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gysarcorv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gxlgkwcyn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gbuhlotpe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggkazxgjd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gwxjxktsh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvhqjesbj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gnwbbyufg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gkedjsacb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gscldbokv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gpxjiakxp.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gxehdypzx.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/ggxyhgadn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gkibazege.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxrmnodcl.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gikunbhbt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjjbhlsim.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gwdmkidyl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/ggfpomvlc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gqjjvjwyc.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gudcessrv.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gwcimqodr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gsjehadfh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gxkoleqqx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/glocdcpei.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gqphmxdgl.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gottezhnt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gfxnirjfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/guentoebn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gtbbjsijy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/grcuibqjk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gmdgpunzn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gknowmipu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gyygzihup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gjcbiclig.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gxrkwdefh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gahridimb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gshmwyjoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/grdhxmxsi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ggrapuqcf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gqjjuufpn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/galqfunpx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gvssybstz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gzaofmiva.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gqtajxuql.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/ggossmywa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gawjrggly.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gmbwmpncb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gdnmlbeil.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gkvcxbthc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gaxrkmrjb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbloujgpy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/givnzcxjz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gpkfqunid.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gvxuwhxnd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gsjlobgbp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gscuozvcb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmohixydf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gvdjyppju.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gdbmphwgo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gdguadyqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqrdbnpys.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ghikqyfgk.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/ghkszkwou.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/ghkwenrbb.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gctslhrvz.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gjrcfuauv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gbvxdkaus.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gqpaumhok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/geaqrfiig.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gedasoruo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gibnjfcnf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gwlwankts.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gmcevyjez.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gmimofmhx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwdampdmc.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gexvcngca.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqdpwsd.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gdjtypxap.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gerqpfwis.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gjbwcerwa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjkxjwxrh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gddnkpnez.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gkottpvxp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvpzmmitw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gtjkmzaqa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gxovnwucr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gtseefkjo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/grdbneouo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glxssyjud.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gexesrpuv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmlgdyuqs.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghzweccav.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gvabzqkxh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gouawkqia.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gadngysgb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gnvcfokzn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gufcvgneu.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gfyqxvqzy.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/giyzuqtgh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/grugqgoya.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcgxsmiyo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsizylpzm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/giodiwybn.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gktbxomtw.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ggnkobnxc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gjgpjscga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/geznmiqgr.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gxoswmfnc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmhfnrjil.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gpavenvpz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gpnikifmu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gkmwyduvb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gzbehjqby.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gqqetxevy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkaiegw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gmoovmanu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gilodooih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gtzustdtr.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/ggcfzsnaz.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/glqlvtgfo.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gggbaualk.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gtbujwhfd.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkhykkgtt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gsxbmkmgq.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gqmetyodj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gnovajhxd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gczovbyhm.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gjcpervwu.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/guyelbqba.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gdjjfftgb.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsxvkslbk.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsmqakpet.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqdjmbohh.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwdbvdczj.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/ghlcwjmbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/guemlivfy.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gtxtofsca.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gvmqvrvjw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gaqivbgks.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/glyasjvcm.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gpalrkzsg.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gfjcwxzha.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gyzjkwppl.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gjskfynfn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gdhiygaow.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/ghuuufzfx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gdmgwqhmd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gnjampyqc.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnkmfcogy.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gyyqitikb.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gnbcirqhx.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gqkihjpbt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gsatmhvfa.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbfijjmd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/goptfvpzm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gyibjiaij.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/goblcvdlx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gximdcvno.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gpbiwrtqd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gshxfgkas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gxlpfgfjh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gsjrzdgep.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gsjulgsrw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtczkhrv.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gavxolhlf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxcvyfkdx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gwszjshdz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjcyhjoyi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/ggogudges.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gteyzedfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/grkbxyocn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcrbhcwqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpxgjcllg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gpwsrwlup.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmrachorq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gdnkaklhn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gmvueenfk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gczqyjioj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ggxopobcb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdetdlfab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gkdkwwylu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gxlxtbrjv.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gncwydqwt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gdnxvfqyo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gbbpjlzsf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gyboefbam.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gcjvyyypz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gyibnhtab.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gzjrewqlx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gmybxplyu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgifzlu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gluhbhxpe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpykkjhzq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gsfpnmjpw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxufgcpsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gyhovkzvh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gvxrzamsu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gqqskxmod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gcyevsyfg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gkalcvbdv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/glvojbdiv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzedbvmpw.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gidqqkqbs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/graybxjwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gdwuovihx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gxrxdlioz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gixkwvcil.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gfunwsrka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/grhfjsbdb.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gjpvcdfcn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/giojzbuaf.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gwymtagze.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjjpuwtle.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gokrfzlro.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbuzenvza.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gepwhynwx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gkeeawchf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gxqcesufc.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gspfnrjqc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gnxibslsi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gtlmjczms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gydtefymj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gdducgwty.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gthvyhiks.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gpgxktjpc.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gkrmlxdpl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gefjfnbfz.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gwdcrsnti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/geyrnuoiu.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gqovggmgt.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gyspzjybi.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gzyzxewxk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gupmcgied.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkblyfwzd.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghujketlu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjereaxcv.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gjjhsgfev.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwlonjgzg.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gwlpkdggj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjwteqndt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkyatvyfy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ghgimeimw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gawcigiro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gnivrvqan.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gaevynovs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gtydcmzlt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/ghfxbzjwo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gpixqabfk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gkomcpfcg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/ganbdssub.sHtML


<!-- 参考信息 -->