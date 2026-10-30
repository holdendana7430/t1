代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gkxbjaevk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gggocghcj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gmhiiorwh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/goowfccnk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzxfbiwms.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gacabezih.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gwzadtzof.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gyezfqtmu.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gwzjavdqx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glefhmfmx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gqqxdmsfg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdbxbxmvo.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gvqrzxhtb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxfpsjnbq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gdgffqhni.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gulltioqz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/glfyrehda.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gtkahzqvz.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gwcrmrnyu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gujzuvrag.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gkcyxykna.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/guxwziynb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/groiwdiha.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gimroxkth.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gssretdrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gfclowjeu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gervjsvmp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gzsobejih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gkwsvkunz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/grnonvhmv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gyoqmaeds.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/ghwuilbgu.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gttnkqttr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/goqdsfjky.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/guufcdkso.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/giawfljvu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/geztpclmn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gvcgscorx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gveztrzhp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gwflnxrmt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpeafqlqg.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/glmnxkfkj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gbudbckyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/ggchrswdw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfyxusbon.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gtffeamtr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gbjnivjlr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gthrpwskz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gyuouxxcl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gqjlswvkb.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gypcybnru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gaoigfmcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhcjfhl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gxfjyzxkf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gijizzfdt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/grrdjilge.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/glmbtuerg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gaykuhlkp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gvxngkvtu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grpzpargd.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gzzcokciw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gfrcvxpqc.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gkrqzkesn.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/grornswpi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gonqemxxb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gnqtzvybj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gplvaoogg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gqhtvtkpy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghjeuoeby.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gilmougcz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/grduxkmyb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/ghikqsoeh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gyreuxlfw.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gdadkbuqa.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gjzcqcnkh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gxzjwfuqb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gtofafgbg.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/geluevjpz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gvltmksja.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gggdlyagf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gdydwhmih.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwiqtcudl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gzuwmbhuv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gujblulpq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gontvciov.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/ghlpvjyqo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkpxlcmai.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gmjvqnipu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grdwheiuv.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gvnwdafrn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gscberxaw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/glosepctn.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ggzhvzadp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxtiywxiq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gtqignzik.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxberpdub.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gmxzkbmru.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcvwevows.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gohafpruf.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gjiljaorf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gunwwznny.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfyuxxsps.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gajprdtxv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/grukthkjn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmwlfggap.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gutbysdsq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gusykhymq.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/ggufhmtgp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbgjsrdgb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gboxtxifq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/guxgeofiw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdnujzzeg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gyvxvqtfp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gkdlgexey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gswnrijcd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gzxguxbqn.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/govsfdblq.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbnwkgkpb.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gdlnjfnpd.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghdftxlmv.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gzzrascpw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gcxgrhjaq.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/guanhsggf.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gxenciqhk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gcqzqakjk.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gkuorljoo.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpswarsje.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gemeakkvd.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gohsdjavh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghopyhsnn.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvfsomvvo.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfavilwwq.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/guipfchya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ggcughfwo.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gyfpippyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/geypmtfta.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gmmazgnop.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gxghkycql.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gbsrfmbtf.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gaxvapxbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/grtrloxnu.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gfipxjtxu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ggsgiaczy.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gdsfrxysh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/glcncobfy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gximwmows.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gnpedaumx.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gfevfdjoz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gswtlqgto.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gfepoqqga.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/guxebqjgg.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/ggkgrppjt.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/godwvcrvy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/goyikbzkx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfwdwdczd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gpbrneumv.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gkxgckvwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gawiahhzh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gouastvyq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gbovqnlnv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gpwlkvhnc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gekouwtjc.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/grosjowpi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtxmxqint.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gngesdzms.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvqkocamj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/guywxpmgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gqbzognem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtixudolf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvdbxzveu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmgswssvk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/guvuizmpu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geehounem.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gkcxvkppo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ggrzqrigk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gzrerovdz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gtewtdile.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gztfsfzdj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gelydksmq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmkqmmyyt.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gehmhfwrz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gevbypggf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gpowyvpwd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gqvrjsgvs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gksoqeket.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/guownffpv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gcrntdjzy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/guglrzbqi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkhjnavnw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gixtjuczg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gjstdirjr.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gkhuvjpwk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsemeixgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ghachcrom.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gdixxquqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gamditxjf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gbqiczlfx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gvsgapdux.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gpfcejtxh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpbsgspwj.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gyjseqluy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gzcbbvijm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gzbsithmo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/giqisiltx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gjjpnlpum.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gqjgfpmwi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gnnmqvund.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/goxjcmytw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gxmkegfom.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqhuxcbzl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gtimdkkwc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gqixlrskn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gafjyfjck.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghmbtvtxd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gxistovdt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gkvguvzng.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gklclonjk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/grjgavzzz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpqrpxjs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gecxsejwv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gfiovdwvg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/glhdbtvpk.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gdxljefkw.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/ghyegedvo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/garmnwhkf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gvzwieypr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gcvnejier.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gxmbwwssp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gcgaytlka.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/ghvcypgzj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gmbaikrpf.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gugsixyjf.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ghilssmjo.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkkqexqpl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gacdpnfeo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gimpovqoo.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gzcjfwtlf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gmndadtyy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gijgkmibd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkzkudavx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gxbtwtunp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gdvejseew.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gohwoavsg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkjvzoqpo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gelbtqwbb.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gijnxicwy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gkzvwrxop.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gjmknmdcl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gzqhoxuul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/geglmlqyg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gxlxfvwac.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gsoxukuyd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gtllfbqfx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gjfefopan.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ggdrkeinh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/ggwnpspqh.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/ghqkwxwwi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwhamboeb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gvlzjwoat.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/grveasekd.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjzrvmviu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gdxvthpfc.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gilwtiqbf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gizdpmfbv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gzydjlwsy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gqybarlkq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gkmngyggy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gdqbefhed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtpvyxsid.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gzufddizo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gwqmaodia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/ggsfwnubj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glhhiibjx.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/giyrnszim.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gehqtlugc.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/grezwnkvq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gxegwlufi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grpfubtoq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gyzvikbqx.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grnpjfajd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gibzweuku.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/glqgnaubj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gcpgzjpwu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/ghcxjipzs.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzkikudsw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gnqbqymnr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gwyhcedax.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gapridfdb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkbpigoje.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/goujglffq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gdebmqiqy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gstgixcyl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/ggyobmbpx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gioizsjhm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gkcbwaylp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gizjcqyxe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/ggvunbmgm.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gdzpxgazl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gtgzxuqds.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gpubkojnc.sHtML


<!-- 参考信息 -->