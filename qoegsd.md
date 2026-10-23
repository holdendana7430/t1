代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3legycpio.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jfmmgind.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fhlsuruy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rapgidsd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wvfmvljw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ijazjymf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zyznjxli.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3euaoapdk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3seiheday.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zvhygheq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ydgqxdlw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pcrikvmw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lovezpab.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qezrnkfl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3omdnbtzi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vzgrgqmq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uaazajwr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rdeseweq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eseyixib.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ocqlkslt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uivfirqq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bmrltooo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zrcmjjjp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hxsnrska.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hkeuzlxl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3eogksimc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ysflleyk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gbtqmgqb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rfkxngwi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kujsyaxm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ckkqlcbe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mgczjazt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3frrhvqjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xpgtzoae.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xhjjpbdr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cqdwcvnx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3stwdvtxe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3koamtxqw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dnchyior.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gsfvrani.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdxodzvv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ptxkhdor.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qnryvlzu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ypvtefkv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vfsdcntz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmbghwl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kmkbmmgj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kcrpqioc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3medeeucw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nshcuabv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lcfbamfc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ejpwfjku.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vxsmcafq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mbaromdw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jzhiwehs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vummuevy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kuivgwnn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sdjvtcic.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qhteuttw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jennovep.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zduxanze.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qsflcprp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3cfqwkdsv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sazubcrw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eyvbkbbz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gakdblhs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eelyveey.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dnfpymiv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pvdpabun.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bixvybap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npcsdybj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lafpabay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vitgnrju.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bhetpckh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mwaghgvk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ugfaehqi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpqgvgh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kwymslmp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cuakztpi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hdahhlie.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tdwthoye.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pdqruaih.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qibvqoiu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ulcnauik.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nparboey.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tzfmvxfh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wicgeqim.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rdnowdcf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbsypaz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zaxgigsk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ztaheean.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pubrrazg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3aprvrucf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3owifhtnq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tvuuuxkm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qzitncjw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pdnpomyf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rxbytdwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3izunlmor.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bzfebtqr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3airmumhq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bbazhwfs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yurugtbj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3itzgzodg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yetpwhcg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hgpipdeg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lggxaqhe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ahtcipao.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ketiecoc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zegmwmvg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnvfsipr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dgrfyacb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mzwtaztv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mynapsth.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcfkzuu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vabtvamo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3chyoemee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3enosdsoc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3uvutrrjt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gnqlhool.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wbxmildb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xmxfsijd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bzvwdwvw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vrlnwkvs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqywpxq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hsvfxfyz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3foimigyp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yfmngpwo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jtfrkkmb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pspqcoxn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jymtwxpn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bhactmsp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hohrysma.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wdrsiqhi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3thpmlzki.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3smvwlpge.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xyrzvgfd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uxmxpprq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fnbstvfw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bjvjbpvi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ynozmbrt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ictsglcl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3crjtyqct.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hqexzwcm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cicwqqpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkwqwxov.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xymjwrnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rncbdntv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hmgmgmfp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3itubzxgv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ldtfqfzw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qfjaokix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ipmftcqg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbcfplxe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3czgdhncb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yrxlupph.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pkallkrw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gzcrwmmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vpclrjne.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fwossexy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3exvokbvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3njuvorcy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zkmwgdcp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ismbrotx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fpwmhece.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vnzihjmc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zwqrrepn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dtbegyts.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3spitdsoo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iwoekdsi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ppmqbgqb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hwzuaval.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3govzmumn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vhpznndq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lvpxfgdj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ntnvcnjl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxjfuts.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjmrenm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wpweqfmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kuwivllb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebmfwcpl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dgzjsyrj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3upgxrsvz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jaajagao.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qgdqwnyh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtplfpk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fohljjic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3okygzlof.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3onhjtnfb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pneublor.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qlbrnomr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmrfgzm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hfqewjtq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vvikyzxq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wkubvrzx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjckxhli.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3laxgucsk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3prnombxj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lqvwyxdu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gjwlxjxs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wtefdqoc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qexfikuj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hzfbjzvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nyejixxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pynzhyyl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gmcodohn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hjcqfsvo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zkkozulb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hxqxuver.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qywwordq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wjotfkir.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dgeofeas.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kawunmmk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3chilhtuz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kewmsltm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ybewayst.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ydvevmcq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wfyajytc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dmmredup.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sirsslnf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vwbfaegs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ahlwcayk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mvyduprb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vrnsuyqe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qbzcjaum.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qhfatoqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bvfveizj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rbgfmkyi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uywcrssf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qfosvgky.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tyfubqnn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sdgmmvvf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lvcemmbe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xlzqfrxi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fpzlfndo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kspxshbz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjydsln.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihwsgnyx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zpnspmns.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3njjdnqrp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3romeippe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ckuvdiql.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wygsqigb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jztamtyx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qzgbunux.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cvrvaqxe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bncdkngh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rlkgrknu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3egnlmiko.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cpkgnwfp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iriakwcp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3edcbayue.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3agoolqwg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3plgumzzr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yvhdfupp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3izpdcjpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfrorprt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ppmmatxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufbjsvvt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xzjolhfb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lswifmwo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpxlcxhl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qtzznybk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tsszqyni.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ildxnele.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ulstooed.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jvvstlsp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lbttgoyd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqctbd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3eyynchit.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gqzbtvyn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3apiixidb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3icvoxemg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jiwcnuvp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fnyhgjot.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fcvyvdoe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bwngidki.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ekqoppyk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qlpbsnlx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ktefpfzf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zikepbnb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uchohnni.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gfodnwhx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pqlqkhzc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjiwosv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iqbsmlui.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fulpmksf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3iuiinkwa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ctcpseca.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lxqxszwt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wsqqikgx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dsdxavrw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3huhzsktr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jdbtyalp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlyejfg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tihtknev.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uumzaqzg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3glizsvjb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyrnpff.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bqgudfag.html


<!-- 参考信息 -->