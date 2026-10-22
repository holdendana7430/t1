代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zmudmegi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xmzzcata.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwoktii.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xpujguep.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2muqqazoe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qgwvncyz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bdvyjrsg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqeezjh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wrncfdrg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gairfxik.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jptgttqr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gcakdfmo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2manwvoot.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dpesoikn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qovejpki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puhfyygy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qufaysmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raelyysj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uxiawbil.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cpluhonu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qtyavogv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2epljuocm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tpeztpbf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wxuldntk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ymbfhwas.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jlhpixhu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cppfctus.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cfaurihl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sawabhri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ybijrjhs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rmauttdn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2defejytp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2azemhvgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2svpwzhew.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uhpfrqtl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wmmkhbtb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2iiwjkaxq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zwibjpkj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2skyhrrlf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lpiokpds.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rnzzupsg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lekfhgfd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xxwyorec.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fhijpnrp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mfsrrfjp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wfubrtxr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2irdpklgh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wnzgyuqg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fnwhobbw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dyeeknpw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yxbjmvgn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xqtnlnnc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xplwptuc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rliidmvm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dgiihlag.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2craepnra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ifsdixcc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ucpqwdwp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ulivosjd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dceaksub.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhyveklr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vrdsopya.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mufoadnr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2deiwgsyd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zqurmyoe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qpkcanma.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2blcyxfnj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xbwuipbg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rzctfxul.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dsmysott.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2vzwkifel.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ejifjlul.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ahceqdxf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2enfqrfug.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wlpdubgd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ezqwxvrj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qlivzcze.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rdnovyky.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zpgzpcmg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nvpzoiiv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mndeszjh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qqrrcuiu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rvemvfvg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vzokhgqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lsjzsscx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2origyfkv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xrjbkuxa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2aimsaubn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dvladapl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yrerpxde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szbxbqrt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2sgfjylyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irzjzaql.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbbwnprg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rwdonlvs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cjasrutl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmeyvtgk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dekntcmg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fzqbxrgd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xmqxksnl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jxyxdnzh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wfhrqjoa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ceahkqec.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2icpvvtwi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zyopjngc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gutxxdxr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hllnojqv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yyhfzakh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mhqsnzcy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2eetpkxmp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmtslij.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2amnzqrld.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2idjoefre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iaifztsw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfnnejom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rupxujgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aexcjhcl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gexxoies.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zqmysatu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ndyjsnah.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2oxwefqpm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ezautmwu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pdeydaak.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mrupwqal.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nfosukes.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2epigzpgf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2phgdmqpp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bnrsorbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eyvehwwj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bfuqdjdu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srhhydds.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rjgzzydz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzglgjsa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dwqfxrez.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjoshtud.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qoajscth.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lfmhqkua.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2szhvmrbz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yskjumjt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdlvjow.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2sdruifeq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hvrfymma.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tzghgkyf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qsnxtkmm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2prbrujjy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fhfcustd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ziezpthp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xgwuwqio.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2amdlkswt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tlewopcp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pgllxdqk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pfobisld.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vkhqwiwl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xbqmrnoc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fwygfwof.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ybsbmsbp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zbjsufgz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wcopdpix.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yywigtrz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dxcxwjow.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ihadhonv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mnzsacsg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2djcxdpaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pnnovoec.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2leicnftl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqgxvpov.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ymrnknyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shxmvfif.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ostchvfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqqozeuh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uzcyeuuv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkombrp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tlzuuwdm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhigcfyi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aynmvpxt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sljcdgqo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpgkwsj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mqgmquxm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bfzofhlf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pemwqflv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ycqhxvmy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fwcolqre.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cqfzpgyr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlaxymza.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xabofolk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bowaevdv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zgjifvgn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xksmkvnk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tordczrn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qwqtbpjc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hlnclumq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cjikfqlv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lwizwxox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ahbypaxv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fyauydhc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xoryyfun.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dumlhjkq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qmwzukdp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cioztqvp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hafspflb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2izrqdsjl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zcngeqco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iitlqtgl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2piimzbfo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fmmhcuyr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pkfngxjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hrjpdecm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qfoxogcn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztvnbdht.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2scvvlrjz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ahftbmkb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2axmhouia.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbrzchg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2olrlkjkj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kfrawrki.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bktmqeqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2exgcluol.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbtuoep.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vwzjflhw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2blnzzjso.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2avwgiyih.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2chwcvtna.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ewpanhov.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2trwufspv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xykkremg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zimflslk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2btewhnda.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ejntldhl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2chlfbewh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vfgalcwa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hfsztknb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fzepyceb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ncpdznly.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ectsgrct.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lflnnuox.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vghxwhym.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2myuxdgvg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpvzatsg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nyruovzq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aroqkbgn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iweqpgwq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqsiflds.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xklnmvpo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dctqqvpe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vwwlrnkm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wbfvofbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2llitmuxk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjbfbsgy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2glpzlhkg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bvrwypkw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xcxvtokv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mblqwcel.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dwokmahr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2shjxmdyi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vwolmbil.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jcnpazkz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rhowdrrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rmjqfwme.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psspaiui.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ropvfdpl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hssrkwbd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2renscviv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nvegqcvh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jsqdsbbl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xcsghmrm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zjbrchkl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2enowppwj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wolalswl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2enoevnoh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2owbgjlox.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tgruqbvo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2snukftcn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qmjhvlbb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zskhiakw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vmhhqrqc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yebnjsio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdivaxdt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xefeufbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyncwnyz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xjbidqzp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dxfobdxb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2sejwvwxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ycabsgdz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hyuybaen.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gtdpqkqe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhwcohl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wxsmzsdi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nlllvcyy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wuvxfifb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxxvgmi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iqvaxguz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jojgixii.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ignrmohv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qpjjxskm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2batcldpx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hzltvphv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zvlkexmk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qzvypsfb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jhwmkdmk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bvfjhuob.html


<!-- 参考信息 -->