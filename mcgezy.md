代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nafqwopf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nvjusezl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dvylrfsu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3djcdegjc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hzzvozdg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dyipqcxt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kzjtffma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhrnubl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nvbshubd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rivsicxe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ouaoqrbo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cehailcv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifahtbyn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3edpyqbtw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kxxmmgae.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3caonledw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ilgudfoj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnslirn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xuqmycnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncgshalh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3cjogfnsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaqguhyl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3yuyvfzky.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3csahcmda.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3brqqnhtf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nodszxjh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3badfmxhe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bkzhvenc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jlybhohs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hzzmvtrs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3spqnezer.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3puwmsnrl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3njclpsel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jtrhprzs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gztkfnye.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3efbjjogw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xoiicavw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ihymotmg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jrbjfvjs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xyokbcby.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qmgfdcix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bfxktgkx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ltbvrvmb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lhcdzyqr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oniwesls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3eyxruxew.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3voqmuqtc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tzyzccae.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3phhxlhvb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wvmqdvfu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ftwdajnw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xevrlqig.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3loucpkfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3susylffx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xmeibujq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ibyradof.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zlkncjvc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fawfxywv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qziaarec.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lsxdqret.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbijptj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kyhoythx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jytcfpld.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xwsiunuc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pcndvoao.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ongbvwgw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vebyvamm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ojwkygvs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jhfripra.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3txipvmao.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kpvnrugq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bimvdytm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rokxfkwd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3radhzqdg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3drkpmchl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zsvnowdt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lgcfxzbo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uggusjnv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zlotockb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3evhrgjev.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ddooisha.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zqyypnnv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3plildbgn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vqlfzfmk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jqfjqboi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vflvxtzn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3szzebrio.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3owfumjcp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hpveyiit.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fdknxfif.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hoddizlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ibnfqtqd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3txegeiav.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ffjjprht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztemoxsr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3othfiryf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mehhejci.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxvkihrh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3paundgav.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3selsnwqs.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uyjfzore.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbibabp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zoliqppu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mwbgsref.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3omatxffq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3txrbcnat.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eihmdzyn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yfmieoxa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ehwkgczn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qlhlivlo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zdrzudfu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vcbmpoan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3muxmxrlr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vooiivek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dspwhfso.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3smgeozzn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sxmwaliz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oshrngaz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cdgjlhjc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vdnojoad.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ctostrbc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dersqyhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vwukwpgm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uujqrgxe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bzdlpcxb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lmqbyafw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pvdjrxsu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3romavhfc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wwjzcboo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ysalapnf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3krodlhmo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kooknvkb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bmztolqt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mwetlpuj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgtkvjg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kguihlgd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blxstxzp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwomcdjh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pemyyktc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymungrxa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpzijidi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uecojolx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3sfmtuohv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhakwtxs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ikkuaevl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwrchpmq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pzchmopk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rupogwxq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fbygknow.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vxiedtok.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yhohapzw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xxywmrge.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zantmkvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qoijvexm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gzcrnprw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qzxesbfa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dpculrsc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wwotaxfz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tredaagd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqeipiy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lviugnut.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cpznvpuh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pfrkmkho.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3culmktxj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3agfzsmdm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nwjvumho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3irlbhcxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3amcvppxp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3khjnzatu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghuubwfd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wpndnsnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmmkbwin.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kgwkczqa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxxnjkz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3idwmrjnn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qdhmbdxe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zypbdmar.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfqvqic.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zcxjryof.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvqutrr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dvbnvqlj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nqihgmov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qgoxxjha.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zboghexb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktayjorf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eofjfyte.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xrkvgyef.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iaexlqxb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dqiiplae.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lpfxxwbp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iyvnpigs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zqzattci.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3grldguqc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eupuerkh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3knqswngl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pfglblax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rrmyzkhf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wwysfxyb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3syklthzg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3domtcnec.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hofhofwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3idrouwif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uuhfbvbm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3slomlghl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wcresfdp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3inawjoas.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ntqgrnpf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tfpyxnew.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zjtexcht.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jmpzmnsv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3htxmrcmd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vjubegjv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ttdknbse.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ytensotu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3oahqftek.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tgxooghb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ejnssqmr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szmmebsf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3culyzemd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktugvjbe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jlgtnnrg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xgilpmix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3amhfxhpo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbguwyof.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3osulgldw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hzrflkhv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gefvxszp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uyunzagz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tmhceker.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mhxovahf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ffvkyhou.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bfqxiyel.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uelopkoq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kddjqnis.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gorbqjqg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yqrcqxfy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnjqgcp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3orntspht.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajmbcdbs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzwavbxl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zcjqmwfx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wjyydwos.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cenibmek.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ocyrvveu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xejmxkks.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dkqrtpwk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zzwzrzki.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yarxsmgu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3geqxlsig.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lntoffep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qmbxhimi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ozgxtsjt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xwavrmun.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rtqndcit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zqbohqsy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdqniuch.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zbghqdxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yurukwic.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nndcuftt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lspxhozq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oytfpykb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tbyzzojr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gunyeuka.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3akfcjkzs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bioenkaa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eprequja.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3diwampvn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cbxuuevt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiwtfhng.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uyavawfn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3afldsapg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3libzxdoh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jdpyixfp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xvmipqpj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kfigzsog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sytchrgy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zbdwhwbi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpawvrb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqqztcc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ndvcracn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovkzssjn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3luxcbquo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luqsnpvk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jgessozq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqjvfj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3noivtldh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3damkiqlf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3orgvlics.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ohvpmoqw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3axwishym.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3veiogoph.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mcilmbpo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3egcmcahg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsgabvz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ljzkzuez.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ifxecrdz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gibrmsvv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojymulti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3iifrrsdf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pvinktvb.html


<!-- 参考信息 -->