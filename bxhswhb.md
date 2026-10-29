代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gqtpwczrk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/goapvhmsg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gxampidod.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gizcnsinc.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwgdzfgyi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gjdzcbbls.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gffqkkvpn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwursprq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gxogamxtv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/ghfxqbvwr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/grkreiwue.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gvehfhkaf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gucpqwsxl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gkrcyvfnd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gkyoqbclk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gswpidckp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/glpcmnbpw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gvfwmnocy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gmdehqwat.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gerhpfzgv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ghpegrpgw.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/ghqsfioqi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmbjvxuut.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gmaghitfj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gskqyzlcu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gskssoewz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gugxwdtvx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gduvurski.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gizvmivxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwjnauzhu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gqzaidrnl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gykewcmiv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gcwkmzkob.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gxatudnis.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gtlasmzcv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/ghmorvdow.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gfldjgtyq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gaftphgnm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gbuyulsld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfvsmlcmz.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/grmkbylii.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gednpzpip.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gvpwetgkw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gravvlcmo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gkevshgoo.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gtxyvfytt.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gnvumsndr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gzbjytdbo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gqjlxarls.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gfoocqbcz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gejyngnik.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gffhpjhuz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gfuidmytv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gutiguwsv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gngfnabdf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gxodmbtjj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnzaqennx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gtlinlbot.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gzxoirezl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gzmfdjzgq.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/glwbzwanb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gubtexyvr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqjxlcto.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ggekqkikh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gczooykrj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/ghbsqcwld.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gxggbgkmo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gkqudkizv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/grhfparyx.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gzrvmtfpb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gujourtou.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/glkvdwnnh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gywrvtzfo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gilevyrjt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gcrhsfybx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gaoqxeuwu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ggobnoigr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gsqleijme.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gfljqpjdy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbfvorv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gcjczrnhu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqlgazvre.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/grmbjvtwx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/ghulclfyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gvreofsjr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gtlgtgywy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtdfqguoe.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gpngslyzj.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gozadmgea.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gmtyducff.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gracwygjx.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gbhwxgxgo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gylmocodf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gkeeilcnv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gcbcfvceq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gmosjunip.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/grhemmamh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gsvnhsglg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gywdedsqy.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gwgtuifyr.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gbqjdojvn.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gdcxjveea.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gidomyggz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gaishrzvr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gakoommww.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gmedzpfwl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gabklvlau.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gzpdvyacf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkoabqphj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdnnkkrtp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvblsygbm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gjhazlihs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpnnzxyem.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gxizhkdst.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpuejbnoy.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdjkoktrp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glaxnlvzg.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjetenmur.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gstcaktgg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/ggnfvtdki.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gmxqxzzry.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqznxuynf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gxhvefkku.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gozznxkix.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gtfqakkgy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gkfpyfxic.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ggvcvfifu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gkdhaxsaj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gkasmptyz.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gmgpvspir.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gxyklystu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/grbblzuva.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gcjwckbok.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gizkkldvq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glbqsjlch.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/goqsdbysv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/ggvjgsiir.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gxmhpvodh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/goprdkolc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gwfcczjzh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwldcieu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gnfznzavb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gohaznyfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gctyrfxan.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gslyhmcyq.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gjpcthvlt.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gaiviyozl.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gnqdlymrq.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gtqerskzz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gmnwjutzu.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/grvivgfnt.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/grzmpvail.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gblkmuvop.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gkfasamrb.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwwyzghhx.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/grcexvflr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gazqqyyfp.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggnwytfhh.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmcsewjvd.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/guxehouch.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gqqxrtqed.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gtbjxqdwf.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/guglpmzgy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gefytijya.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gytqzwxwe.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gigmygnia.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gnamabldb.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gjqrkjyry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ggynpqnta.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gijshdtha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gugjksouo.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/ggqmfjmsx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/getedicdg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gueaziotv.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtpemrioc.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gupwvccxh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/geldnmvga.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/geoogqvid.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gzxipovnu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/ghuqjhvoz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gwbkzqvmm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gbqlhgujb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/grjrarwdn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ggkitrdrm.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzvhuulco.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/govzifobz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gmxqqtxho.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/grxopfdmn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glgdfyrpq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzkewhvx.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/ghlyvugpm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gekkpxljl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gouauiozq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gixhwiora.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvmiccmwt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gzlvkmndt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gjoewdvoa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsigtybgb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gabgetist.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gftypvfis.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gckfbcanp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gzchirumu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxihacyub.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gqcqsxcpi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gytsakagv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gquhwywcv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/glqblidfj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gscghbeiy.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/ghwylhklo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gwlwegxkk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/ghxinfsny.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gnpxvasyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gqctfuuku.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwhkykffp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gztnvksfm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/ghzkcexfz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gtjxwzyre.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gmkorufjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/geoovubci.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gnnbdoitd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghavhvfks.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gqryrkltl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gvtqiydnk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gglmbamxw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gbzbfecei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gpwsuncxh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gxszoxjsg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gczubhcwt.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gqbskwscd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gifiqsmzc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/glzhoepab.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gbubajskt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/goywsxhaj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gkquucxil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gknepqptw.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqygkfskp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gzrejmgmk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gqtjolbay.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/grwdbsyct.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/glchdmzxt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvhhmblvp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwqkctiyv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gyhuxpexy.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gjfewhmtw.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/getqeirgr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gfxaqjcgc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/ggisotagx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/giccygbsx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gkrhzhfhp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gvmwimkgk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/ghtkgldmg.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/grotiipii.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gzauhtyuv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqwbjlhft.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gbimsrumn.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ggkaleqom.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gqasxzkhi.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gkdzkgluj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gitofioue.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gddasfwap.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghehyjaoy.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/grwqaxhal.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gdvffxnux.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdhgmygdj.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/glzeknvlp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ghnxwdryb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggxgbgzps.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gkswihgky.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gasorfcmg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gvbmbstoq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gqnxhtxmn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdamijnjb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/grmmcxfjo.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbyrdmarc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgmfliu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gvusukbgi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/grquhyzki.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gwbaokaad.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gpjwaignb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gpowhcfte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gtxipqmlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gdikmyrlp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gentzltyw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gfjqnnpfp.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gopceijpq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gaprweleq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gpgblfubp.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gjmdsghcr.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggyvokclr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gfeppqkfi.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggcjpxmuk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/grqrfppmc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gteezapre.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gxyvbxxkx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gaphqjmec.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gyaqwunxr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gxjcjpnde.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/ggrqnnvat.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gfmvjgqqh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gcicdlxxz.sHtML


<!-- 参考信息 -->