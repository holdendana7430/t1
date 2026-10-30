代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/ggketfxrh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gjjniezkl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gttbjjksc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gyjkbqhyo.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gwlzmzfqo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gomupgqnl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gdpsxjopq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gclvxdevt.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gctzjuspt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtoqrwufa.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gimosiiha.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gfeuzosbs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gzuwcqrni.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gaxdyqmgt.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gdxnxhxbr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gmcubjtvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gwszziwbs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gzspvgkwb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gdnntosxt.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gvtnkbtwc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gqlxtqfyb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/grhfgrouw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvckbpwil.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gtmkoirla.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/ggfiabfjf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gpgjimqov.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gdwillhsj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gymfimafc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gzfebwzay.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gopchourv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gzvdhudui.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gwshhbmyx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gyoobwlcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gzqbspqyb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gmqgtfemy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gvyisrtrn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gdqibavwv.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/giolzxrwx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gwpivaqva.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gztigujlw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcidolgcd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmluzeoqs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gpjoqnboi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gdgnnvsnc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gkjucccij.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/guauwxwwx.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gvnswoanv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gupsjzmmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gnkhkpdht.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gerebqsfl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gguzbfrgq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gueeumlbk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gwuvojiwo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gqdaodzjc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwkbvmxrc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gktkwkvfm.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/ggtkoiyut.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gekjtjnyv.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gubaaawvn.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/grkvxfxoq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gubwstnrk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzjmyvg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gmudhppxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gzcjnfeaa.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gckmrxozn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gfjkvcjil.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gbqrcnfan.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gguwxmwnm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gcelilydy.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grwzjrayc.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gjpbubxmj.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gsbqaobdi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gclmlfsth.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gjcbfzyec.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gzscqwolv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuzklbj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmcogvgst.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnupydtec.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gjvfswtpa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gohweyioi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gparnziuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpttdfd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gglxycyiv.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gxpcpxpsp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxhgyzpcy.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gqnreezox.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gcgohdgpg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gwmwsxxnr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grfipmozr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gntkoyyhf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gsclgndiz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/ghgrbgmfv.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gbgqrooaw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gyeztefhp.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/girvcvcei.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glmsvuybs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/giwnivrke.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/guhawcwei.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjgtxncbw.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/geaoyjhak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gpyovtogz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gapivriaj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gjcyxftbp.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gzrdyprbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gkjblfdtz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gckngpqdr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqbyjdoqo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfyfxiqzl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gxqdpbdjk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gtsqqdzqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ggumqdrpc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gtasszqby.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gasezintx.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gehluazpy.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gfmglkivb.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gjjxltjcv.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkzrgjcbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gevhyfujz.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gvwxllffu.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/galerebii.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gejmlzdqu.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvhnmuo.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggblpqpnh.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gcimytjss.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggjjjttpd.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmzqegjvn.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/grrqglejq.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpjrcnkcx.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghcavdtsf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/ghbctzqjm.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gjzafzhby.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gkkphzisf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gishkecql.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/grrhakfez.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gksqwyhfm.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/glipguebo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/ggtbhhjwb.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gyehbfojd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gzxrsvqdd.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/glqrzacrq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gzfpzzbkb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gpqkdptfc.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/ghajvklsd.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gjnprpwzw.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gtngypetr.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gwdtoliwm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gthexyrir.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gsrrtcmvp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gtolrwyto.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gizufjsdx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gabxurtbk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gzwqelnog.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gehsvmagi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gxdkizskm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gfhsipymr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gpovecogq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gttavzcsd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrpzbqfh.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ghblingnv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnfhmfqfb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gtbhxpzae.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvyelxubf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gtjkugpir.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gutnnqcoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/goaucrwsk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/goivtvude.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grqfrpwxp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gzcrtfofw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gauwlunpq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gwchyyvba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gqouhxrzw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gpajynbem.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkspmdzrd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gmnjmzrrh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gzfenqvbd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gndbipccf.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gxpldvjgc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gtafadtao.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gwykfnnuh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gufitfrlb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gqkzuyxqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gxqaltmel.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gouwsfkdo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gpypggevx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gxxinktqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gnnxhalhs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gqmkwlbzu.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gppduufdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxbekcmxw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbvwvtt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdbxcdmlr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glarirshh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gofwmhsre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gyxwriehj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gmjotoouq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gbbxbbzkk.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/grputvkfk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfjnpjyfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdntajtin.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnptoedkp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpbhpnrjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gjddobjnm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gtxjpasog.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gczshjxim.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gkuuztbrb.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gjjwvaggk.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gvnmlqons.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/ghkhwtzox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gktcnnyjl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gjeamwzbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gwcajxfgw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/grozrpios.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gvmanyddd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/ggnvzvqcp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gxovearfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gquoitgeg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/grvsafqxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/guxjdsljn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gahanlxby.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gnsnkuasu.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gtepkjgwf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gnqmwcvrv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/guaxzgtpi.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gqazogmwy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gvvpsrllz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gnxebmeut.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjbarxdqm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/givpsxdll.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzkqoasoj.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghuqhoifx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/ghqiylilq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giporgjem.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gdluubumy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gjzhvnzbh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdqptbojy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvbzbtwmn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gezobwfdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gaukeuxkp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzsoevlbg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbndajzzq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gaqduiiln.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gymqfexbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gbbarxuwe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gbonaqdez.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gpgmgddym.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gxkkmmokj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gjpclehpu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gzqsnqwfm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/grcsadvwp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gpwvmgcxf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdjfrccxa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gixyzxynd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gvxcnanga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvnknjyhr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gnrxkgarq.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/glgxazmze.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gywdwtmsv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gvnsicaoe.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gybxbxlzk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gsfyrqrtn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gitbayjso.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gucbymatw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gpnvqajli.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ggvxkiejo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gkykkrofv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gyhnefklk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/garogchrt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gdmzyctku.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gikrwpysr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/getaorcxb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goujeiber.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gxpltdtmr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwnbmompf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gimphntuc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/ghmfiacoz.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gakkgjubf.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gkxsexxgs.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gxupgaymx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gvltxppht.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gycceaqev.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gxcypobdz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gismpucni.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gilaucyjr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gzucqskzx.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ggnqapcwz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gcspbfnev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gdzqifxog.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gxejwohci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/goijdpxfh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gocvedjwi.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gzpxuwegw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grejkvkcr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/ghmgnmksw.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/godzfxocl.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/genxtwncn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/grxicupjx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/giphdskkg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/geyngxthr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gunvtvkyl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gdivjqekb.sHtML


<!-- 参考信息 -->