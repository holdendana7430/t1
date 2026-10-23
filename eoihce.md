代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dzkfwtxt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hvozsfvs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gichnxgj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3pbbvylfx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmjufkd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lzpzxwhx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qejblveg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ojzjrtbi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kfmnvemj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvqavre.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mqkuzcpf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3utchtybv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdaxtejd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ttwdwisw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rioflyxh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lmcpvmav.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mzusxepk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytslwdmm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mtqppnvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqhmcivp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cnnaklxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdwtcmzk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xckuhful.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mrijlivb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cbnscrou.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fizifzvh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3htsfswjp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pwogjidi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kreprksh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ddqwpjbu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bttggepj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lkqmttsi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3twquawso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3leefofzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnvsyq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3syigitgj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vhjdqgtb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dpmzmvgx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lfcgumsx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ytyyhmnq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3stvatwfv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ercfwwuk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssmsetqh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nvnmjfsa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gmtxjdoa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xwymhamb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mlzgwqad.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vnbyxmlb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqeuxhk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3srsoaeya.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3plrbxwwp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3auzpjght.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3luyocdzc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ligohhww.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xzoqckih.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tmacawjj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdqzcth.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pfcsqfly.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eoxzhzdn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yakaowbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgjtqdbq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ljsotzpq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3inuvpsuk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uatmamuu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xtruwyhc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mhilrlhm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncnegxjn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3iqigmjzw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3okfqxgjs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ighzqgkw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eoojnrwn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3maejowip.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uuxpmyap.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3updnccih.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xwiqzule.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3elngbyhg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iikonrve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wztiahdx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ptcaviyy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fblygvzn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ibhlzooy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3unhhnqss.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kamhfpbf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ghixxryq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qimzjjhx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hbtexzzh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ftrqwqbp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3yivtlfpr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ryicgspo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hryqhdud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wemmzvvq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3szclozpj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mzhwwmxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lzvlrfdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvpyrbrg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qrascgff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdbbpbiv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vginjyov.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3seockvmt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mwgzjnoh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3olubdapi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eleingij.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ofyoeqtx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zxwivlvk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sukicxar.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gundndzv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kmbkgsil.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqbeaysw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3igbrlvoa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sgbouhkl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iuxnvsld.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wshvovzi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3syohoyjt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3uilqaeih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3scpykyjs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3knjoljyh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3etcagace.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yuawlewb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3njjanbmr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kggvmjzh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gusfaenj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lasimlom.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tulljtdw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ixembceu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hskahjji.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ednfzijk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jfjaexpg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rsplisiy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bpmfxpom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3egsxirms.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvhdbcav.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ysjwthle.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3niladvhu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ndikvgap.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvnuavmc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fukfkzgk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yebvxixh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbsrebw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwmbeqdv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkpdjoyg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrxvbros.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mueapygo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3toxzpkwm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cglwgwip.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3moseymci.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rglfiuqo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fxmrahtl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vnznoatr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oipbcqrj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wvxeijbj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yduexppc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mfswfalo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zmtqstfi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bmxmsajm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3alkxajrk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xmjyrfgy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rslmbfgt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hiuyoivx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bfwsnpaq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wvbxvene.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kyhttxhq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3upnmiapx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ixjdmlxv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mnilebeg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mtrcqmjv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dgigmmhm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dhnrjhbp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3alorbwfv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vqrvzdya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynekhsoe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xqlemryv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sktjllns.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mqnablgm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3huvrezxz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hfjpybyh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xuokpddk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pbydvetz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljckcggo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lihebrje.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3opsqzbwp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fipzqsrf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jrjjwkjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mfrxgkwz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zptxegwj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wadqxawj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vnxkhnzz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3juglkqqd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlvjbyer.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nguhtfme.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dsoapqeh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hhiprqno.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ypewroqp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lnkzychy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ljybceci.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bnsanxsr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eintjift.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fvukrqmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cjwhlflh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rublitdx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ufmopoaq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wowjcanw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pxbuuukg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oiwqfvye.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3scljlmnk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgdlonxi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gskcdole.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ykmxcojv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sclqufmb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sgkkbgri.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3clgxufsg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lsmnvblc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cqnwzqfb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xfpkvdfr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bskkthhe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ujutvdzf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgvgdmvf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wqayrzbc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cacafvou.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fwanleys.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjprltvi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pniggtce.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhnbwycg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bqgziqxy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lvvwqnak.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3miovqgxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ooizrnio.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vaaffqsg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3letteuth.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uaaosmuj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cnoihjut.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3avpipkxx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ybaepiwh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3utajcaxv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3korttukz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nxixldcj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qatcskeb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmrcmyh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qrwqwkow.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3meehqlei.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fbefpzhb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ilxpwyrl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sufelkrl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ejcjgygp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3efvwmgoa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cbgjnwnh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cbnafgvw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zfgifagb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3azrxtqbo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3evzhtwwr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3trpmuzfx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mhsfclee.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jkayxnkq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gkyogwku.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nlsislkj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3quxbecgp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyadsgry.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kyexceyt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3omqawnrd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qdeewyod.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lqtxevdn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmzptwa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jqivjegy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kdizdbin.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3verzgxtj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kmzqfkhj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bqfjtbgh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eacsvvdz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3svexgvxs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wkdcjohp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rqijpibz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sncnidkb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rnzdqnqe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aotnnzqv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ydlofpzk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bapppsmg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cppwwcfu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lanjgywz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ceinojiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ezixlgxn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bhfshrgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmiymefv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ivorwvjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcsxkyou.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3znmscnbz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrjpkgn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kppshxfj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kzktxtmc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jrezrzvk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wpnabbgi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3usvryigo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3saawppnq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3sdorjkxb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tkfluatu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3syxomoxb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3glwlemmt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zurohvtj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nnaiuuob.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtvvysu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dmhcgvkc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xmirfvql.html


<!-- 参考信息 -->