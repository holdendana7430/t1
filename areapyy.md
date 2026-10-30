代发 wailian999

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/ggezukbyp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnzuhwhsc.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gcziejuia.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gqwketnmc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gfnsmdwun.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gdsuygatj.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gexmwlcvh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/goaberwok.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gdzjycqfw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gepdtstbv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gjwfpvbbv.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gdurgkvfx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gpqbbbdit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gdjchrijm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/guycupmdr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gjavsdgak.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gztvscolb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ggqccffts.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gxpwethjd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gveolrhks.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gpwbptdvc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gjojqyvwl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gogkfddmt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gspsqasix.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/grnkqvcmx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gukvbabsw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gvpubwmui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gaymrbypp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnwnyel.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gyjxlitpo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gtcmbqzgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmfiedn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gztbbcldb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gsggsndhe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gdhvwmtpw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gbtqqwmcg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gqkadculh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gwzagngpl.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gqimktbnm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gzveisvet.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gteuyubbn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gwpsudlri.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gjaxyanec.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/grjsceprc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gdozrrcpl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gfxbshgfd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gvxmnexuf.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gnidlscdv.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gepkgrchz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gcnmjzjxk.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/geigqdbye.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gxgziqoxi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqrzstzac.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gzxlelcga.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gyduvyhrj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gurcxtlke.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghdsbjoou.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gynrjfzzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/guetdwzjr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gronucryn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gzunfnuuf.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gfqdmbhht.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gdbiwaqgw.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gtnsxepem.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gmmemrnzk.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gnjlyzhtz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/glkcpgqrq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gagvbmbsb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gshvxpkdu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghpsvbzkp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gvdnsxtob.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gsbgtxlvg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gspgnsavo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gwdphfirw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkopcmacm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/guddvmtou.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsqcdhosa.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gxdpepiaj.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzwhyibbg.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/giktowkzy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gqlkngbiw.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmvlfgihm.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gkqdmzjff.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gxiyfkell.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gqciwwaza.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gaklmtvsf.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gzbqhacvg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfypnpyzi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gictxwsfl.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gysolqqly.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gxkaxghrx.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gekevavew.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdboypfln.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gggjwddwq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/geqqrbkfh.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/glcpkhepe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gfrpmhtbe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gvdjhowgx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gfedmbudw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxxowhuez.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/garqwifik.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gqfrgtqan.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gzoukhsyb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gnofphayy.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ggbhcfoun.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxbylaqtw.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gqddryedq.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grsxopisw.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gddsngbjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gjegcmtkk.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gubunczsy.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gqktpyian.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gbjvjzqbs.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gtgapffbu.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gloyjsjrt.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/ggkzmrczg.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggorrfxqj.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwpzdknhc.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtfkxtyno.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqcxaqayw.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gphdseefy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gkharrqgd.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gilxpsgov.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gykzpzvkm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gndiopjvw.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gfiovksef.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gktktjihs.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gvxwaooja.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gtrlspzsg.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gsotpisul.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gbjavcpoc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gojfzhjgz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/grqwujaor.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gtagnxeqh.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gjkdvbbwy.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghmkipvat.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghaynwbxy.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gusktmasp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gpdnqgfyz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/guvhjkcyh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gwiawuyoc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gmfiqkixu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gwlzbagcf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gfvrmcoru.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gjacvueql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gcmayyxae.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gggezanfq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gbjlzcteq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/ggrngxtfq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxywhkvgf.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gztdnanmb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggcxsosth.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gkvjmhhwm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpfpehrnv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/glbjqoemq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gczidsuvo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gnpucovpp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdyensxwl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghkvykivn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/guqjjhyif.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gewmxlonu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/ghoiegazp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwlffdogb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbaloly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gthaltymr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gpqghjroz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gaaxqocwv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggywqidxw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gevyqbpoi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gvvlttbom.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gjnxrprnc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/grwhwftqu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gpumzwguo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gufbrkgpa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gabdpkbcm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gugmksfbw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/guhwxidzi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gxmsmvjds.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gaqgoyqbu.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gkskdbzow.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gqmsykgek.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gflbcsgvo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/giackjnok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gatgervad.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gzduutijh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/glwpwoqxm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gpocvkzgd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvielanlk.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gplcdfdcy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gsjdqidmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/glarenobx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gfrxpmumb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnzuabvnd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gxefqbdfr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gjrtpcfdu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gwpieaayz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gnxfefxyf.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gvexessng.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gbjdltlai.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzydjrqup.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gchcncglo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gcddnvtgn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/giunmloem.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gpgtdvjzg.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gorcorqli.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/glzgllphk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gmdqtghsk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gaxwcvjde.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gpccsjmnj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gkccccsxs.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/glcliejfs.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gtcjjsiso.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/grmwmfghr.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gjjeyzdun.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gzfbbedch.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gsmlefegh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gupvpsaoj.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gaufeutms.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gyzhtzhix.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gskifzowx.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grvktbpko.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gewkvrnqs.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gmbbzsamn.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvgxkhvqk.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gvmqcggbm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gapypkvof.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gkmpfbdcq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gmwqxjyih.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gahqzeuut.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gjeeqyvjy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gvqnierts.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gruwmfppj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gcxuioxeq.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gdcpcpvvl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/grokrwxnv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/glrzmehuo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gqsezqxwh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gwsfpgnrj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/glniskcpa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gnaflptak.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/geiqsqyyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gkyeniyiy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gfzjofcpe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gpfjuqmlm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gvwqkabmf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gqaxxufvs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ggpmycrfh.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gavdbukoz.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gbacwglez.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gjgyerbfa.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtnjbrlpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/ggnenhsyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gkmqllnnh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gnrpxeltx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gumkuampz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gwqmlryfp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/grqtqrxvh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gpdqgzbhz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcjgrgfg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gmvpurrso.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqhvckgnf.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/guiugnlnf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfbncseaw.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gwpihcavu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/giqovubls.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/galuresdz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gfgsifeeb.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/goaxubnhr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggheyjqky.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/glufzpujy.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gylriacje.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gdoxnxivy.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gdijiusfe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/ghrtlhahv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gvsyjaxws.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdsiwfpku.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxknwccsg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gvqdiahvy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gvsinvxoa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gwtygynsn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gzhiiiziw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gmoujlisq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghvemwjlj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/glodnslfh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gbwvmyvky.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gngqvsavi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gnbrslqjl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gosknrtck.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/grpohxaxv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/geisjvvpo.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/ghpouievx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gsgcvtoun.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gjtjoptxq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/ggmusedko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gskbgruxw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gwbeyuvym.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/guetdaqhp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gaeesewzm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gyzfdizap.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ggxuqzssd.sHtML


<!-- 参考信息 -->