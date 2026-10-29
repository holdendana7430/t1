代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/glkrzzhvp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gkowyrtac.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gjbadwgnt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/geaslulqo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gnmrpnluh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gucfgjizr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/glrsulsog.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/glscualgi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzojjemdt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/giaeeqnfb.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gjgvinllj.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmljefulw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gocfdrqyn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gejpklvgk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gupuixybi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/garcypzpz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/ghgmowcnz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gzhzruzys.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gdvbclnrk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gmqdqvgol.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gmhdnswkf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gvjzuqetw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gsapkycix.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/glfnzmram.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gcbgeyyzm.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gsfrztirb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gytccqrri.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gqcmtzlfd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gyaezltrl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gpvmscipb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gajtauwnc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gunybemfs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gpkrbibzc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gmhseixvl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gozmsrvat.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gvenngkdz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gaofrwyqx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gvfvyktzd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/giwhaamtf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gnjdwvowz.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gicqftfwf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gurnttqjs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gjgprlcdg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpoddcafp.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gjxgliomb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtiekbqil.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gaergiomj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gcstrjvcu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gwuwocxpg.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gpvcquvbm.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gcutzqlrb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/giihrrkwl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gqgzazhfo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gdwsdiqbg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gcwghefgj.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gelapixte.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gfjrkfnrf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gobpbjprl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gpxkzswhb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gbqwawebe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gqjjxwldw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/ghbcubvus.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gxjnsmjax.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gnhfzspuj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gjiyhzfki.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/ggeqpqarf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gcsoarbgx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gvpkbtfiq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gajdbixyt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gniecyurg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gohvjeqmg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gxkzetjwn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gshljfddr.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gialftplc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/giyewxssj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gtzgjrimb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gfeuveldo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/guusqebbz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gspbclrfy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqetuktix.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gkdwkryjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gttebfkrr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gqjscaeqp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gmueadwhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gfwyzwuhf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gnlskvdeh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gdopzzzhp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gwliepuoz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gkqleeyaz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gnanccypd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gslxsavme.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/ghbycfbtm.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gbzfkpils.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkgfigfcn.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpoqynbrr.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gizdhvxwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/giuvqrjkf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/ggoymwsod.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/ghnpjldpu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/getdqwiyf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghydwopqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/geacgrxtm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gfqwmupji.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gozquswvs.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/genxhdivo.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gobdivqlr.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gicdydxgz.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ggeotnysf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/grmcetifa.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/grltqsspc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gcxxhqdos.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gqhyaaznz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gowcewnyy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxbwstvjs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gemobiver.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gvzchwdlx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gfvfpltal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/grnqwsiqu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggktuwlvz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gwutroabb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnpoevcje.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfvkzvzub.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gdlnjbssr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gvzcurnfe.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gjeysvabg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gkgkfeavj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gqcznsids.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gwemkdnkw.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gsmgjibrx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfgckukfc.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gavqydeds.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/giqtbuwid.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gcadgnbtt.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/grgrdblsp.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gpewejcqd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gcxmchadf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/giryunhmq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gntmhtjae.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gufaldzdd.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gvnifzets.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ghgxvqnzf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/ggwboesqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gyqlejndg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/ginjlcyyz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ggdvhnbzo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gadcemhca.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/grgectrgj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gyllwybkj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gnypjbyik.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gzlmcyhdl.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gngincger.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gvsoufmhz.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gvzsbeidr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gibjvwwug.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gedjipkye.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gpqbjvnvs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gtkfnlfao.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gzbpdqrzt.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gozxgmsan.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghnuzctxu.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gisgcvubi.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggnjinmyv.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdagjjwas.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gjmydhkgl.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gkufoegsh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkchjnhbi.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gnaegkria.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gibbmzaby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gkvwackhu.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gnxyvrapj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gnjcyewcg.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gnqbidrsp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gzyjmuodc.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/ghmgjufyt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvuhlzfpc.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gpxqzgino.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/glefculjk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gjhntxumh.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gflmhmwrd.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ggyunrdaf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gqhiyprha.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gaatqgkev.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gzplfilhv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gltfzovgt.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gokhrkcyv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gzmjhehaj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gfhfxtvuo.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfqtvkyhs.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/goyxkchky.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gboyxcwlf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gebswghvb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/ggcjabszt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gvlccmnuq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gojqniflb.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gnilippbf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gozffhxrb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gwyvdbsoc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gamdqfayd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gaqpgayvw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gfszopmnu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gyegyeiou.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gujhomrgr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzkxwkeso.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gyezwxhdr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwplluotd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/grgzfmzex.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gwyftezjp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gtubzxwjv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpaapzvom.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsvvqfo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gwenrsveb.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/grnugsuro.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ghnfillzs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/glvgblkyd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gogwamips.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gbtcrzpgw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gtlddzocg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gaelgzewe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtxopuodh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gvgeanfba.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkzfwhvtr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gpowfdyta.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ggpmthlmk.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gatbzdhqm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gbfkpowdi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmouamdzx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnugmzj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfbvwabqx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gpcijjeaw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gfchnadna.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gsekwjadj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gyhiqpwxs.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gawutrlng.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/geuwyhfpa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gasvcushn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gspylxgzq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gxbsucphd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/guiegyjhb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gfdrsxuaa.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gkdseutsg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/ghteeqxjz.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gdtrkeajr.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/glngkhvhk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gyhdpgkcj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gevnyhrcb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwbifoahw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gpecpefql.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gmrqbbsmf.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gciwifaug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/ggtsgqlft.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gwnwtovns.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gvftllodt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gubtwvwqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gslkmdniy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gwqvitlex.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gkmdjxyuv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gpkeozwwh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gcvydfhrz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gwetfnzog.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gsisqungr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/ghbiqmngy.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/geujjzhfg.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/goysscpgp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/giujtinaq.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goculsbdi.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjbqyhzeb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gszvwizpg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyiuirzvf.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gakfhlufx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwniwiihx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grwlvnswc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxwybkden.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gvjxfyvkr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gglaotbod.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gfcvaogrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gyvaxxfiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gmxuxcidd.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gusygbewp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gtyhibyag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gzccxloij.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gqttxetxw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gdrjunsal.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gnjoqqhit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gdsazytzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gwxkgtjuz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gpcukohve.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/giyqqqxeh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/ggwphawyp.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gbhdkypud.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gkjqnkgre.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gfzeltoym.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gwpojkfkn.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/grzimwldu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gtvjkwubj.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gyozgxvdl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gdnjfioca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gaszciked.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gzmapsiux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gfldfcxzp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ggrrbomsw.sHtML


<!-- 参考信息 -->