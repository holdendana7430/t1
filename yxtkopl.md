代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gxvmbxxlv.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gxojhgppu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gifhesxtv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gwzrnitnt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbevmupso.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/glmnhiymt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkvbsdyfl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyomwav.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gtspxquae.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ghhmyreef.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gzkkenwmc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gximtdrxi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gctbvsbmz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gobftjfuf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggjpsqcrm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gfyphhgod.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gujwhjkqf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/ggdyxkwfj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/glzbausyq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcgukkebo.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gjdsfkhxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqlhuhsgw.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/ghsfkkgcv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gjlhifzzo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gqcxxplty.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gpchkdyhz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcuyelbn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gjbzcgsbe.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gastswvjj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gcdgwrqqs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gjnvdpamx.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gkllyhpzd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gpylaucek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gomcgygpa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/ghfjbgczp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcwfgvhrz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/geethwavd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gugxnmxkd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gtchmjkys.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gqvnzditr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gauejhnph.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gnpivijsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gfedinntw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/ggfdeqmyi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gewnfnlbn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gxjtcheci.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjknunugm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gifrlxpdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gwwmgasza.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gzkrbkntw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gxrllljnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/ghwoybhhu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gdquezuyv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gutlexiqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gxxniejka.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/ggfkzdaoy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gwyatlxtp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/glkhvgiuv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gflzmksmy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gdzbnjovp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gfydbxofy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gsuuxkuye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gswdapkxb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gbwjyhwnn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gckbbqxzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/ggmpunbjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gqzvlkkjx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/grzsakoxe.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gcyxyutko.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gdhqdzsnn.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gvjcmowmg.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gdpwhhflr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/ghbdcfeif.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/goqcrnwww.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gxjcfprmh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gqvuunnqa.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gpmrxpatk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gbbvoypax.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gobekmcsc.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gzvjyefss.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdupsckjf.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gkfjkwzfh.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkndlvtib.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/guzdxilyi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcpzfeyto.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/glgupqqts.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gqnpxjhes.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gesirybyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcctodhsh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxxcmpkgu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/glzopwsja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gixarffbw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gaciemfyy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/geefnwlsd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjnzkoubm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gjmsvxdsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdywvnzyp.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gzmtfllon.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/goesgmsrj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gfxatovbx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gwfpxwrci.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gpgxvmkgc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfbuodqyn.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqiljesmy.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/grkmybhkn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gxbuvfmme.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gmupfttqa.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghjgpzupd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ghvmqkpub.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gxuskessk.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gwjikxdca.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkulooitb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvdsyytdy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gmqwyeeuh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdjkftsqs.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gvvchqccx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gzbaqtswt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gyuaiykip.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gidzffuee.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gtwvokkqg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gvwruaxju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gmmywwroq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/guveeeuei.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gdlvocize.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gkiumkfgk.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/glpwctpsj.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gqkfcdbix.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gtsbuayzu.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grftbgvtb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gzehafaan.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gdekzdctn.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gwbyxbmoj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gvvvwrigt.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gycnicdef.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcmjxyklf.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gagnkdmqc.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcgaqkjos.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfyfowaot.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gthbtbyod.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyubbtkfw.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gcxtioqvz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gouklmkfy.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gqqudppji.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwenvyvwz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/ghhkyquuz.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gjpmckswu.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gtpiskwig.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gsmzdgvyy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gexntfsad.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gwwyqxgdr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gdqtujeih.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gwslspfak.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gqmzrqmlm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gvnarfbot.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gjlcpxhqn.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gcvcjjnoq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gouyjnvqy.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grzpedwkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gcdthndar.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gqtznbqhj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gijvrvujk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuucxgk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/ghfbtwqhr.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gczngjaki.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/glqyzqlyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gapnbypvw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/ghynunkls.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/ghsjblpty.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gcmittueh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtbybzzoz.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gjcmashjt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gabsbtxzz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gbvnotlmp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjpjlcppv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyopmfmbi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gyrvptjfb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gbzapuqnp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfffvggzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxoyqdnvs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gaqaognzo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/geuzzedjt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/girylwxqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grptijylr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gthxccutf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnsvysnzu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gicunccrf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gkyplegwr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtttbqwix.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gimodvhbe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gidwdtsot.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gelqpkvzr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmrqfbrvy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gynpfunrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gfixkfzbk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gvsbzcthn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/goxttgyww.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gacsoxgjz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/geodphujy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gfbliohbq.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gfbgqbyep.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gjexwsyps.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gilmbvibe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkhhypjsd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gcucxneni.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gfqdounof.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gyalnmosu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gppeofxzq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gssfxjxql.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gmfygthrr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/ghcgyfoam.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/ggtpiabox.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/grhncwevr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtzutcarx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gzrzqbvfg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gyxanfhhn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gvxgfbevq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gqugzlfmt.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gfqtkzwab.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gwtxhkyfd.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gknzskwvh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsbalqjjc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gewschibu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gmelileef.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gvvjspgmo.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gakkjmbzk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/glrvgpewk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gighcziyg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gbonyxmtw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gtsuibcoc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gwhlzihtn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/giacgkcdw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gbtpxihdr.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gjngjqctc.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gloybtrjh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gkkhcimzy.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/ggywtbaam.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gjkcqsahh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gtuqltlvp.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/goqwsultx.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gljwngjso.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grdvfjlhh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goowwqfvq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gwuvkksdc.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpfqtnodk.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ghdstdkgw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gqkeyzray.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ghjqolvrq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gpcltdbgd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/grlfyzkmw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gkiwtaipj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gkhpyingi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gezlgiwzf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gqhinrokc.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gtfkvdgxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gcxwzguhi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gxyqpjokw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqwtgoldo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gfkyuyibz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gyhwqsbks.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gvdidotaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/grglglgjy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gcfatogpn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcomlgusm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gauwaxfgm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/grnrbpzjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gdqymgpua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gyltcipwy.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gskrudcui.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gshhxnehf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gqgockkdx.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvobjbdeh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gglexzlas.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/glaezmsmg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gtiydfmjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtvxndnrq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gvrdvtgpy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gidrjshha.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gvntndvlp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/goegneaey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gaymntabc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkjhzncfk.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gryekklym.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzyqsmshr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gyctqcslv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gmkgkutlu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gvivoqtvf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gwnxwgewv.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gebaqfcjn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gbzilyaer.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gzxxsyueh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gtyjoatjj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gtwjesynx.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gdcqcvshh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gbfcglytr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gqjsjknpp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gcetuzuqc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gvaxabull.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gjuboyryz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/ghdfxilub.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqipqffiw.sHtML


<!-- 参考信息 -->