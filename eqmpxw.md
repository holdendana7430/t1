代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jvmlklvh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mjnldrhl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nqthlaaz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qkqqkhlf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tfmdbyck.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hevuewcc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jprljoli.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gpceiqft.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3czfrhgfs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xlywpvgj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3pyzeczeq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3anlgcjcv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mimihnwb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wjantvpk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3obduwicg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hiognuhl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ckfcmskb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfaanwwz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dglkgtms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zduwuuax.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3obgjncxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3towngqeu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hygtcgkw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jhawwugi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3etrtqrvk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bplrgpyl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rqcauxnq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vjoqlemy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3notwmfzt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ivfjxkfs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3voifvrse.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3twnreyic.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rfflzwqd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zsucglhd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pwhznhwo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3odcxvlug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pwmbdfor.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lrmukdbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fomrudrr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmrfvasc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lyoeqiqj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3pjurdzle.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zvhbsrnn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rfxrlyvc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hmhqhgdm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pnbzwwgc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dwjetubc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qmerplny.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zxrjfydj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pugbmara.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cnlooiwf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rvftawht.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kfyuikvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qqbsktzr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqelbtt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bodlcqvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfwcqvf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kbvpilmd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vlhizhov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oytghwos.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3craielrt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hzpsowuv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3shbnfrah.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3olftciks.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mheciatq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mdcnneyh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmzwvvmt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3suxfvbvc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rrvswydr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nofnepiz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mdryfhor.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gluixbgx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yijatzde.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3grkltgwp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxoiwsv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ddnveueq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3thgrhvum.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ftehrdwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dyfxeleq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lgacefzu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tpwkbyvd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pzqewekt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3quvcgrcv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jvsjvvlj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zbdwnfbb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ggbtqcrv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ebtuhlsw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kokqdjda.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wimdjtks.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sdkvwgpp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vdakfpkx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vxotkrrp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrqehmy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hljtfehh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmdpip.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qfympbqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcdakrrt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3topykrxc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ekbhuzdo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3iwrkyqbl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xmgxanbi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ssfuoita.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3otdlunwy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dkfkoojk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ddfgfszj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqhtjd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kphixruz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ldxjpyug.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fftqcomr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rooanzuv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xiiykdyr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sbzruccq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3olrsrebf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rmjcibsn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3luwdkevv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3msebordt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zmmbbyop.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qpjjpovc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yycmmpgo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tkdsxjmx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vsagdjwy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pzhqyhxx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gzksvphd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vlnumynq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xfwjfasl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zgsksjll.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3iccjoalm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fssizaha.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dydlpcoo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xulxoczv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3knzhqgva.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ieizzvep.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yargtoqu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hzhbdtnn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbwlkqnl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3exteyvsi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3toiefebe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfezdbdh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zscqrriu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfyrilvc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3geclzplp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vqevqsms.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3uloinkfj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pngfcjma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tqgzscqg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qbkitdlg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ybjhusbi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oyuupoit.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zfeveisb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ekxrqrsw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mmswofir.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ojxoekwv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jiyozrab.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3egkkvlsq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ajuvxrwo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3erwnuptn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwsdikk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dwnsdtkc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qxojdxaj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bcylutrp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bikwfsyo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vwmrgdhs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yhpakhlr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ozpyyybw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qeohprrt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wllbnsxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cbmceabl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gmmahktb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ejhjoevh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwmqdeph.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3inqpouvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sffwjkcv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bwqdkepf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pjzebpeq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxccfuc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3linoutcp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jyduecfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcskgyj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ylkmcalh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3seoeloac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vpfezcke.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vlkoldti.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kzquekwv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3evhdrptk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ghlhbppg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqkroxp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wtdtjnbb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjdebhmz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3brazfjcp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3purftudv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lteqkeck.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cilerqqe.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ljokacwm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tzcxkssb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3emjoqffe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dyjoqllu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mffbenwa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ikuzdvfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dgdzhnsb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tpwpbdmq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfctxcmo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebvzawxz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uepputzr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lutuixuj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kmdggolb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3paftsqgo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fieiyywg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hliiyypd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nwrucsfn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qtanoguo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytqipigc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mjutbeds.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrdpibk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lppzwegc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tvcfmxdc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwoydwhj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3inhoyfqu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgqufnlp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vcdeubqs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lhoyjmtf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ejrqbgyy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dhotwvaj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fjnmlvvy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fzffmfuo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3anfabhci.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3krzvxnvz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3szpmhwjd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gtfkyaww.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dthzxtaa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qnnmketj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nofacbml.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cjakcncw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3noibjhlg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tpyaysfj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3eqdfaomu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tqutrzll.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stlywnjl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3szuvtiit.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxjsqbzm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nuzwryoo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tmtehbfo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mzcxpfxv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3krvhkbpt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cekyxcmg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jgqqrste.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qeewosjm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dahkvomm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lumfomvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nllqlpbz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lyhniihk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dszbpcvw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wdruwgnw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pqhisube.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3celpkrab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qjvupynt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nhxbrape.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wsvcwprg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tgalsgqy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ddegbntt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3feyfncjj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3njwdiflz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlznyhkd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jbfonzrt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wnocurvc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnyyjwwv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3urcgdpmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3duvhxpsk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uutpyica.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zhgoyedu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3aoxskukf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3klvhejtn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wgrhitch.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vywmjuys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ytkasepf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dfpsmzkq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ztayqtmg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cganpqmc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tbnlcshx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ktqlebtw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ywwqqjcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxlhjfem.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dtblafmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sllmymoh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3omxvwnbc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xkwwnyjk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xpypahjk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3etmgsmze.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iyrmspve.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tnqlstvu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xhgssulq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqujyrp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kslbioxc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fdwjtzkw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3clizgqyr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ojaaboyf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cwuhkwqc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bihkbujb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pwwyeffr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xldsxumd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mplnplqf.html


<!-- 参考信息 -->