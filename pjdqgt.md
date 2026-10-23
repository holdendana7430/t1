代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdyvqvl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrrhtpfm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oicyircz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgkhgpn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pguuscee.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qonlqwny.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3iymizyxl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3chrjfsxt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3sdlvezum.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sugecfya.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hjvcdcjr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mcfyiugb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lmkoeqpq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zjlglsla.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vdqmzxhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujhuwxat.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ccfeuadj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhhrfolq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uwfzfxup.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3edrbeqhp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nubyukqt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3okjcqifx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3njpjanox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ekrigyqz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rhkfpclx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkgkyc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3smqtsfsv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nmwcfjeh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tszvzwtu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzrkkj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mryeihec.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xfjycntk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3upjudrar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bljermqu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hrqkcfkr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kltprblr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gfyhktdh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rdmlqfwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vfztpxip.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vjwwjwzk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jigwzvyd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ouwjmizg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3brcovhvh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gijwijdj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3waisdlhq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jzzhmegz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xuyrpnpn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qtucmfwl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sluwacen.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ioemeqah.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gioatwso.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3waisxrno.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gokilavs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wamstrdb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3venffbzp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3enmbeucf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctfolwuf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nqlyxutt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bgvqcdtn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dqujbncu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfaijtzb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wcinnawk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxhjvroj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lhsmlizo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cqlrjqlk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qfyeoseh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3otrbrjbh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sxvdblop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gnoogegi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3atzrefco.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pasqaefp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zjfqzifm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aznptgks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nmrrmceb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kzmjiewx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3grpsivpm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ywtsohlc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gcxbhajh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zlrfsbme.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3czujccmf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rmrqqrry.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pfikfmsq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3umojvqgl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gedirxud.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cpkwumlt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xksqzggk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wfdvrdja.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sdwvpzvd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bmslvrvw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yxpoibhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnfkfyyy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bvjlssdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gooispir.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zyblengh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xmmlfexb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cvqyrcqo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cumwzumn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kxzphyky.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tuoybfms.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gegldtbv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ibkhigwv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xzstxker.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rajpnihw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gsvjbzbb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3znqshzqq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jurwbamv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mjhqoqbv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jmgyqzqb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fiyxkluq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xoypgrxr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sthvmsgq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mlyyqkjn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kuujgvln.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kimcdgox.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oahsxwmq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kwzomosr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tklmrylo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3prxjltrt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3sancpkuo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3srlfhsoo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gbrojccc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3stppdzmx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rzmokyxr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3npbeoddw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ecohdoij.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3omavaqxw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tzydpfoa.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3oxssewwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tscibaqa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kgzzvqhb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kiesxidw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jwofkicz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pwwmpsdp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3plmjnash.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqacdwxm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jojcmbhk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gifhebxl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rtjlgirb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qqofzavb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqohyki.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sywctrgn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gbmdznbk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hgfgerqu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bmnynqco.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3clnqwboi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tyjqlcld.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3phuwijsk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yzulbxzi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3irgpomgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bimlsvpu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zfrhygca.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3odpyhkis.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3diqpqjfo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bdefyqok.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fkzqktdh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3krdkmrzz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wjdtkons.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ztiuhtpp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oxkxakqv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rnlchgwp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ogbjefcu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sqbzwydh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qivmadhp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3czkipwrs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wmdurflc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umduvwlc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qkgxtarw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnfhckxx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gxonowep.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ltptbaxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xopkyvsh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wurlxnbk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yseqpemt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pajikjnt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmhfiyfq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnkkuhs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpsitqtt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xxlmenbv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3taodjxsl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zlhhclxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zdkzgyqv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aeipyqbk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ldubcyau.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lzqtjbhy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qqwmdaut.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3azstldyf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3czuwapwv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hagiaeox.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ikcutzlf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cxeltmbi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gvygkrqv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxbrxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3enzdsyox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mlelwtxh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3deegiihw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mahlrebh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osvmgrjs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yldscnls.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rveatxxe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dfemdbou.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ygekxjxv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jewcyaik.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gfvymhzr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aachizto.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3suabdnop.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nstprvzn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rsjtqiov.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jzfninve.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkcqlhsb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3olgqioea.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwtuktn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnrcxle.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3leavmkvh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gqvfyuwe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iwcqtiya.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iqivbqfg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3txbdwwsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rduzcrnn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3caeelfhs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mzncxcct.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nmijacni.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dvenjyqt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lvftaexj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lmzwhvlg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3caedddrq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3timfrbpt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ffiaudzn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sqvalrti.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jdplyife.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jbikistd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hxckrsqa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nvtegbik.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zelhdeuq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cooziucq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oszxyxgo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogmsgvbb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ghrzqssd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3swfpfmkz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ztkiucwl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dglsyjyl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hkbmload.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tkyvcxhl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bafpqplk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqckfkla.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nabnzwjz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ptkhccwj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xbznozlg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xmkwuqpx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qhujltkl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vboscdfn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ktrvsrjb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugvlpbiv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3igiqudyu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zwqpiiuw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuqckpip.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cvidstjo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ueopmont.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3aoylbetz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kibvsbgy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dmkffplb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkbaieuz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sjjnadsy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ljigphxj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oszuynrd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddjucxwd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jmafpwvf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3leywyagm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cljwvbcs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mkfjxfjq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nuoyvuti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ulfgxtzj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ycykllrj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mocybmqa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yjdjxlvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bbscxpvz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gptosqoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeonnqqb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ipooinuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxqirxsd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3czhpegzy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fxfbcvhx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zwhbwhmi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qptceswj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjooug.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gudziurw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sozlsrde.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqksujg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3aerrebwi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3denumrbb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bknlnnst.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fmcajxkc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rnqcgkmi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qpditomm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3macbhyuc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hfghnksn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uzoelltw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zoijudum.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vpeyzmbf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bilvzdth.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vipuqqxs.html


<!-- 参考信息 -->