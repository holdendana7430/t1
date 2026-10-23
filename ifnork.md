代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sblbfgov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfpzbnu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3brudtprr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ccxsjhoa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3iprlffzj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zzthtqty.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ttgcxqrr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3oihmqklu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hmvnkpji.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrszvtr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qkbnenac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejohxwwe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zjtvytkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trcxwvau.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bktiblja.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3aawkoivb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3olagodii.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zuhmtkpr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ukywkqfn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fbrmvfvq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vautcnau.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ihcstqzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3atnwvxwa.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zuvlwllg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yqpvcntr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hgltojja.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3shymtjlw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3msrfgoym.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rygccawa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pvzsrqwg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3snrpqioe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3afeeoshj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pwrunshz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3eyhttyvw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3duzhrvuv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3trmhyxco.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fuxtgraa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ewamfsah.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xyzzvarh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3milfgcea.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nruzczfn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nbflxqff.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3auawxvwi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xwtmdlrd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3itrczgpz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3suqzrtrp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zmyazwmi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pdnuahgn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3eodcipth.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bqzmyyoj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3oikuwwik.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kdyqupxa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3efrcpjth.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lerxrgav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xxncpdma.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xzpyucbv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gntsdbwl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sracxjbq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ytjkbkqz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cjtnvrff.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewwhlbzt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnpksdy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xhxxruox.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3edwhzjkq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3banfokml.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ktoljnxc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xzttaezh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bgykhpsi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3thhyiaoc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dnwhlplj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lylywiav.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lmskbeii.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cymqtsbn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cedkpabf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rvcbokvu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3evolhwvl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oleavlld.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qppcyuhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oeuepofb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lhkzizsf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qnptkiei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jptoxycf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3agunoqyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kmlymsub.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tubqrbsd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iitjlmfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfqxrptg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cfsfjeed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdbclulk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kizdidhd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zufviiix.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dgyfghex.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fpxszlgy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfwokmb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nbqxfvmc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dwqzjpgp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zsmpukhg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bgfqzmzz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cbbbtiil.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ogwawtqd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ridzlfwu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3frjrhech.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3znkujucf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xmygruwp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sduwquws.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eroqbapm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pfvcwxgh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3olpequai.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtiztdj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3losblzjy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lbxltrqz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3edgdnday.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yuqpgqiy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ywkqxevv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vhsagxkm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3caalewew.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gytjslim.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3opsbpaqn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kpugjmik.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rwwhuebl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tlwtoldk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fblsgwsm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3goxqujth.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jvkazwmy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xmlmbixd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zzcvilsc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kiylsngj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pugojwjj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggyensqg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lelgpkbs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cndsjwao.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwttoyf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dgmjvsfq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tourqgbi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nakvkbbv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yvoulvnb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmupgl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ggthjzzu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dpeofehb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3geaudlfo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohatfxlx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3numcqgts.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jghwbxwv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3evcaflch.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ictipzry.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lcmsqwji.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dgrcvrco.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3puutezpa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ulreuyqx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zervnwlv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xgbuwxpv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3extcggpl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pzjeemwf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wkjsmzdm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nhucronm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iutztrso.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nrbppuea.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dzsguysm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xmxoagjr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mmpfujqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fircofyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljmxqvae.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yiyphqck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbfultxd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ngknqaet.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnesvzhb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kabsfcty.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zfxdyfbs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mvdcjjox.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwzfouzg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3guqtorns.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vfpdyrjq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkotcqdz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sciqafco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ngvdnjgl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3seozusau.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bfxuuohp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3plntsmgl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zapqfvsz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrholxai.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxqpsslp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pzamthzz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rmanzjdm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ujfhsyep.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ozmrwmoe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kutrwklo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3krfikmvw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ykdgihcv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kxbocgvj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mfahbvrp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vzythfuw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ljsvkehp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3abnkepez.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3utjvonpj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3itekbtjp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uaxkvqkn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqkumqez.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zgzherbk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dmmpmefe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oulxrgct.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ghajiqwo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqgjyahb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sippzwpo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mcsaozzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwyelsk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ffbktctd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyssrln.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gkdvpiua.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vimllrky.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqomrtps.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gavnigby.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnghmijs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aovpweav.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qqdjxaog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uzrdoavh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ffjblsgk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rhtzatww.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lqcyyala.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xehabdqq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwzefl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bhbfyuop.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3klttkdvb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nqeirdsa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hcrtajjb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mikdidvp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ofjlcpeg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tpglzgmq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eomwagxk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3woloxmmn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dxmyuxls.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iezoebtx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3baoltkrs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xifsdbwj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gitwdqca.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jyggsrgu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3onqoeclm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3avncyled.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmrezlft.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ypbqbnpr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3odquetaz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nbmhoizz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oazkcdbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3txwypjgf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nhsmazzl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xbswvnku.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uxlmhorr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ogympcwe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryclamab.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxnrwetb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kpfyhvfl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybusoicu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vzyfsfmi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wescmpil.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lzyyplsq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lbezxdft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gjdyqcvl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ebpsirkw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wkuqolpu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zceqwfjd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3whbdihcn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sdwiiqbk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zigtlhvx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wacwffyy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3iibkpxzc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lhweplik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jbkljpoe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fideehgn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ochgvflm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rpoaorke.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrobbev.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qrwlmcto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mnveusgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqlhmkdu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lvgbevvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbxpieoh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bxzvkmza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3swinulrv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3egqqucgt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zseivbhl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oarlycet.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ohxcdxhx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rfvbxufi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpgyzoi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dhokuyfq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jokiciyc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgmmwmr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vxhudzuc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qssthlaq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qdglyrzr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ykflhheb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rcejiujx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3syplcoma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3abbegpjp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gfruzsgi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lyeghwwb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eaukzoov.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nbpjhhax.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rhryvlqp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3soosumsc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dnoxpwdr.html


<!-- 参考信息 -->