代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gxhyppcls.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/guznznrri.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/ginnfhtbj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gyyucvgcy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gaozytyba.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gmgdlxudr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grmqkpxir.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gqekpzybw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gxrgjtrxk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gievbgxyt.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggyplmros.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ggyjtnchf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gpsavaowc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gwidefnay.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/ghqtriumd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gdhnxuruy.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/grpqhnfkc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ghzhwxpaw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gyeysjcpz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/giogcpkvs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwjyqcdcp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/goqldidby.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gxrzvulxx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjwzkqixu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gobdrejmn.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gtxflhxri.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmkoqpvlv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gkedxktmz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grdwruoud.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxgesevtr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxctaokii.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gapcnjhmj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gdgywuhxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gdpoqawow.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gzkhzcuwn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gdvduxzuf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/ggrhjrimv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gwgypaint.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gigdcbavt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gxpccvnyt.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gemikjkvx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/ghdzjopps.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gdbpkvbvd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtuobgejm.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gperdkxfp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guleqidkn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gvdaoiqsb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gnqewlagc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gmuvetqpa.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/grfvvstyj.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/ggihcvyyh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/glykjfuwi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gyllepfgf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gsopehnqe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/goywxhcue.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvswmkpeb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gjvkuvuyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gyzfpdeja.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gwxzxgtnk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gsgvtrbgl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gwvybffzj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gzmrcuhzi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gqkyyhekl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gkzxywyrc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gxnonetkz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/glxmewyyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmcocxbdb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gqulwblme.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/geylgzqtk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gvggybdob.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gvqyorltp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/goowmbipl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gmyuyrqdu.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gbyqqwwfl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gbamyezck.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gqimgpqod.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gbkqljbvd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gsahhldbm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gmqxljste.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gjifbgbef.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/ginpodcyb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gjuifxsws.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gsqyhulpa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gmldilpgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gifcwrdju.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/glxmqytgy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gbuicztmj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gojuqtxkp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gavfqxqqw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gzeeeiwdh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxliroihr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gtrcnznwn.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ggryjlnav.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghrerjsao.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gyethtefj.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gsannutya.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdnuapoly.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gszqmplhp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gqmawmkev.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gndpdyfwz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gstnmfzpm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gnawmomqw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gdouprbcn.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gzkpebpzi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gftcbjquz.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gppgqtujf.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gketscjyt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gkgjswdqp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/glzgrnrlv.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gqwhmdnjb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/glismorgk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gkysgfpwd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gistejlqp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gobbjwlim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ghgognamc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gwiccyxnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/guqbephzl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gnxjequku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmpmazmzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gbgqewpoi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goyryiwaj.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gidoyyzer.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gccbrewcc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gzhxalycw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gtcabmwud.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvmmgvtnc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/geqgehtkp.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gbfoafnxe.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/golkhjkxd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gpbiyuszr.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gxzlovsnd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gmtbntoci.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gslumsgiy.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gcfdhvmde.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/grpsadyat.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gbobycihq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzwmfxgsn.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/ggtpecfqs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gbxxlhzcr.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gygkknrho.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gblypaknb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gsvbtazwg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqhcgkicr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gercclgih.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gxotcnvlt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gugobavvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gxzcuuraq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gtxpzfbri.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gepovetsy.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gaijpvjhg.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/ghbbghreh.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gxzjbjzih.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/giuqszsdf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gkiibkdek.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gwcuuiqwx.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gamfiwrml.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gsxrdjnlt.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gkzwifnjw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqxstuklt.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gzmkrvsax.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/guarewfhq.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giaqqfslh.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/grnvujlps.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gidyixkyt.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/glrsrvpgb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gjkxqljua.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gqlstcpqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gpydvglgn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/ghvgdwdux.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gommrczqo.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfnvedjfx.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/grsgdfqvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gnnmofsfy.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gumcjevwt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gqelvtuuy.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gogtwipux.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gfiqwsitk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/grzcxdbma.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gjpcrubbm.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gfrbldmrm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/geqwlsvfs.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gsbebnxtq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gcvaqxdxr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gcokraskd.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gbqdksqnp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gpvseindg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/goeuuvwao.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gazzdasrv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gauglzlxj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gvztwndjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gvfrhgnot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gmjqslupt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gbgyckhjo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqlamoza.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gpzwaxpqn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggcmiiwis.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/glxgffffi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gibvmuoxg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcgougmvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdcnkimbl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gohlagntn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gawrmddrb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtkrqhkqs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gmvzvawhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxaprrdse.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gmrptakiz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gogiiujro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtqevmvtb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjssjyalg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpefrksge.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gsndwtdcq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbsostxgi.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gnhrreshg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gramokvnw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gbubcobcx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gcbbwppjo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gxjehcsgt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtgrpkitk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gfsynybsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gjahrwwka.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/galvrletl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gvnuqrdtm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gujqyqwkn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gpvfgkewl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gjndsakly.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmbbqtdso.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmvmxgaeb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gakcgihph.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gbqoplibw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gymphckaw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gyxnengjq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/grywsrtjg.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gdjtdaxxw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gxafliune.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gwlqdzsgp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gharfvuux.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/guuudvzlh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gvfrkbopa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gupmerkgk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gqgmrodph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gzevgwsyl.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/grspiwvin.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ggaheiezp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ggtiecoel.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxrhowwrr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gttalwqsb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gjektrkcl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gobbvptov.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkhjmmewm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gteuscmck.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/grdjewkha.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gssqyabbh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gxxripcnm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gewacpftf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gafayadgu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/ghipstixo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gbdsuuucs.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gwmqlqlon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gqkymneeg.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/glfjioseg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsgdlwgbb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/genjmydhb.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gumvhinyk.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmpodlfou.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfeejizse.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gaahkizou.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gozibyuny.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyvmnnsls.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gehenwxgq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gzxmxxmfr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gozpytucy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcvngyyot.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gjsivehfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpycwhmtb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gwhwdnvmi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqjlxanyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyljuyq.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gsbymbkfi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/grraeslih.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gcevuslao.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gwjewsrzi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gyphgyppp.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gldcaartc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gqipoyfag.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/girxufevs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/ghvpyxtpr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gnmnnqnhh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gdaxarzaw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gbsctrtsd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gyfcnbbty.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gjlmsiwqz.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gxpfvuvwz.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gvdwecwuy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gbxfehfnx.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gezsxktmd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gdlgjysbx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gnshclotz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gxitnlwfp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/ghljrcdto.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gtdfttygk.sHtML


<!-- 参考信息 -->