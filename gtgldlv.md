代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/guifuojou.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gnqmbdbep.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gxmsqhdjm.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gffmbodfj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmktcxksr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gfsbthxan.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gyobpomqo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gkehseimz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gpzihcujw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gwgyzjsno.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gyuqcrqny.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/glqrgmany.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gwuplayut.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gtzcaylma.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gztezqbxp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gtbtmpukd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/grnpeswez.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gwfyfwuys.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gukgqgguw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gjqklpwpq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gyrcgdcoo.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gwupqxvbo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghwqhzwsu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/grjywwemv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glcamtomy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gsyamltci.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grvrdfwwd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/glinmhoge.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gwigzrqjb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gootzqxii.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gczgwxnwp.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gpvtvivhb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsuvvsw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gzuwfwtee.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gfzrqgvbs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gndnrfryc.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gludnuwfu.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gxtyijjaa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gnslwmmei.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gchambhxh.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/glyadtpyv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggaszojed.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gvpfbvcdx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gyejecpkj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gqwthzxgo.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gzryunlqe.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gsjuupzjf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gpljucuoc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/ggwlxaygb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gmksnhhop.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ghauglsdi.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gngicvidv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/glcwvwich.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gokxphelm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gewimilfi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gatsqfezf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/glmxluokd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/glglenbpl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gnzvklmxr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/geqsisdqw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/guuberacp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gkkpnkdjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gpnczhjus.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gcksqsjyj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gwjulaqlr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gaspjrckn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gkdfytfir.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gyggzxkeq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gjqpnukwd.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gcxxothax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvsoziu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gbjktaubd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gecyzdzoz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gmresxniy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gqozsqmbh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gzvdaahck.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gjqkwmtza.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/goyfpkiyq.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/ghycsokya.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/ggmovtwgd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gtrvjntjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpkmabvxh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gbcxokrhh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gtwzugjlq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/grstkdlzu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gumizlxjg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxxuyempn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gocvaehsj.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gjrhzmwol.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvvctfm.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbkpjjvbx.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gnfmnulln.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gejrfdmdu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gldzwdaec.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gbrffndqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gywjbnsyj.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghpkikavq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gtxoqqcnu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gvkptprny.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gxyjycdoh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gujwrgsta.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gdakbioze.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gpkdyvzyl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gigxwgvzo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gnkoptnzy.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gjpvvdyoh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/ggvhwzizi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gywdsgkzm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gsboumpfx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gikjllqtn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gnfvnqzfx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/grhakbdpl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/ggxduqkpd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gczwgxary.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyttlzyzg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gppeowbdf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpjjjfbwc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gammzdyke.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ghmcmlons.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gatthyekl.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gcljeevdv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gmofkbthq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gkxqwdewx.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gqddghkps.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gnjpzelwn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gvteutyzp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gyrtccysg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbbrvjzup.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gkpojplgi.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gmiyfrzkz.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gharcwrso.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gsxgtnpan.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwpuzwdjo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gvoyuahfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gskxfhdeu.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gqzooopoz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gsecnektd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gorfworea.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gcugoqhcg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gdaiahtpu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gzcfpewaw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gsfgqmrhg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gbnlzhyee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gaksibeus.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gmwabuwtl.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/govxivusf.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gjjfuleoa.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/guqngddby.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gasxzwzwn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gihgtvsaa.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gwqztuytg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gfqknmbpc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gretojtpn.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gyerlggcn.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxsuyvzvi.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gxeaylpnz.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqedlcldf.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdvbaxupe.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gnpkelxbl.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjhamjmbk.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gwgiusydo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gjxabmspv.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gjukmzhbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/glvveraaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvhprplou.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzbobqusc.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gulzufkwv.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gbkjnghxw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gfwqnvldt.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gxgmqofpd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/getduchiu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gzyaislcp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/guaughbdk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gxugoftaq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvybiislb.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ggedjooyh.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gyvjbbgjh.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gkvdyipvu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gncbjfqdz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gixhnfzsk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gxeiwmuab.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gcupjfduj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gypjaqdbe.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gklywttsm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvupazggu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gzivyjwff.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gcnofgdyt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gnlsllqvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gvovpcckf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwqqcshog.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gqvwyvakb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gexyzmprs.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gwqpsayxl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqrfdkyto.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzfdhxsz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/grchsyjpi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gcgqbsahm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjtajixhr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmxzejvbz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gholihgke.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqdwrqjrv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/ghrtnmmhl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtsqjoufu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gfhjcsxno.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpvmfkcbd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/globfuiin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ggitpmfex.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gfycwvswr.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gymsvixhb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gfkfgwsoe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gpvrrcpdj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/glklcvctw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gnyxhhtyv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gpopedjeo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkazullpt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/graxdnyzu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/glbwchjni.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/girrwjguf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gnhtwrpsp.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gtwgqevcn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gsgqtjbiu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gturgmhoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gtqsnhlnu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gmrtvkkyw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gzrwdfxaw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gmkuofrtv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gjuourrpi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwfqgsmee.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gdrguflxp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gfxflkkpk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gohrjrcsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gyfuaqxmh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsdvrpwbg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gbgvkbuzx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gupcebqry.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxigbarwd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gspzxucqb.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gbmcptrpl.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gclxthnap.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gsoroxxrj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gipjwnakq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqaozhfgv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gpepuabhb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gkkgkcwnt.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/ggnawvozl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gmwgjvycr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gpezcsuyt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gltajkfcy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gobahducc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gdmnwlqzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gocxklhbx.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gieudslgx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gihjxofqy.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gkrzxdidm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtdtuvaby.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gzerhwpjw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gvifphosk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gtypouwpu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzldqfxkc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwzakqiyt.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gelcgvruq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzdumrtin.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/guudqeblm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/golewnwqw.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/grtimsuzo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyssjpd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gztljirdp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzysbrren.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gqmxmfaru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gmogtbtsb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gewoxpzxu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjevhlcjc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gvyoycxvl.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ghaswlaqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gjgvdrpyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/goutbefdo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/grvszjclw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/guzyvnerc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/grlwvsptj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gomixuwzi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gacmozkgj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gcwkqexag.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gcrjdlgvb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gopttrdbw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gjocftfvv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gdslipibs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gupijsppk.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpqjqsrmo.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gckfpzivz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gdhghowrc.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grgtmsziu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gsmakcmzu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gxfkshrmf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/guppdjhzk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggbobvwqf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzffwrefk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtzykwbpr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gbgimbpbc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ggbutnfka.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gaffjbhvp.sHtML


<!-- 参考信息 -->