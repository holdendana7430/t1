代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vxgpfgsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kalzygky.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ctrchvzz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gzsknpfp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kdgoexmz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mmxxipsf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gwsourcd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bndmkcui.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xhawxwfj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3minysysc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zwygjnmv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dpsnpmxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jgdrxglj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bavhmjbk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tltceylc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nhmordil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yozpnkjf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ivmhvxbp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bjfifnbk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3azwqvpla.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3irfmzwyv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3djgumnwf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtoxtjhj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zykmbuxz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aojfflsi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3uevfrvgx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhjtzoh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lgycnrjk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wcqxjvks.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qgkerxll.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kykytzpf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wfleuqvw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ikosscue.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jkvczrzt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hcqkyqyn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kgowprxv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3beymxajl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lovcyzzq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aekxzffl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rbncvcim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fhhachio.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pnmktgpt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3luiohduc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iifmatrj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrdzwzub.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kvgxroco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlhuoguz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dboglvds.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nokmmclo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pqiwbllj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rfuvadpw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nailjmgq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3linxklsz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vibjghqy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yhlwunah.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cpucfvec.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lmemthmi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lddofhzp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uwirtllx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lickltlk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wzcgbpid.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jnnnugnc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xzwxrbct.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3crrcdbfj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ucyyrrbq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ymimoxyb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kobjehof.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mxuollef.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xindwfdp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rjdykcxe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pihxwgpo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3clebkdrv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fnjxffrl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zqkchjiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jetjeywz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zbxynprw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlmgtabn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3voykaild.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xyzuajwg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ljnihzna.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxkypxlr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rinclvty.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zlxlqqtj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zitnjcfq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tbefdjjp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nqujxulk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqlqlosm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pkntwfyf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3usgpiyxl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3srwdwzmv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ydaxkxxd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xgqqqfxb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cpwxfaif.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3azjospjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aruqmmnu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rqwsgopn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ewjijvkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jdhpxrxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tyrbhlib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nbqrlohv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bisevgnn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qzikynyb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fncpwbam.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pxyhbxsg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3smuvuxcq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vgofwres.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3anrxbapn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3axmqpfxr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wothllfa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3enwceyib.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eryfvcfj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xpjrxeil.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wvxczbji.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bdlncoya.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzpmyzn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cmfxwqiq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtvtaaq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3caxsfors.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eewbnjax.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgqkzmck.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aiythesf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3clnpphuc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fufpfzfp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ryluoqiq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kksifuqk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jjtwgcdz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hbjklzos.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sudygysg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nrjolndx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wwwmnqay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rblfbvxs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vnjoptjx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wuubjfdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3taqutonw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nwtcdhsb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nxpfavrn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rnukqgsz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jrhqxfqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rfbbqgkl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iqycplme.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gmquiseu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fkbzkyod.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lhsipxpu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iukfpjoa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3trvmzvqb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3akozxsur.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3brrtqzem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ukgbnqam.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3itjmkdgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jycxxiep.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rrwwilkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfrkyugj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wylnanib.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvinswz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pxwuahrj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rorqbdyx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3idgxcvlf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdxrgjkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmhsaqk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jqyqsfmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cfnjggam.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zecdnjwc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ecamdbyx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nvssomah.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3giftqkjz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qqthdswz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jxtttnet.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3odvgwydi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uqxvllgj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jantataa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jpovozfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bxzzdcqb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nuqccyvk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3exehsrdt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rodoeikb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eojdsraf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3thytpuco.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jaqcgbte.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ipuggqyr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zuexsnwo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhndfkip.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3duqzmczz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axuzxyiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxiomml.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iluxgtjt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yrrhyguo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhrrqlt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iuxduhoy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rwyojxxv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bqweqitf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3umdbjxrw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qqoginib.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aivgmiwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tkfdavyr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3auznmqry.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqfgnoqe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rhijokli.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3edmwxrsn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3acdigsnw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vkzwejcf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qosrtsza.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nzkbjnmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3glbttbgp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vgxpilnk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvvbgrsp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xdsbjnwr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3sgqdhgbw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3aopvfpcj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mjvkkxhd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mfzgapgx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nymkcbps.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ewycxzbz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cjrrfayn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mjdcpxks.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pmecjvpe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rjnsayep.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpiazye.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uiditvio.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3loplpcjx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kbeveaux.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3omtuyehr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kwmofwfc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mynssfgj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztvfwfnd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hqbyqcxw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lhosefmz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3izsawviw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fkkswvln.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3keyuxhlj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uointujk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fxwjgray.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jcnstipu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggmfuxal.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tukhvdve.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sxwwmkkt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jfozdnlo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3teffgffq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dlquaitd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfrgmdt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jrkmvloq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tvrgiupn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmsvqsyo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oaphryks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hxhumnai.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmhjord.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jrezkuwq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jpfbmmzj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wyebebhn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sxftnkhh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3giywrztd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gdreuuko.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zzkieyhb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hrbhtowa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dqjxsqkm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3efthehum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qjdqvxsp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bhblapli.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3smvbgkez.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cozqfqvo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3spkwaxcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cypsbyft.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ecjkuxdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alfdrblq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sojtetut.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ubulkfbv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dvhjocga.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rmthrblf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hauifitb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ezohirpv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3osefwdwu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jvojqgea.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lhjagztu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3dvcbiseq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjrfmlg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zbygdlvw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nobjkzxf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dlyvytmk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jfzlodvj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ufswyzgt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zypqykky.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dtdzofln.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hcgavsgd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjqnfuhs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qwprmhbd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3npzdzimx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ffuelauo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3exqjmcsz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qxzvothn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jmfjoput.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nesifasl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qtareiat.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pzthcjrz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kqildcwq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdrzfutn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lwrussez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yrenlbto.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dwnosxda.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rirqdhmr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mkjcnbzv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bhpfxzsc.html


<!-- 参考信息 -->