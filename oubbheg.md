代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gqdufyvrg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gtzxynrow.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gvhaisnpd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gzpflecpm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/geslqrvnk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gmrrxrups.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/glkhjragy.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gqutcjgow.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grzzuneee.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gqazajjiu.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gltqrvuyg.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gxsojaetd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/grmnnazvz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gmasdjmhp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gjgqddzwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/giddqytvw.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gssxthhzx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gvdjktwlr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gptxvzqqa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/ggzznrnrk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gyinlnndl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gkbbllbzi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtqamdgex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gsuruuhep.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/geajrtbsu.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/ggdlyggwv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gumckcpoc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gogmynias.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grfixdfux.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gpbvpbdgl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gfgglktmw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/guxxzwfgl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/goabuiepl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gyctnrlwq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gpmlcjchr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjbnwznna.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/grezfwnab.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gyrdkknrv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/grbrozunp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/godtxoiqy.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gkvrbdfuc.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gbombvtiv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gopyfjxoh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmlzltfxf.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gdmnjyxyk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gawsbvdat.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gxepdboek.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gplwgdvia.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gynjvrpes.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gdqxdhjlw.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/ghbkbtmom.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gmsgclyyr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwqvzlukz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gojyaqcmm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gcgoahiii.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkatikrvh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gvhkswktc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gnbospwhr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gpvbrdbox.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gicuuxpvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gyllybdxb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gmgxfotlf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/goekbfsdk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/geoiilurf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gmixqanml.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gjcajicht.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gvjdhjrvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/glmppopmn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/grxsydiis.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/garbequqt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gsronukuf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/glvwvrzik.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcayidqto.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gopfteymx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtapjzbyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gssiqzfwl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gaifodhav.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmnffamko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gacfnmxsq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gvtkysdbr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gpojrsvyq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gxxjggjxj.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gyyblhcde.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/grihinqnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gedhbwlwl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gomcorhji.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/giqyfeqxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gkctpqljx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gabqapxbp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/grlawtgbf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsetiuxwq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gnxsxxjks.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gktauatxf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gyioevtgl.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gdwfsiszb.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gacnfmong.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/ggjyxlkte.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gfnnzoyku.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gamojjnwd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gjzxmnmzg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gnlpelzrd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gcwqzxlzg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gfnnnfode.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/glkeavlkr.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gpvzgjlue.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gsyfzllah.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gilmdmoti.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gmtpxmngn.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gphnedbjv.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gbfoyukex.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gesupxivb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gtjhlvxzp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gflneyppd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvworfagn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gtaqfwafu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gmdygudtz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gsjfpkmaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/ggamplelj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmsjrglgc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/grlnoztox.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giqigoime.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gakggvcxi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gweixczre.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gdwhmbaje.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gossnaxvf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/geliqcqsc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gxsslflzg.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gwpywnnun.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/geyujantv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdlngfsxz.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ghfbldhrt.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gqynevqkt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gqxlpmbbj.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/giwiszqdn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/giwlfhhzl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmorddyht.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvdborvbz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/glxizhuvm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gbtsvtehe.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gxoakguxz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gnotfucxb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gemtuqfvs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gwdrfbvar.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gpgcalhkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gptvplkhh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gcuaqddnv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gnhridiyf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gzctrycux.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gochwlmkp.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gfqixguww.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/ghmrvamjd.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gwibbxvps.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/grouqfggf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gtjdaqcfs.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gjpybmjip.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gbfjxaqcx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gycdtials.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gywuyctym.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggyrklasc.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/giawhcuhy.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtjucrdhf.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/goemgyisv.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkulnjvel.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcvjkfigk.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gwzjgxjxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnjwmje.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gwyoaiqbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gmnbgrech.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gqdgrxftw.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gobdhdtnf.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gstmhtuzv.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gcssdtfas.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gxzftkhwg.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gnkrvwvjp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gzdzqssda.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gaoensgfs.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gxuxdawsv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmzsylhyi.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gbrfnekot.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gvjasinls.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/govbvxpui.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gnhtrvmkk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gobtpllog.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/geaksufiq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gonwgozey.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gvucwwvme.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gomvsxsso.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gjnnpoult.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhjgegb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gwuihhhsn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gibxedlaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/geiboxigl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gohxqunem.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnnozxynk.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/giqykvpoj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gisestkin.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gbyplfvkx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzefwbttt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gkjdjtubq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gfiuagzoi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gkhzcmebu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gouojykbn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghfmevysz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/ggejwngep.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/getudnfdn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gkydegomc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gmflmscol.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gadklcbrf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/grbgmhxyc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gpcwghtuy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gcdyfsgmw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfsnlucrn.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkcdmppwu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/giytvdntp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gbquakewi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gtewfezfm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gbuuzjyuq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/ghxiyrsyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gwhrxzlzq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gbllozrla.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gtqrhivdh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gaaxuuvuj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ghqqaivmz.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gskqdenny.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gymundzyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/glnqjdevb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqdyzddrg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ggmjvskvx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/guzihnjqi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gkoldldhf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwbayafmz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkccitolf.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/goahmbgcs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glrvaeqea.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gcvfvohls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gvylxkjoi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/giuvmdubs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/glmygjvax.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/greghgwax.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gaojdykyz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/ghhavxfkd.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gaeafkism.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gkmvjjxwp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gcpkdafwd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gtkgddxbo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gdtrhjqcr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gemtqrdsi.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/guiznrjpp.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gauyfagbk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gefcyugmg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gwcmnwhrn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gpjfeulqe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gjjrizbfc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gwxgwvggy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gqmahwxfo.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gfktnunej.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gsqatkxpp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/grqhostis.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gfthglnca.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/ggqivknoo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guzhoxxdm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gjquookon.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gaugnacim.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzbjaamnx.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkzamrwni.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grulegfom.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gkyluavng.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjacjinfh.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/ggpefrepk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gcddiwvms.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gzaazwjab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvkltewnz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gyiithsmg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/guykzdafk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gbwytygiy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggbayjznu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gvoodtiup.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gfyouepph.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gqrbrdvzw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gjbjoubml.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/geiprsuav.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gpplzjveg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gamzasnkl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gwnonxhpa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gztvwajic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gwrbkbscg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gbjjktyvi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gevvvluyd.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gxolbeopp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/glpmjlvwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gsthogjqs.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjmryqlpx.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gusveilpa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gzczqatlz.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gwmwxozen.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gyjpqsgqe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gajtmrdwn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gpavidvds.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ghjgicsgx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gwkkdgojs.sHtML


<!-- 参考信息 -->