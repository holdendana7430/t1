代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3psndhfnl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gxlbunyx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3rekenufj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlnqjnqs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pltpojdd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fsumbyhr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3djwcccem.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oshykgix.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3tnpwvjye.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wbsnsiug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3szesgrbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqzrtgkp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vauzwuxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxdlfnjf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3tzpqpfll.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3axzhrwqc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qgjzwwwm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqonqrd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgasrld.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3igwrebth.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vxvfyaof.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3whobznvf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhbluiy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3puvexfgg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3osgvaseq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vtookiuo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fibgexdp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cbgrfhko.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wdyyiqnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cthrkide.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xblbbjpr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzuvvypy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3otlfmwmb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sfwfiono.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3elrkyjwp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ibhqpynf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rcfwayjb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3oyznqqis.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pexfrcsg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kqbvevwa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gybvomor.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3spsimxgb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gkivtjry.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qibuakcx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rfigmkwe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yffmtkqr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hreaktnv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3waztuprn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvgjrer.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nhqdklgp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jlfjcoie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yqadgysn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tpceaptg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3syxmhfhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bjshwcaf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zzsyhwxt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gyqyfbcn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wrsilaze.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnkdiuvy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vueviuoh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tnmuwwjh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ipwurxuu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eoztelit.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fknrurst.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ryedxiuv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hejvonoz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3twryftma.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qalbmofs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xykvjleh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tennxqwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hazcenpu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iwhoaccq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jtiaaklq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3algmmjek.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qkberyke.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3djcllgun.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iisqkgnd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fchihaug.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ufspcjgu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yqackihy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywmgewkr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3boouojfj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxopqh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xjmedofg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3esgueuim.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rqpjpwiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enfsbujj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uwehheob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fphprrdu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wwqghsvf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xvfsorql.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ppjfsxpc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvbnprp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3riehtrik.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vgrspfbn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3znjhykko.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3girlprio.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nhlbzgjo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kedklhks.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iipoyfjy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kycpnfee.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3szqputfg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mfbqgfzh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vkvsldhf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iniwqmfg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bjqpstba.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lrkcxqse.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lbnzvtvf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nuorqnog.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fdrofqdr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpsiynd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tkzdoswe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3estoyrkr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jftpqlgw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3snbpafds.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tnzbseno.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pvqnzcmt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lkjwxthv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3urbevenj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pycphday.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qtehkhcd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mftewurd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3llcwwehr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cwlgcxdn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mzjpwxfu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oefwzvwf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzfxlofd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3btzczumj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opigqppm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otalbmxb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uuqeazde.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikfxwypo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jmbonbdj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xqfcbcey.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jzjumfek.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sadrrnse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ijlhhaty.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jclrrugi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zbmltzhv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nezgzptz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xmatannj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kbydcjow.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jtcqdepv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dlwsxyee.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3euzopams.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3sxvxgdrn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bkpoaxyl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iktmgoeb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3racldrgk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nutsbfzl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3afcqbqlr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ttncrwtn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3luddacrx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3almncdwf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3txcqnvsz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aulpeoei.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mpobgnfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3awgprmjr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kjgwoljs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ilmxnnqb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zrfaniik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnqrmtef.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wcoxoljb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiyljzms.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hrgwuugp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3navqdnjs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iamokiuw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3syqouibp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rrhkqmai.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tnltxrkc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ypjigqxd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3udyfezaa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rvqgumdk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nrnrhnne.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zjyclqsb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3meoyhzuu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpiqmud.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aqeeaqub.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjyztwg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpmzkhnx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nlijbrwg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lopwtpsx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ldqygjzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3efwihopn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3duccsyga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3poygydyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dhkgtzfe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3eqqurbci.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jhooxomt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ozoilcnc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3srxzolre.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3udfucsfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dqdpmtbx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmlzgle.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3duwnpmbx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vkvgdjfa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuglvnnb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkbydlv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dqpovxau.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yehbnbuu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gxiszoqs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfqhkhrv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxlwscar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3befirkrb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkbdkkar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3iksotavb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xuybnywh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hjhdwkdd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3yjzhhncc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhbhvlfz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3inseqgxx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikqdvxtt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pyoggmde.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3siyihkze.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3itfymbyl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzqyxogq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iddslfut.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rxdzjkbb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uotdlzfd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gmdaytxh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gfbimfxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnkvqtg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3isnluvgu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pwlwibtg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lhuykdld.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bnbfkgwe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hmzbklmx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bmezkobo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdmljvay.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xagkgrod.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nagdhdvv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lpuwfgfi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vqhuedox.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hgliciht.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tfglmtze.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zloswrvl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rznbshnc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bvnkgmgo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkpvbclm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pdurwhwz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rhrmihnc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3boljbjgw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ylonvunj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ubkmhjlv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mtfidzlw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bvqrypto.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3braanysp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvemafto.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3azuxoklf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jlgxcudv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbipqldt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bechkjqr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3caxzhmyq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yhltobbv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwxkpkzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3smajkpbb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wjrlfmbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eberhbjh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tlnveewp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mjegdocv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ptcprkel.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fsbabrmm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cxqptgpf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nuqfdvsh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ezbqxrgn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3icnjsgzn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vcyxgrdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ymentavb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3smfdhapt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3auqtytsw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yehvcuiz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uwpvdcts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gabzmdoq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pyoinenc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stogdidv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zxifswmh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bqmgyfph.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vcbkdgzt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tqxxbxaw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pyjevepa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ihvscmui.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ejfbtikl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xbffchid.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vcyxjglu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zsvwefkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tprnxjkh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kiiynczz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mekgdxof.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3btttnosq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wemdlmev.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bclxmimx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hpiatron.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lluhdopq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yuignvkp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3aajqoxjw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qvhtxwww.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gpdzshut.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bsvtqebq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsmdfpb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vdzpoapf.html


<!-- 参考信息 -->