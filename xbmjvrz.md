代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ggbfjxnvu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gxmlkecli.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gfqsdkzeo.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/grzqoolyx.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gvftsgrgu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gchoanuik.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guysijgui.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gujewqaxv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gqrdocmzs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gsgdtewkt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ggpnebkzu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gzoboqlhy.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gfbhwkrel.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gnvyyyyzp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gzgvjozmd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gknivlwja.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gulgitmsl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gsfloepjs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzxdconvp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gmojpbuxc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grrgbpkce.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gzpvwrkey.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwawuhoux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gikttoets.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gezrimhhi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnaiwczqk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/giezhfeih.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gpmdfwdxq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggibimlon.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gsqmgcvvm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gcteutbri.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gupzsyhjf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gohhskaov.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gbwsqtidn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gqnmwoxsm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gogeeajlt.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gjegqmiql.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gajwpbdfn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gqlgxmhbn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwqtpjbms.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/garhrqugq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkyqpqwzw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gkrgyoiub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gfwpvlhdb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gdgpllllo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gxzagezmp.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gcdoxpxmj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gpzegpbpo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbxkkfmao.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gyaptojqg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/ghgetkipu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gvzapfbki.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gslzvhkgv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/grejwdmkn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/glvbhpnsl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gappczoad.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gsruxzhsa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gbhkpzizt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gerwfsqxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gpvktyzxp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gtfcxlduz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gzcqecjqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/glhvzxygz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gulypmwqe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gbmiveuph.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/grntjatqa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvktuejqf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gfxfxbgmf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gmiageqzi.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gkyvimflh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gkapbzfcl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gdxytdzpl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gnfkpbgws.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gihevrzpg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmwejvphz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gjcahjmxh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gfmgzqdnz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gokespnjf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gbphgmihx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/grxolmrza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gqifdnowx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gwblhmpii.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gzdtzlydo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/grkfmmzkr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gforukvga.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gcrzjrbnb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghsaqijuk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gkxjjxfhy.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gqavlrido.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnubldfgq.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ghwbaludi.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gimcfuhzq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/ghrkaxaav.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gzjphehex.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gjeuashyz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gshbekasf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gghwhiukw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gnevxaens.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/glnhcoazy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gagtddivm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gywpjlhdd.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gxvhjhoin.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gizvrdnej.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gpnekdsbx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gwcpqejrl.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/ggnpcsbgh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gooeumxeh.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gmyqpvmpc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gzyjljjlh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/giexiuktx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gmhvjbhbd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gokqiumnn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxybgrlgw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gkzfsgzng.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsyqbuzpt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gtktwmpvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grbsqstfd.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/grxuwssna.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gwdkahcli.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gtmbtixgr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gsvnakktf.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gymihyxnt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ghkcwuhym.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gbzomadex.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/guwuufhjt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gmklpbxhz.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gxodlxdky.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghrcmrtpb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gpgofecpe.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gfgothwzk.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggfzsrcqr.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gdsitpnhu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gcgshljui.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gykcneytk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmorcucfa.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/glsjwdslj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gmcnutyfm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gadxankps.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gbnihpyem.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gcvfefqtt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/guximitfn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/glrbnehyx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gnwwaabdd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gbnuuwlby.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gtliwbayq.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/ggjszqpvz.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gtnziwegt.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/geksbqllq.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gbrrerzlu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gharcakaq.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gkuarwkjw.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gfvrkcpvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gfkowrhao.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/goqvxxnjp.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpzsltupy.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gryehfdbb.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gevdzqwko.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpoydqvxa.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/goqrrvivj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbulgqob.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gzrrjqguj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gnaiserll.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gpuxcsdvx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ggsznthfd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gfsaokduy.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gxvnwphbl.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gslpvenad.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gpgjyevbd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/guzgivuim.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gtfrzezax.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gidqtpssf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gsxwuooey.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gucldcshu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/grhjqspio.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gixjbenwe.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gdoqvyppq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gltenadps.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gyrzjdxyr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gfrjoakmg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gbbzfloez.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gmqeslkzt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gojxygmew.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ggpvkjzis.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gwgambbpq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gifvjjxkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ggohhfuwt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gfxxjbvso.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ghepmzitr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gpdxxwabo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbenclvwf.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gokjidcuf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtbgvumws.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/ggtaornrv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjciavtry.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gbqxraztn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/goetgrsch.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gfgfklssk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmvfoqjvf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxiiiieqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gsqngqblx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbcxkpmvf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gwimnelzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gyfgdwcaj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gnxkndbki.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnfwgmoxj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gvrfijalb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gbcpwacwr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gadivdtsu.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ghwkphphv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gexsrfxnr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gchkodlyx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gmbvsnnwt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gbypksolu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gxzriadpt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gsyppghma.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gtoujpmqt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gjkwslvwg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/ggrouotti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gsteghqfu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gsjeaqngj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gabgwtmqx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqozyhspv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwyysghbl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/guneabqvw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gopttlvpv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gzdbrhrle.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/govuwopyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnykwemgy.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gfyttumab.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gbykvvbev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gfeljpudb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gucfekufv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gazjayjsi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gcvgwbjoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gftddhwti.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gwjncidqc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/ggnzztvip.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gxpeqaxpa.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gwnthgzxz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ginvepakr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdbhizfem.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gaggcqalr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gdndhbyrh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gjwjkasib.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ggilfggrn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gswzkzjvc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gotlhehep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gnkvhtxpa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnbfwei.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gwwldhngf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/glwukjeoh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ggywsyuhx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/giaqnhejb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gkgaklgjy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/ggrqwedlo.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gcgsnttyt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsnemyxhp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gblirbtts.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnyxmpvll.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/guuiopqig.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsybfejjo.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtglkbxit.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/ghcteoksi.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqhlcbzls.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gtlzrpbsr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gaigzpgqs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtwfcognn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/giittsgnq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gxtylhhlh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gkttxzjbg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gnlgmqtgw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwxvqnvyq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/ghubqomqj.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gopdnprxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gwokeiqnp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ghcwqhynm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gkwhwfhdb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gtbvfeums.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gluwswnan.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gshhzdpyv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gqvnwdqah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzvcxvr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gxlmszwhv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gzddnquam.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/glipqzpfo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gwqjliikc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdpadxpmk.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gpjkwnxkn.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/giivuytcr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/grxiqsnhg.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glmyvflap.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/glqhwyput.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gmqtgbuit.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gjcwzthae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtstpmlny.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gjnklekpo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gxxmjyabt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gttbrrvmw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/guxiixkqq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwnzwdxcj.sHtML


<!-- 参考信息 -->