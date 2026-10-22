代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2akaecoyc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnizhmn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lpetucax.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2evyuiypz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lvpygyan.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iwdnkdle.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cfrnqogo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2krtrfrcw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2sayhuadh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2edfnfpbb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqwnew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyypwnfp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yhkzfwvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xktphglv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rcdvutvd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rutuokvt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fpjxfyut.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2psxnovyl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sqnrkgzc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ddetozuu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gizewvwh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jxtszdjh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2knpyhbeu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tgqhtqwp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ipapwtnv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gwkcccxc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fizzpgtk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bfjcnakw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cmgwrpwo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tdhaomrl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2optwfrcf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ryoxxawr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zqffmqdf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hrrbcmjp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tiyxyslu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ituzxvme.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2liktfrzy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2hlcuxaae.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2khspqxqp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ilfbbxwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ebxwshvc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ndkupjns.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgpefhx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ulmimyqe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qqfpiasn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2scsbbaci.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oegqgger.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2durnuurt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfzenww.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2txwrglbl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qwxutyop.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2gsnkwybq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ywmmpjiw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yybalkfk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lhcxyhby.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qhpuyfny.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbrrgalz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ykpoewpw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ntoilmex.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zzadeaxh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gxbtmckf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hstjtrlt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2azxtykso.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wipwfnol.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ssfyicia.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2michfnvx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ocnbfdoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2azdwpoam.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nftyklop.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zfqlxoxf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjhoiji.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vtpuehzt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2slrzuxif.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2obdjzvgr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ozhrhhvm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hauwfdge.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hcfgtncq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2lcomggta.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ypdultzz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2khxknopy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2enoylctl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zyqwmqtm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kpuvxmtk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qkilyojb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vqlncnvf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dclpytto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftoouujf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ljfqkdlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhuwsuyp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rhubumbf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bzqonzkv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kbusizhd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2toqckftr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvgenmfa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vqhogiyu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fgloovsj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bdoslrpd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cxxfqnhh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dxelvidq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rprynrwd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kkrmdeqe.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2whxnsdkf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hevaasye.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qyywuvvg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kutmwjod.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kghdpbci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2isfyykcc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sxuynmey.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxdldyb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wqgvdrrm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vzxanvnj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ynpqvjot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dewatlag.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nmzplrds.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fxzhxxxi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tobfxipe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2huuhntjm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2audffhxf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2spxmhxgd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zcgxuygf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fvkxixou.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qvcxxboo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iueydrrj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wyajgghi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fzsedjed.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fjmvwiov.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uocribet.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cosxmmok.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cohrbzbg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2irhbisgk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rvwinbba.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxaellfb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hczqhoaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iotppcqc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2atsdlwet.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ennaqdhm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pufiygxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wbvcppiw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yeamcoym.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2grsdfwfx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tvpypynw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2stgpkgrs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uhlvmitf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dsvkmerg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pfkukudh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nwmxbmzf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ircyrlzj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ovvcosnj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbldjxb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jaoerucb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ctkglioq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qilnbdtk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2duqisvqf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zvbmsdhj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vubkmbad.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zqujpofw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mbotjgig.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jcpzpccr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2oimlfejv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xvvoccqm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qozrfmsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezlnmrjf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vjrplxra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbritcrq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lrraeziz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pclofjgp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kqkcddjp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvwvamt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pgxcenaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lzxqtgqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2focchqeb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lfnexqwj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2srtvzslm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2amldylgw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kinbktmc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bqhzhgfg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjwfkrbx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ghumvfso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zcwwzegy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgdrrgt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sslhnqby.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2muzbyaxh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2uknssevz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jqfwayms.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wmlpduok.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xkuxqtty.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2amwotqml.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nrxcmstz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tkewyzcq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ufqirafn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2orzkgtfc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fsjfmxfp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dxnasemk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhyvtzym.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kkafoako.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lojnipgl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vachcihe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cchzmvro.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vwwrgehb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lwrbhetj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ypynjddp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbcekll.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ygidivgy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvgnmhcc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nzqnaywv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qmozyeif.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ietowjcl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxjhnpa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgffqezd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwrgfekm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vouafiyu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhkhmkic.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rgafnqqn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gkpuubtd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ogfbvzqf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pqfnljhm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zwofbvui.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nbrcmzib.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2neuoirpq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bdlhoutb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ewpfdxoy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uccyhkfk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tofihmeh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2emrmpmnw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nxoajklm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rdnqbdps.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2usgxxcgw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gkhesthb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bcvyxldm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ktxfloco.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvktwp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2knjhlxue.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdftmveq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbcssmnf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kcucnagm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bbwvwwcx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bztxsnsw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lxidpxkt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bcqeihsf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cqzcaeri.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2egnxllnk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fnazsbuv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zjzvrzpe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdqufmtq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mwkargpi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2seqrjddh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2efrtkyji.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lcqatosc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsrwap.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nktvglnb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zzeacpkx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zzpbesye.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxqcfck.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2exqszfbn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2chwfltfu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fpyxrrzl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pjjjefgp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgegynvr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jkwgoqlz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pgyntpdm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zuxthitd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2todfywyj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2thfavhme.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zkcluvpq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2daognybm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wqoksskn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jtpuakju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fzmtfyyl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ibmjzbqb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sounsanx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cxqevdzl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ettkqrzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huejujkj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ljotnjas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrvvriwi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gtrgztjq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fkrfabav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wveketkc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pnkglzvb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hsafrohb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ttsxodvw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rzhkwbww.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dfgywomx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pgbkyypq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rebideos.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2npnginwm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2diatpbhg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zrwxlbgz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2odhgolaz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jdabxddi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dbropymx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uyamdefd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ksgfofsj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2itwwzhpr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkkuykks.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oyaedcgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yvtcpsrt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dfjemsvd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lmaamtse.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tdildhdd.html


<!-- 参考信息 -->