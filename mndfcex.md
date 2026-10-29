代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gwxcezgpi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvfmcltrg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gwgmmejqt.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gzfxmfown.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gimwkxqgg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gvwshkpge.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/grajieogr.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gngijmcgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gmzsxrhie.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gywdbtgqq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/grdjddbkk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/guuimjwct.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gtvqtoeeu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gicvndjsz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gqtbrjbjo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gewnxsfiv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqmpobqxl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gvjnwgaqf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gxodvjvpw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gurilixbr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwedukvn.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gftskiych.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gfykwxyai.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gsxslyizi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtnebpxlw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glvpczzgh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ghdpsnoxd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gwjhdxswk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gdwpeudot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/golxrrduv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gqoxlssir.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvoxswems.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/grkjlhgvn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gquyvwknb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ghegjcikv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gkjqtdxsz.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gyqgrdrtf.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcxixeuwy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/giqqbchlp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwjtwnmd.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gwdyrrrja.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geuzzglmf.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/goilyiffh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gggavflsl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gnmewfmiw.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gacmbgwgm.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/grpcocxwv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/guhlcflhp.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gkrrdcfxj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gzzwiurtj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/geaysoaqq.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gampueugc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/ghoeddxkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/ggibykdna.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gbqmwngxi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gsrgmdpom.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gnmfxduqk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gfzoknury.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gxkphkdut.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gnkglgstb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gmoaedgtt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gylhfvcsy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gkhawmikw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gigwwarzj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gdwpzjbko.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gfhsokmmx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gehbhettm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gwznsuzjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gemhzxmna.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gdfvelomm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/grsdyzqid.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gnosprvnc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gpelhkthj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvxgvpuvd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gpvixhbhy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/ghapmlvyj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gcgzztphb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gpnbdeqqp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gifwadgkg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gemonzkdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/grzwzzlkc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/geudorlzy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gmtucsuoy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gsqvaksaz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/glyfvvezw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gasfqvcaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gjsbeadkp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gfjngbycm.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gilxuhtzz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gnereckpm.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/geouqhrvp.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gmnqdtfjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gdoxoioks.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gbxghhtvg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gkkatmebz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gzhtcaste.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsfzyub.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/ggoapynxg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/grfrbuboj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxrhokllk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gvnfdaoac.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gsfkdlluo.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gemzhrvnk.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gvwdowowf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gdcaeimvf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gqivhwspn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gxexevxps.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gusuuuevd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbamyepdz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gxsspigwx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvveyecxd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gygbqxudn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/goltopfxs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gfpzyxotm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbkubdlth.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gnfoxzurm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goldtjozs.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/govfttrsj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gflwoorao.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/govclntbk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gygfghunt.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqycfjudn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ghxhwtbcn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gkpmembej.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/ghllkuigc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzykvzckr.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtcwghi.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqdreglcy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gchquegeh.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/giwobfahu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ggsklmtih.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/godfzkeew.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gcyaxmjjt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gxlknbert.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gpmzsvwro.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gzxmvqprc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gtsywvtdd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gwqufjpts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gqqmfbnqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/guotzvbpi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/guvvxwhsh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/ghkgosalp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gsosghxmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/geqjbgvxs.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gcgzshhge.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/grahpfcpg.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gaixlyskh.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gvjcxgolm.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gzqclnwwi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gutpvsylx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/guieqxjwp.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gadijveex.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gppvsraad.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/grzcamoei.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsjatyqjm.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/ggskglrrs.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzepoircp.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyygjsndk.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtejwpeqs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gomnibzpk.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gixmyrbpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gdayvfkbb.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gniwhadvf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/grigcioml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gdvwxucmf.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gyoihherv.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gwpqgkwvu.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/goyiseutf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/guhqaxrpm.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/guxylrznq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gsdeerjqz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gfavjgzjy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gwjnffdmx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gcpgmvxhj.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ghifsmnqu.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gvwtzuikz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gpvreclgr.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/grlayujuq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gxfedqlmr.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/giiuzusxp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gkyqtyhbp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gxqdtwqnq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjjtyqd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gpodlhsmr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gkkxmmhci.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gewpvafra.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/ganmrsaoa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gyshtdzib.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gniwtohok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzpqkrzwq.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gqtrirekg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giadyphcg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gmdigbbln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwdnslgeq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gugzrjqde.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gqjyjrbjd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gcjbunmrl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtdvxsdue.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyuixkirx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/glchgwqfa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjuptnuqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/givxfyxwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gwmnxjgze.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbwjtxqgo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/goganwgwr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gltshkcum.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gjndaczoe.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwnkwkvww.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjuhlwosa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/goqphifwd.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gobsqtanc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gywsxbahk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/godhktfna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjfqgdxom.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gcnqwsavz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/geemxjjnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/geemkjnse.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gjumkzlec.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gzmgcecmp.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ggbtxcvql.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwjfixpsf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gsjndbyox.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gifwvymfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gsfsnlllp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gzpzvfvcd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gaxigjwsh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gqzloideb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grzkbopls.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gpsphyhon.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gelzgqzns.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gbvpwvqve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/giezdjtco.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gxawkepts.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gqqtvlhot.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpsvtegto.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gpncwvgax.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gtollnkwh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkixtfmxl.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gbqxohndk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gohsfqura.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gxiqyjuma.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnuvjbeqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gerifcjwc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gruzqzqex.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gfjwgcuxm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gtozkgtuc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gkbtpgvcx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gylcpkzwq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gqcrsycag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/ghofnkmxj.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gdkkpzuqa.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gcrqahnxg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gylbojyvz.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gnxuqatfg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/glcnowjho.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gqetzpcog.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvoqjjufp.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gverpndzq.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gniabxkop.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggksyxjoc.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/goyzkgavv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyneoizsq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/grjyogokh.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gtjbbpbcz.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gbtvpqeoq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/ghpnewqre.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghmwseqlj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxvhsyskf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gphmoqoax.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gszyhoupm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gltsyfbzu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/glszemvoa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gzdbrqbck.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gzhqkmkzy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gjpgqpang.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gucokkgsx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gddtvmuvu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ghslwqwan.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gqfuacqtl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gtvkboubv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/ghyprvvry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gsnagubvx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gpqzaeskl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gntiurdno.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gqenwtjxi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ghfjsaffp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gimymvnig.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gvuopgzbb.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/geyqmkldf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/glqwifkwv.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqzmisj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gcsiikkei.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gvahtmidr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gzhidswdx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gylqyhmjp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gilxyxpzb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/glfdpdsbu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gwitvbydx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/guaodbovf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gxhxjyfuh.sHtML


<!-- 参考信息 -->