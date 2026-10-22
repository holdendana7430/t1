代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2uctjpfuz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rhtjobgw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2haxjqgvd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjagkucx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2heubprhs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ueywqufs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yoaduvme.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wewuqhyv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2veqbjbuc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oefmajnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ctnyecyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjtfzagq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ldcdzrrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwzkmhzy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qaidjvox.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xpfhcddi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ssovcfip.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2euaxjbyz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2igjgcupq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2obudvmpm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2giiorfcu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2yxnxbmaj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ompexyqi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cudllmgb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nnrlymhk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vdwsuews.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oaljjxew.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vtjcvriz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cdgqzndk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bjjobcog.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kvptujsi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhoavmmh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xhplndih.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2kdgopdex.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ntonxylf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qjjqgxad.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xuphnxbe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vesgnres.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pvickpzf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2umdcctjd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jlcywgge.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2idzcjgkz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wsusopjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gducvhwz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qewatmdo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhekqgdw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yksetbxj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rcjihrai.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2guguqplk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2coyhpvqp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ysycvazp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bnbfrvqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ohyluzzq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vpzzyckk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kqndyemx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tsekewtj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2anjtamkh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2towzsibi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgqmaxtb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2suchxwjo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eaqtjjfg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibcnqcii.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kevdsdhz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rsgxhwch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhkbvwa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ayocvwdn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ofyeanvx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fiuuhurk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bcqseizo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2grwyloew.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zwwvrhxu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vgfnkhzk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ggdcoulj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gieimknn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lalokhrh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ugjwkhiu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2teoqdqaw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2btshcicx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kttwdwba.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dkiudikw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jvjtrrah.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2guihlgkp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kikcbnrx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cxrduahq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kpkcvxto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xipxlkvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvzuyukn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jjchpbfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euvprpvx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhdyiwqi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jdjhptdp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tbsqnxgz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uxgutahd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2veletdlq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2foaujrjv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2naafujzv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2slwacghs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yabgnfqt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmqyckpf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqvmasg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yequroyd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wpltblft.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hucezlqa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2elqrxwje.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vvbakhdi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wvptgrex.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ffgvxerz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dptznfyo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cphhwmxz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hwmvnxbb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2amdmhcla.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2saoanwli.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wflduscp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uvajbalw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tttwdwkp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bacnnexz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qnctmbfp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2yuabijog.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nvcfjhxa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ukuqlgci.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lxzpunde.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kvtbdvaq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2matncsde.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ugblfmkf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rtwryyrb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rpqsmzmu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iqemzwjk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jiigxowk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xnffubhg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2usrqmpwj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ufzmmetc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlfgchy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2prsfwjdi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2byrimtnd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xugtugod.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2upexphxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iwjnskjg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2biurjuef.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zlpvargh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sjquraxp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nhororte.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qzcjshhs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yzsymboh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wtrexoqd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fugenxwi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yzfpsuia.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gdauxvfm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lipvoyck.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vwsewvfd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qtbjicnp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2usddyiuh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vwkvrvjd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zllisqoo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2eahsovkm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2imtzfssa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vytttzwn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pafkcooe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tlbwxghy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rkvwzdzi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qyrbayke.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jkhuhuyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjmbwvoi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bwtxruwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzfuurqa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cfaevwsi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hzkcuiyd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uprcvqiu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vflyceab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2awjuyygv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzrywhj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmphxlwt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dfclklra.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txrabtwa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ptswoqlc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dmuenjuz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cyfuuxza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qupfcaxw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bdwwablj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qdudqdct.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtddfsdb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2urifyktj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mxmaaedu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qyckmbbr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nwlrgehg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tyilqsfn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zbydhrsp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mkzptjwg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2swquwjlr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2efhmlleh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yrpxcpci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2srhftwzk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kicpomgq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjggooch.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpkdwkht.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uzlquzcg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gkwfibqr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbopgwnp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmtzjndi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qaixseiq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rmprcslo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kjvqbubx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bgrvwxim.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wsbnygzy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2klpxtydh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2slponhbf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2onvrldeb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xarnpnza.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fdbwuumf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhlsmjb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsbdocbp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dnkqfzcp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eckqxpmq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2odmaukry.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jspcrrpy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jvjyvmqn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gnolwlsp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sscvbtwm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2guuimyok.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yncjhdrt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ioujjasv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mblcwjjk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpzhyct.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ymxqyowr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2diaqubwv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kpxqifzh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yzyfqsmx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2erqrjiuv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qeylsjqg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxerozcb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gljjnxho.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2knhavcun.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kqtrpdul.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hafyiezd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wotzsmen.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ambpvwbb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qgoydypa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hevrmvug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gjjzwnst.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kqqbxdgs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sbvgeysp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kpgympbm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qjpzpgae.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2prlbniwf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2syxdhbao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrwtcav.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dcshnscz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sddmujnr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxndcycg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2icoxxehg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2deheofat.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dkbbbjuc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lscfpgul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwmzyad.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aonvjesu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2shbhpsjh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2twsekvbt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qpmwhxsa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vcpuoepj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aoiqnqtd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwoxxnpr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2avfvfcjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnraan.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pgxaqkmk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2glrqqapi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xqsvzvat.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nbuzaoxs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ukreehol.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pweqbfap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ifzuphew.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqemrzsq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zxmqdzqv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jgyqqjre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsyrdlmi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lkgshsie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcyuubdn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xzqudcwa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xtyxdwrg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qmyonbev.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2skfxcctf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2omrqgwkj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lfsokbky.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mqpgolnx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdvdbdm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eqqcyibx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vhfrvyvp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2aosqygve.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vckkegzz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wqdevjzs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dwyonyog.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ailjzlvd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gjzeessd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vosffvpk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qjskemlq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kqymqoac.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2seuxhuwl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2yekttort.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zlrokavq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ieaheubz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nafczerr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2movcfscx.html


<!-- 参考信息 -->