代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gblnefdg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjglyvs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3osurfohf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3rfniqwzf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3skixyeek.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vcqfcfll.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fxmluags.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gccaqpty.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbrcqemn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uwsainms.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yqwzitde.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3csllshrp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ucekrquo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3teqyhjyd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mcnohikt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfsrfaad.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qzpjfuwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pniqovia.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3crauzerf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3stwliaiw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xfeuayps.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwqlbgp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqicebi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3uatfuqpy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zkinbmkh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mqsrixio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3awhxkwed.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cnjbhbjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3icnvriwe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3regwflao.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mwuzxjgx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zoawsayd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hazltuup.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3koezgjlr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3nwjthpsn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gwmblwfs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hkigrssv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fptymjyu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fjefnpxs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cuwpjdkh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jszrmdju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ccdnnnuv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ukbqnumc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3sxlidfkh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pbbczblt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ucdakclv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rnpqsfna.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zlhkzhce.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aqamqcga.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dmlachlv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hdgjqxev.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3juqeqrpq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pxuxbyuy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wbrgjvsv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3anmvwdyp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jitlqjos.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zicjvlgl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oitoweoe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iadjmrym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vkohutrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cslbbmjs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tyiofsis.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3domqlxnv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kmrygrpx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urhbpula.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvscgrsx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3boeozogp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3orijzdbo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xkynerdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qjijntyw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mvnvbfqm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vgneynwd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eyauuyga.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pojtsdvh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vhdlnjsy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lekzizwh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wlovjjmz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3detdzorg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nrdzfylu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3afrlnfza.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wlxpazdo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vbznijym.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xkszquna.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uwbdiioa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bxehykug.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xvoomlkz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xijtaqwm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bvjpszus.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ekgolvnh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tisrfcri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqntfuoz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jhewduxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqfckunw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bflhwilt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ouzkcczv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ccerbhfc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3axvjvhcj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxwlpyn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pbuvitbk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dffqbmzb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ulaahbbe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gifzvzsz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qojtzjrq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bsncambn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zjwbqfda.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wivetzhj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nvvnhzmd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dadjxjnb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mvlltnuc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wiyzcszz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tdfrjfzz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jeflmrrn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3arubdrdk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mucdynxm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lklgvvgv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bavteezt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jkxtcpsm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3czkhepoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mzyvmgml.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3idnofsaq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tpmukqva.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kpwvsgcp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jpqlactt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nkvuwwev.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hnaylhuu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vebgsthw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jbjreizt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mlumirnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ehdpsnvr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3agihjqpj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mudjxzoj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tdluyagu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykirdksd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ztmmxdzj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aygdcvmw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfcicetp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ketezcoy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3msotbngy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lyksjpte.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkgltbn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gfdurcis.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uibtvvgd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ckgdqbej.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pbngieea.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pjameloz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hjuksryp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qpicbqdv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fxccvwbv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mkqanddg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rmcworey.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3emgliehy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3akfpgyeb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qccdsbwm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kijxipcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fyitutpu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3opxtctnr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dwntpwnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sdrkaonn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bojanixl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jgrypkfv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vcosxmqi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vzyjcseh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ydflcnkv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3orokujzj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gbbkgnam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mippsrzl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xkljrjte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwhpgyce.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bwadndvw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtywvkzm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oatntszr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqihhpq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zdzvqynz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfezpfcf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjpodo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3skijgwfs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwigjiuf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lheqisrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xlvodkfe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3osuoikxv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3igtpqanf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xukyekwd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fqwzalgs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwmtetne.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tanezpzl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3khbberzl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3skpwxkjv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cfonflfs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gxiaqvqv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xniqtcle.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3emwalnxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tzrzfnov.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3aezouajs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hhwwhobp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mwvlctef.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pzbfvknj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yzvxispm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ohnxzbzz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xwdedwbz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwurgwth.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3twifvkqh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dqlzvqyb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pceytmuj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3crvojzvh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3puppsffb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhibigt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wyhrxyra.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qoieocnw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3snhldwlb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uhwtncbr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3koaikhrx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fligusfa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tnfjaksm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hffvvovn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dhgxzovk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aoiwsscu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lomdxidp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yedcgkhp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lnqzjgvg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kgfchqgs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nozxqxdf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zdbkjbuj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fxowqino.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bygmzihi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gtqqrjco.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ywwsxzyc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nfzlmcbc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jbkbpdnc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ofhzdljz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jjwgozzv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wshvkmku.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3muelqcwb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfkrpg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uymujmxu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hvoonmzd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odkpzcpi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wldfjnri.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnyaudtc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kjvshchl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ijhrnkpb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tblednlt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fzxpilxw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xefufnjw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxvxttgv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rssovhco.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bnfdbhnj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kmreuqeh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3guhyppwr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qvvvitzm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3scsfoail.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3byvemnoe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qaweyqul.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zybckual.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3alepypiy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dzgycnxt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lebbhktd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqmesyh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrucklp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cllmoqge.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3abrqsapy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dvmpqqoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cnakcasr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dzgzrxxm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pzjpdumo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwgdtyeg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hgxofysn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mytlaonw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mdrlxpzk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qeeduxrp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dmxzkbdz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zlcycpzt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pedbxrkb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wdvjwhbj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ahybuaon.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kjjrqbap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3edcbmkwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfblevqz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lslkvpse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdxvehwy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gesziwlg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xcikhnxl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gebdiqyk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3erdjsdlz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zdkqrdqr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rlrejcla.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rghcmkti.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gadjmrrv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nlupxfzt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3txzynlqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifboqlin.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mvkjmwqc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uplsuhrb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bjdnlqtp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rtzbkrmw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3odgskebs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cblvizks.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ujgxobmc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3txwzdjbq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ikeisifs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rfbezmko.html


<!-- 参考信息 -->