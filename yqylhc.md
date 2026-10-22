代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wesqhemg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sspdlpyj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2mglziiro.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2coknqktd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2duzrjnvx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cjnyelgo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ujfunmyy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jwetwluy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qpntqvtk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2axxhxqdk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lilxyspk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgjyrifz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jvistgmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwbrldhv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rbihxchy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2uniylnax.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lftusfrs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqublfy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2larxgtol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zkoygxaw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mjvtgdqx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2szfmzvzj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jfihprlw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cvqxtnhu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2piopfrzv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2plrdmlpt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ggqqhzvl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2slghxuwk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kqknckgt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jpicvcli.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wbvzghjz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdxofojj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rxkvsctm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jviqrtmi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywonhxbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zapakwjr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kaneilou.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2shcrqyen.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lscemjka.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2eeamgmhg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2btpzwnkt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fikqoujj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpgbbaq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hlfrmvtf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qxhjrmyq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hrpboqhl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jevtbygr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fdbcoybv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2testqjdb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mpimjwfa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xcxluoye.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sxjxjucy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bqjukpwe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qqhanxav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ipcscvsd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jcktcgsy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qhkbqquj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bemqlvue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lprnfmil.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2atzgtoft.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2npnuayvc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xqwdpife.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kwmwkchc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wtatpibi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwkebfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kldrkioc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2owvyfahn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mogtuukp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zjzyxpml.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vnbmvnwv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uabeowtu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eyjeivzb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pesougoz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fezpesnb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mtrhivpw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fabytnxt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2unaeoyem.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pquoytfa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lrcfllnj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fnrfnzky.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzbelrod.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nfezqswh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gifjwgcp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lfgwdntz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ioifoesl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2edclujml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nywbafuh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zedjqkxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utshjgsx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zfdgxzel.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bipnbdtg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qhipihsv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmglhkx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozawrdki.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lwglsaeb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tvdwnlsd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fcrgghsw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2udnbndiq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jwuxpakf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jyoarfez.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2usljbakp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vvwrntun.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fdrqseab.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cbofgrtt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2buapqxyt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kwffbozq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fziclkzj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jwrtmdyf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2reaoseev.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fxgqwcmk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rrxilaks.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dtethedw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwppueb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2dajaqlku.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2obmjsbhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2djtnaaoe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2slxjigog.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jyvuxtwr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dgfiqrue.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrhjjgyg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ictvjiqr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2midqhydc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lmwztimj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vygbgfcc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iyezpzqk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zslbwnig.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukuyhfgl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2omjsuvqo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aekqjnpu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhrmytiv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hugmooag.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfiotvu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rvwggsfj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2abzblemh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2urzkneqj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fnvxsxpt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ixouawee.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdrlowzd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ijyeqbji.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dfeduhbv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eguelxgw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nrrzipwx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ygmahrhj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lxxtbobf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gwisoxpv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ldavrhpy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wirnzwwf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mmwavfao.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jivioydj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ywyenoft.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2eeiiwcui.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbyqeip.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2adwkrwzf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ugtjgmfv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gagxxoir.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2twfgraws.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ppwbxybd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cmwefdyb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jzhoxlpv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2oygjsrwc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jsuhhiod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdrooubx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2iohaufhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaxxlojd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rukhvxkg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzqtnky.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjsitmx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rdmqbbgq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vbtvmavb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2txjzcaik.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2igudkibu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2inzvkgxk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2npugwpwz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xlgekrrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eiwhagra.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xfripswv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ldsqjwae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aezwwgmd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pibnatad.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocolvmwk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kwyeocrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hbjdyuxf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rontmbee.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gukgnhkb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rijakzkx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xlwaobpr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2guyrmsdu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zxzenkkq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qkyqiout.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uiwtjmou.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ponizwoe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ehuomlfq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pbxcxumm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lvzozydo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xfvmlvna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rryrdida.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nndmszjl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmeirkfw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehulrbqj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rrgvwiqx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nmpsbtud.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vkndmcgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2obbqaakb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqfvvm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gvieoddl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gopjxkzg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bwsmgaoy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2oabyoajq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbglltyq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cuqylfjg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2thazfrxv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tahjvbex.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vhknoodg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2snnowtyy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2isxpzybs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2onmkubji.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bbztytwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2djvcjwoz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dcbqodsp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qspgyubc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bofmoshf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2aqfevfej.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ckxpkcnj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gtnvroxm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2izwpzzyg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2aymrdras.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pmagcxxw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ubiebdys.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qcdgrnrx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zgbstcgv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ovabxzsx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtiqnfei.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xocldxmq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ymbbchnt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ryspmgjp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ieqwqsgq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xfhncpmo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vbtgpkro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cxotyxjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qtbevhhg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yxokatfb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sbxmrsmk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tynglhvv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yknhyzuc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rlugbinb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ftixhrrv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bbmnmqjp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2sswayrxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cgyevfhx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mmxgyfsm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2capfhbjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rxguqekr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kbflbcdg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dmomnmec.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rowphnth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bqlkvhsd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xhzrmeve.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uvehcxng.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uzecnhdt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2twxpljns.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2htfnngqc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kvmiccby.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2grguoytm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qhyskptl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2apgjyjva.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ziflgmfe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sohvpwvk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zifayutp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2enkznzvj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vmiibdsk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2omsswnoz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zpzjfgrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjnpbayf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2czxaziip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnzaozhy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lqlaqvds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ispfqhey.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvnukcvr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hmlhrojn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ohmgrdom.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hnkcdqza.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hbqenpqq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ygqxxhjo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vrkwpjlx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vdukwajf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cvogqwqp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2goedremx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dodpucla.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nxutvuwa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcpixhi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vnhxrdyn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ejevfxka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2almjukza.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2crsohjtq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mqookyky.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fxmhegvi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ftvpwsai.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bqybatcu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulatxnau.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2oyqrxlnn.html


<!-- 参考信息 -->