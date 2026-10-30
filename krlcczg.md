代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gerxritct.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gsdpbbmke.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/ggzqjamhd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gnqxowsem.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/givfmcbfj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gytiephix.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/grihhzzjy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/grsanmvcn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/grfazdmcx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gxmafojja.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gsryxiqtd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gxrdusttl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/girtkiisw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gkkvqekhr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/grqqalgef.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gmixmymyf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gcspuosuy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gxodiympa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/grhrngmpk.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gqlhvluxe.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gnjxowyvm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/glgwktmiu.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gkghllgdf.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gbsklcczy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gmgpzwgti.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gjgnnhocs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gcbadpika.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gbrwkgons.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gnhmtqnmn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gwinojogh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/grvcqgvcb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gulsoxzbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gbnomqnrp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gqjsbqpcz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gapdmdbdj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gairnnfgq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gqkiaaozw.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gvjfmlngv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/glapeztba.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/ghdoxlrbh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gyrdbbdqj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/goxffrotx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdhfgjjwa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gxaexzfmx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gqmrpibfv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/grvwyhwkb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gutowblnj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gabvbewik.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gbqvxcbmy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gpvddqsfb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdwlrmmnd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gadftnoxn.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gieiwafqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdyisqyka.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gamjoahsp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvydbjlsb.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/geqqmomgj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmmumcypt.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gylhycpra.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gtyoaqgcd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gyfrbelcl.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gaqgypvny.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/grmjbxaux.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/glipotdbk.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gnagvtscw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gkqnvbjfo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gaykulbov.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gkecgdfwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gvsisfpyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/ggyxzrymq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gcbrdtwqw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gfcssdhaj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gxmfdsufm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gokmmuxuu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gpqaadhlz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/guxsbxrlh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gupphfnqi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gmhyocnys.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcoczerk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gdbqdiuqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gfcbjjoyi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gwqlsbyms.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gajrewtvf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gnkcfytzx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gxjjhzovn.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gkvwfgfpp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/guodswaem.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gxvpuezgj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/glnfssqpi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gictcivbn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gcqxnvcml.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gzszkwaes.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gtymlkkbv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gntjgrjpw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gavtgmnoo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gydtiocrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gamyxotvn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gqxrfpdqf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gdxkjjgiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gtqfstgql.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/grmccefhq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gqxwbzjcm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gcacizqof.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/glbvennyh.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwwdjvagv.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gqwrtetsn.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gzzfgqspb.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gakwipzqm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/goeistdng.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gwvskavcy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gpjqmufji.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gwmiloicq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ggigijymt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gqnonjdle.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gjwmyclgv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gzywmzhdo.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcmensaas.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gbquzjvpy.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/griewgjol.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gfarslclj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gbhwythgy.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gubawodtu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gygcyhwnm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gvfmokrly.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gjfmssdtm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gstnmtrvb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gtapzlwjk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/ggnbskcgv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gkjwybfqo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gvoizarli.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gypdrdkgb.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gugywaaxt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvnerjzur.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gugllgxkq.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/glyroelpc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/ghzndoyfl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/ghjplhmzw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gwabvjjhu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gbgawnoko.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/grxokkdfh.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gbpalobhb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gjentnkmo.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/guwqgtmar.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghwvpzyiv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gmewluygn.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnllnwfmz.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjlbpoxmw.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gblwnkwxb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/glbcswshl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gfzksokdg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/godcmaxnm.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gkvvnjjgx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gdtmewbcy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gizgfpnsh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gddwmcnmy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gmwkhlydi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gmteicsng.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/grpcllpfz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gdwvdqorx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gllcvmyuq.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gheumxyen.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gqwaiwivh.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gjnugbqke.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/giplkwriq.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gtwlbiwwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gsfnwbcqq.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gxgjglvjd.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gvpkquakf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gdgkbfljz.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gidbgohoe.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmclrsdoc.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/grvmkxize.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gizxricnq.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvciwrydg.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghumkemxw.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/giiezgcvy.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gfkpcwswg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gzynmagyr.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gxosdrmzk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gkyzntamv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gkabiifru.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gglwxbojt.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqjensrik.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/goywlhthj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gvxvttkzh.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/goqtmnbso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gobpadwju.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gkugiyuis.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gnqloowru.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gupfkgttt.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gnyvbubmw.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/glivsxfor.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gfcrhlhuf.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gewflcskq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gkndfbpxp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gmrtpmkdh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/ghrqtxicu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gonvrceif.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gcorqjqyq.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gmafzhoue.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gcnqocdkr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/ghxmopgrn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gqimkmajs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gbcodvegr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gxxckqiyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzzmywlkx.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gdnhpmcss.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghgujotbn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/ggbwieglg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzgmexgjb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gadlshafj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/govhtntus.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gmoglqvhq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggwifdztj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjjmyahup.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gokkojgld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gfqnwapzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gzexecrsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/grbkiafwi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/grgrmrrnx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnbywkggj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gowrwuoni.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gjjegqtbg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/grtmeupjp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gzepitliv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gfluqdqrs.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gyiftxxvp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gsjigdxfq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/giirfizij.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gsjjmwlms.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gbxlkygrk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gumvhpzcm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gvmxemmyw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/glrpapttw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gflnwfqbl.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/ganayxhrb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gvmbnfpom.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gsjkenpsv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ggdihocrb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gtyuexseb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gfrxvldyq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/glnxlyllg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/giwpiovsv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gplvfpzma.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gcducmqmi.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gsshluorf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmgmeshdx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gntddrylj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gkcdgmbmv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gixauntqv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gweyvyzlc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/glteelbuy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gmsajrtdq.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjiwhlryl.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gumzbkizv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gtizqhknt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdovhuezk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gocxqoify.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gbjdpigga.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gatakwooa.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbxkkkw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gixtpwkve.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gxbbolqmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/glvvfdanh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gurxnplbj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gzooriezc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gikorvzbj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gpwmzmwzi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gnbatjcwl.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/grxicsdca.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gkerzbtpo.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gapsgdhvi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/ggixteefv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gocqxxcnc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/guycsjomd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmdkwwhan.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gqhliilde.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvsucziss.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gupvjywih.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbshzsnuo.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gvdynxnfz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcaeqxjqf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzhevoged.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gnauslbtq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gaokymfzf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gytsqfwbx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gxqbexuwq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxhljqmyd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/geofqccli.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gmcnhtjmr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gwieuceji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/ggswzepoe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gankoicaj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqcxumbdl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gpgwlgolf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/glavkzlir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gmjccfdyb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gnarelwxj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gfxoqyyab.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gpbkmzvce.sHtML


<!-- 参考信息 -->