代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcngwouc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaovjwi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tlidamoi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3facfksry.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cabjrqeu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnzlrdw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3broaoxix.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbsjnsvt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zdfeftvg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qzklbarp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jcbsxjlr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dcuckkjz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pnbqqzve.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3stqcndlp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3szcyyaly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btvkwozh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3swywltwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxlugzil.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vepvamfi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3fivvvfyw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ffjxowtt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3epbkrkup.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bvyvoeks.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zictzjqf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnfluvb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qiwceeen.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqvvknh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xbwenboc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ndagozjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3miqobzbi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bxkvtacb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3aomrhwms.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gydaupua.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3carbndtx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kizxisli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wupcemlf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lbpgjnpa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vidygosq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cxbtctrm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xsvnovly.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nrtfzejq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zpjemfin.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dghupjqp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cqpbvxdr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cxreztss.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fnpdkrnh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3indevyes.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pqqgswpi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3klhqbvze.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zmpftgio.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lojiylsx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jjsrblmn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hjxdmkmi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uutrquax.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xqnxzpiq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3chdizfhx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdiddduz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jpzjqrvg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bhmmrhyk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fdeibkgy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hhtjbltt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ormrerly.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3typytlcv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3agyroaxh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jdgpbtkd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3waqtvfmw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3esfltbee.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sjlutnhe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rxocibat.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xinrnnef.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsmtazw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xwbjexlo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3emqhzkwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zmzcfbep.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mpvuxzyc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uednzyog.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3egchdnhi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lmsucjdi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xyxizsde.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pyplvjlz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uutbqglq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3saxtwfro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ehhrdzna.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tghwhscg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eavwoqmy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nkglyvgf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3crhhukll.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cxqfdela.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ztxkqkot.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ftbiwjgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctrivtdx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3avxcdjxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vemwpaou.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yuslnnox.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xziwdqbe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xxyqytcn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fbfwpalt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yiiyjvfc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ggmzeidh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqnsacax.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3yjzmyhfz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kedjhbge.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hyevrsfi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nnzfdspy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gcnxensd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ttrczzox.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3htwxtxwg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3enzvewvu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kgxpmfch.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cyijjpww.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qoomrrkd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qslattpf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdjuoax.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rjkpuple.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ppyxjcos.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cegavujd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jyidmplg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cixddzec.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ekuzgjsl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cdnthcue.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xjjwrpai.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bdroprfl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3olkxbrus.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tmgylsxq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fruiiaar.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3epqksluq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ttjrkpqo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3utzzebzp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3figsgxku.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zhlnppkm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oekbwjvf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kzrqxkay.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxekxwlm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxumfgyk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qrpkonhi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jugukcab.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gxvykwqs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yixobzze.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dullqaqc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qviscrkd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tqozsjnj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3laykrxza.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3krajkxlw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vgwdkxte.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hhukblfr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wqzpsvqf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dlntktxt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bpcuzztl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3alqneump.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wkvqblym.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ktlpvjzm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3srsouyel.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qbwpufif.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zwvmoajo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kaletqau.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pxwslruc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ovefxuin.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3czxldnvx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dxwzooyk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jfiduovp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cgpbvvwd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xithqyrf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zcjfndnn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vedxuhej.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ybjjtsdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfjyluqg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mwxoxzng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oucsphlb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ptrmjxfg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzinphjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kddrvwpj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jtoftzlo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mjonesbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsqnuwf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdotfcrs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3duoaevsv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3isgqmasx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yocjagjc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3usvtvtxh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnuqybdn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vuoujuay.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3udiwavsv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qcuspcna.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iskifyih.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ravsyopz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bfeiefak.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3orquryec.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mvghuppy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3acdlrcck.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sydfqahs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bixvdghy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pswywsly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ixypinbd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rqgokpqk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3voszjpta.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hsaeuyxw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3axlqazpf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3widpfvkp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hhingbaj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xnqlqrsy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fauuicqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzjopvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ohblhxzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fkhgmnuq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uxxeiljw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rfuiouyk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qmxccbvk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubekeloz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3igdgcyav.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3umytgmso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nuvmzamt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yegjyjrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ddomldxd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3noipaffb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ukjkeqxt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gmdfrutc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fgrgmqzl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfbrus.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3phzzravl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ztmcozea.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ouxhiulv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bnawvguy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lwvecgjm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yncwtxgb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wkfxqnfx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xqayuocw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dbxtkpsc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jegfmivd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3isnkestt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yqsejkut.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3retnsvet.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ocbgpzok.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afuaoebh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cniowxjz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3woacruev.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddsthvrv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ipxtmpgl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cblazzbn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vvpojtpi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vukhjevr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zqwmgikt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvvrossy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3grtgigfc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abxzjkdf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3macqcacz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dkcomhmh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ghweywef.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uocsuhnn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3egdgofja.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vrbdpbwj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gnufeqxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkzxmwkz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ctjzxtqj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hkucaqen.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zgedsfhq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3atrszwvc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uihhjfni.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dkacxmfl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfcghwmg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fbzxpose.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cxxvfzdz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3txrzotxw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3plzyvxyi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jsytkhnw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jicqijju.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fkvipcql.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wxsortks.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vmkvemvv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3iwkyksyo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tevkqbkz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ryroivtd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3szcbikta.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tvibegjx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bscsgdcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3owgenqvl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zqoibhew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzekihxn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hlgijsyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekgrlmtr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3afxgiotm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wsoxcwrg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zsuubkwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ycfefssv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ghysclan.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gdtigpsm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3snwzhgey.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jneqzfsh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ayuvzawr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cyuafmlt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pavvwlgn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fvuulhkj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ujiwlzxb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jzvbqogx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zqhvkvnv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yvfizbsm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eeacvyyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwsfah.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xdomyknn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xztdpwkl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fkmxecdw.html


<!-- 参考信息 -->