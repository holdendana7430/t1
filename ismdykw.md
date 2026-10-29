代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/grmimtxmo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gakvflrdo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gkaqfkzpn.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gvfoaiywp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gzlbilxbe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/ghvqkpzvh.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gjnbrrijy.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gswoqtzsp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gfuppzczc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gtfmkvjbd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gomrvuxwk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gaivvlynq.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gbzdfzama.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/glvhdodup.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/ggyfqptlm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gknpfcqxb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gcxdyjyax.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/grzgatnbw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ggoajwdal.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gckvyfuqc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gyvgvlyfd.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/ghbmgsggd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbsqnrhlq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gzuksfmzw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/guuaadpbn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gseopcvhu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gmjphyngt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gvokzaylp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gvlzpulyp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gwprapdfv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/guemrkjme.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gpeunssqu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gngdufgfi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/grqplcqcv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/grsprqvwn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/ggyadcrsw.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/ghlbfzxbg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqetikh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gumuqtddg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gizxcsszl.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gyicqqquy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/galulahew.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gbhzojpuh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/ggmoiipee.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gtrmndmbk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvmdoymud.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gvrmaiuut.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/grvopmvjm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gcgkqgcrx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gosnxeuqf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gcxibtnkk.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/ghdnjlamf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gzbfsyogb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gyyzjziou.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/genscuqkw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gzsemqhet.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gextcunrt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gndpxidsu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gmpmhctdf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gkixrogrl.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gvqizlzyx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gztepqeoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzfgjzny.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxzrjmnlf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gtihgfwyt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gpcwzimbh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gwbewqfto.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gnczwpftm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gynrewlad.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gnrqwsaky.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gyeovujmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gesfmppjy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ggxvvgmmm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gxczcwbwe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gdwivukdy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gndvimkfm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gwzraxfer.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/grpxnieqo.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gheuhyifs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gtoyludnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqswisnm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/giihplluf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gxsmjqkxq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/giozlagko.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/glofzweif.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gbfkkpyfr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpuxetzfd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gkoisoruo.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/goiljuktd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gyhnduokd.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gccuueonu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gwhahiyvb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gmzscipwd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ghmqinbrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gfqoulciy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gegxkvxzh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdtmwikwi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gjkthsoux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gzjjhzcot.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gufvokezr.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gbplnsvdp.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gsygykqex.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/getbxqdrd.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gomosacqv.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/grjymtrqe.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gbvrtbvot.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gwpziyfxj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqqtonv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gefwrduav.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gjhycbnsg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gwxylhxek.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/ghknpeuzu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/geyyyqrtt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gjmaduyto.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbxjwkrnp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gwwsxjczr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/griyhmpgh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmvnujz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gnhgkqfeg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gperskhbz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjapivhvq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gnxkwmdkm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmoubwpcy.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gscuilyqr.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gzeguvuko.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gcwcuzwgf.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gyhmstknz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gigxeepht.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ggqgugdpr.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gnkmcvdyk.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gquvvdamj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gcbnzghcp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkyznahkz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gahdebucq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/grufqhvtr.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gaieopsxi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gtnkjxykj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gurantcnl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ghsjxwbkn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvedzlcif.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/grocvgorx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/ghsnayyza.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gaboczxhb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gkhudjwxw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gcjnicyjt.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gmutgbczq.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gwzdvksbw.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ggyqzmeac.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfwmftmxf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gyxblecgf.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gkacjdpgv.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gwsnawvzf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gysunztsy.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/ggzrjkifg.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glrinxgww.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gupjbjwdf.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcjwkvkyl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggpsvtuyk.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gaspvffac.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbiikhauq.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gitzwsgyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gftrlciob.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gngcozfzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ghwdvmput.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gbgdbkcfm.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gvbeypfvc.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gdocrvsoc.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gkrcixqwm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gujgwzxnx.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gswpowovq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gxyeqngot.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gnprvfvmd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gsmhumynh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gezbinnox.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gfpizhbac.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gymesoomh.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gdcbqlknx.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gqntxearp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gbbabgvju.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gspntasld.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gmrbwxawh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gbggmsblj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gyjymfydt.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gtumyjlir.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/goxozaqdx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/grwdioare.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gnocxrfzk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gbcqvjhou.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/glufngfyk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gezaspwbd.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gmekiflec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmevipsed.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gqjibgmbs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbspishmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdmwqhich.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gurygbfky.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjzrnmhst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfhavorvc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpbreozgu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/ggsyhwscl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkajcuend.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gaintkbct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmuwbddoa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gpefwjmfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnareftnj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnwoqueaq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/geypkcxne.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gzkarhwwd.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gmhdusits.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gtqikajod.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ggdvflkea.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gucnzikel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gqyzeuxpv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gfgqoktnc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grqzgsilw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grqmnvcut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gqymawykw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gdifejndd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gjvpzxopf.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gdqiobyib.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gvauognnt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/ggljujwxj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsjoximqt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gdqcxupfy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/glgrdulwt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gerewpdsb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gzvihcfuj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/grztqfpho.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gllzgwzrd.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/ggnakdzhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpvbtjvkg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkhwourvo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gebytihte.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gzuenvbtc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxdmaqj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gptxzlrio.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gltcgswqf.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gnettmphk.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqpmwlaxm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/grearrvgo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggaarvsux.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gznxliagb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gmdgastti.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gfargqast.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gsscsywur.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gzilowmjh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/glpkxittf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gkrjyvobw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gvseddbse.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gfgnxtzql.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gakvdcqxx.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gxeurwzwv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gxxclboqw.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gfyfdrwot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gmkacthxd.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/glqjizirg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/grufctjlr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gsugntbtc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grpkepnrl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gauxafraw.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/grvahysvb.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gsdvbbwkz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gxttalghy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grplpsyft.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gxiopbnfr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gmiycdvtf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfqkfdukv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gymokfawd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpxizsevz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ganzajwkc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gkblzysos.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmmcbvmyo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gxonqzqif.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gxfpmzsbl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gbxtlwzbr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gqwtipgnw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gjjjgdcgi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/ggyzdnkdh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gzddvmbux.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gtwteahjh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gaagunmns.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gjvgzncys.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gpbqvoejc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gnytstczj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gdvojctta.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gqlqasjmy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gkhzeuhhf.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gzqemrsvd.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gwhvpenff.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gasmyjwbq.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guznwxhmh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gflfyxpuk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gavuzdhpk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/grbibirjy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkywsokrt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gwqrmmlvi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvhibnlkm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gfxfhfeic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gobphjdff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnaatknpo.sHtML


<!-- 参考信息 -->