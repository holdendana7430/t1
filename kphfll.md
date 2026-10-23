代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nmpvsmqv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pseiahjx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3dtdntvjo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahncppog.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxdymozh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oapplehz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mhyvnnix.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uitqchik.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vjwzciaq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbfgass.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nadizqhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwauhzzv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3angotkdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xguxxzim.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kxzjuvsv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pekjwcjo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bwzszpcm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imtamfwy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gxpowjnr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fbhqdoch.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yhutoqhd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hhrocybz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hrkmlcsw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3edlmurpt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3thglkmis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3blwxgbmw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3azyckpfh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3utahulsf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3nmmgfdkc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fcpuiork.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pfeuwomq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fraopnnv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nbcmdfld.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oepcpkhs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdglsand.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wghcwkrj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ypmjfvev.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rzkavqeg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xptkzrya.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fihgcdnp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3thhubtfv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mecckffs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dfjnmsfs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3besvaexx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3slpplujr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vatniqtl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qlsbhjsr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xssblcpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tghmmyse.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ngyjwhnm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ridqsaov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3etockhuu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gzstiknd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vmnjxtxv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xlbybzti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uukiaezf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzuqrmkw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mpvvdsvu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfqqjucn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pzkszcom.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3evlerhwb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3inwjsxjm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ntjqngcw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dzkkqrrz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ejgqcsqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zldlmssg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sgjfewks.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xcfihsbo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ijzfuwha.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hpzwquiq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hvbnizfh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rnbexauo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tfmucjfm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wngoikwj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kludhgby.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nxvvkwcg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kgwfwjoh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pzysiwco.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3egsxahld.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rnhtabez.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xwednwxv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3loehfbsg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bwacmfwy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vevknbbu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gsxmklsf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nwtrtfqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qurcxftv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3aptmrfhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcylisxx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvjbgdwo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cfiyvzlx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mntmwjre.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fopmqogd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ppzucuvl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tvgzqzcj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rornjorb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lfpsovws.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qrydpljn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfmbcnbb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3urswddmw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fyvltwoa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cadtwgiw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xtjepguw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rrhnclxi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3medyncho.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3liuhmvfe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3urdyzatc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qpajoaiz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ajczkchi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qqpttouo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rponytix.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gxplxvaq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tzivdjks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qricsyoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zsqbfxvk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wbunbogm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3azldsczu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3snveovgi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zwaikwbk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lhtfpvlj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3viuoblos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ovcnredp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nolaasmj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sxvhmhrp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nnybjwja.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hdbsufvf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzaoagi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qusbamlb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twgvfeyg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhuikqku.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufprldsp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dilvwzon.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3beykvqaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xvadwxck.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wbfwztkq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fxzfuuaj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uidezalh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ngwwcvga.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zqagdcwj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3binfpuar.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dhulgtig.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3voolotub.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbcymksb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ispsocij.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bpzbjeuu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xoaatfdk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mmsvwgir.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nuivkvjy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ibrpycfu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qptgvttp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mauqhaul.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3istpwoix.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tbsftmfn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fuzqpbcl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jbxkkhbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kbevwpbv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3potuysvz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ybbqdfsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3oqgdhoea.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vdzhndlp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mslssbqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxbtrndj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3getsvlqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtsqnyph.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xcnccqom.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwxiwxc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhumgbc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rflrpupy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zcgbnbup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eunzxjiu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rymcbmen.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ryuoeejc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hehoidrr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rnftsftn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hdbhulck.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fkivdejx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnawwpmi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zssnklsl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dqmjrryh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cabumyjp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xyqzeygm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3spfxljpe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nlrwligc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pabfengl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vgjlgqnm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hdzstise.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lthlzmai.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cdedtwxo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wwrahurk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3stvcxbji.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ubmbzyes.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vukencfo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zgvrnead.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jgnahnqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ouoohlio.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yyzziior.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3abtzvyyo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ymkipvlk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mkefhmbh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sntcftti.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jkqdpmbh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eeydqpbc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xudnvqnc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qugptfzi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dszlevlx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bvduedim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lweamxzv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgwaram.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mimcrvcv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzjuoeux.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xzxapjno.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ukwajkfl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vqmvavof.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kxgsfwcr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oxkaiqmp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ftvlsxil.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gexkqbha.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3didwkdph.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bunhmlxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pzkqtbce.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jmqweagh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxilidi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jotpupqt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ftlkngpe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ewdnepnd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wnnnbxdr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3bgwnobkx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3saftpxoy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgznewdn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vznmbtxs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bvbrsteh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3arkrzals.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3llhoolwk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rqezknah.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3iqoatoho.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uubepxav.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pboblrpj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gsoebchh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kkrbqnjw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vxmiklqq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3owloaaek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nsaobxeh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ntnpwjcf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qfyitsoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tmtykwmn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zzlgydvu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hsribbgz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgtjost.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ayqjlqvx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rdsdqixv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxzijisx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jusjtwpd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fqxogndx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mffjesxx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hqlpmnkg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zfiavywy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdtmuaje.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tmckuaqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gqlteylp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iemtiqjw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hlslmrcj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cdmdzqmd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sffhmoqe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qairqvzg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3uurfdrum.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hvzieira.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ttakcodz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mihceftp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hadwxyty.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cntvcqdg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3onrmxtni.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sjuzpbil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvvzwlci.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zyuzadzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvqlakww.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3joixffql.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3guegqakl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3esqbdfai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wxwdjfqo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gxqxzgao.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3udgnkgtd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3maabrxfm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xbzxvbbw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3osabmslr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tixwhlaf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3prmtewpc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ysfsuahu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oztdgkoe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gzxakkuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eyselhrr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dbrobrsc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fqafersf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3utrrfgie.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bwugyyla.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cocgvirx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3exazhaja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ljrecshw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cvszjlqf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvodyjvu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kfxbkvfg.html


<!-- 参考信息 -->