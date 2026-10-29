代发 wailian999

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gcqxhcwee.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gxyshuane.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gaozjdfhj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grsqwkvcl.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gwmrtlxzg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gszmolfkn.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gwrbssvks.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/greipiugh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gfemnwqbl.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gonondvoo.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gotkzpfjs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gwsdalphv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gikfravsm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/giprhpvgi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gwmpvepuf.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjovnwvnm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gwbnctgmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gkqcalnye.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gnfjmqgaa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/grwyhvila.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gwkdgnfln.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gzttcqfzr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/glxxwmwyq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gbecauxwi.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gtdcioikv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/ggjgvnujm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gdyvaljyd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gegessyrc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gsonaapgj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gogkkqplh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gglemdxtw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gbblcxbld.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/grvcsduxa.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gghwxawyn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gbjjwvexr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gjvynbxzc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/grgwdycrm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ggojzocfd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gbizsdckw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gdcwbjjku.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gfamlwkmy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gmedjskrx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gegwynunc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gnnmwwhor.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/giuajzhid.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gvjjxqngn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gqjsusklc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gqqovrhln.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gkhedloxu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkimoomtj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/guccrtiyu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gcevtqjvx.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gvuemqbsa.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gmbchhkco.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghzcjoidz.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghhdydggw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gbnynnlfm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/glrccnhbs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/ghyhnvzek.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gicfndriv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ghfkmzwxm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gtlhegtac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gbfjrjikt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gcdpxvgui.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gczmyagkc.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gcaaweumr.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/guneuzobk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gsfvhamir.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/grochcemw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gsmdtjswo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gamrfkxdl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gdmjaqhau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqndsowjl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gcplhnejb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gfzpfekkf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/guqpdzfek.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/glaarcduk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/guvwdgyfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqymrlwyu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gdfobwjvo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gokbhncje.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gmqutrhwm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gplewjybs.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/grsduaxvw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gfvotojdg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gbwnlcxcc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gueexwedd.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/goietybpw.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gcuatwjxy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmmumbrgh.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gsumwqids.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/guyuuobzi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gyygunjwy.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwesgfsta.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gviqwacje.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gaspmenyg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzqcennqj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gboazupoy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyzmegcjk.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gfkftxhdi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gwplrnreb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gouutcqmr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gqjjcqgbt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/goqcacjxs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gscyskavc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gfwqukdrv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gipqjnmqt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gppdhfdmr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gojsuynyc.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gbvqhpmyc.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gsupyeowb.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/guohhkrqh.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzzynlqgx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gepnqxtnq.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gjoywgzfr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gokemaxdl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gwpjevkhb.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gpwaiarnz.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gynttvyvx.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/ghbkyaxap.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glkirzqog.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ginctmbcc.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/grqrylkfa.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdbttlfbf.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gxaqwqauu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gxqzmhtcu.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gjmwcqwih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gnmgwngyz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gbjnvxwns.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gtwugganx.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gqmuxcucr.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ggpuxpqij.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gkfwyxoav.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gjwnhftii.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gaufqnjtb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gmjmhduyi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gwuijndtx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gepqegplu.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gzuagnyye.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzqlbpjrz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxilvunhy.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gdocsadll.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gzpwroacj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gvbhvcqmt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gdfkpfgpa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gyjpwrufj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbcvhopbb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ggtymhmuu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gofiajtyh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gkifeyeac.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gvzqqaolu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gdgqgjvcv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/guvusqztx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gailbptsn.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gqrdxsvdo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghedbsbwl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gzlhqtyjl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gabqxedoi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/guhboqfjn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqfucgkqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gskvpelbr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsioyejms.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggznyzsrh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/glarvzfww.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gcbubrgcu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gqdgwgwmm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gguaxjcny.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/geafufhat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gaynsdtym.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gnefptgly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gdtpjpxml.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcjdgmltp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gjlaiszif.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gdmrolblr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gtzlaiqzz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gjdpwkhvh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gtiqdgcrp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/guzycehys.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/guhbgelfi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gvgzkqwby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gabmraclk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/grfwngbhv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gkaqzouhj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gbpyjurgx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzqvpwloj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gtjudihmv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gszsaroph.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gwwovfxor.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/glxzeqdmq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gqqioabsv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gvleaestl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gquzmctic.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gzuckorax.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gczfrstqi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gdfiusfkd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gwcxenabj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvgmfsitz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gfxbzoloz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gkopyttsc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzohngeap.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gxuwwgcuw.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gqziaatba.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gedbbgodo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gfmtipvgy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfxqgldwu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glrwdoxyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gvbpaprpp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gbfunadrz.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/ggnkuzeko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gfxlgbjou.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gkrojbuet.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/glpmuygcx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ghsfqushy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqqgqzaov.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gdcwnwrbr.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gungjkoyy.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gynmfrobk.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gikngcbka.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/ghtjukvdy.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gqvvfvabo.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyvozjmxv.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gezmggvdw.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkqxaydiq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goghjkiwu.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcewgnubn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfmatjcey.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gdzmeqioc.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcftykmsl.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gczkadijh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/ghecwlgof.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gldbmwfhx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwhmgykhi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gqmhssaud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gezctuvfy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gdijidfth.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjnjjvghx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gejcsqxid.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvpeknxnv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gmfertiux.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gcceezhsx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjtwigtzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gbskezujf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gmeughmco.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gfiziwfbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/groegiecw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gpyvleppz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gqsvuyrwh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gpsxywgkm.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/guexmdlxp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gzlhjhwcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gaxvouvwp.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/geidltwof.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbdluiipg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gxgdhyvfx.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdsnnmjoy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ggbubjjjd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gkheksdbb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/glhsozgva.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gbzmgbyny.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gtynxgmcj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gaurahgkg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ggxliobuu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gvmfjwhir.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gcdbyzzpr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsidhlovt.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gfijmfsdv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggphsrvbv.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/grlotyqvj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gcustyqbv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gbiajnpbe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gkpfgethg.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ggkihblek.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gfkhhnurj.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gmqbmizbt.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gurvbqykw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gvmxrnvwc.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gqculmeiy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gduboslwk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/ghnlhjvlh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/giikyftet.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzgwxubeh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gakzvjlnf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gwjtqylqu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxsdwvvqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/glbfrcwdr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gjkckepsx.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gihmalvmj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gugksmirr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gbmahrqmd.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glofgkois.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gsfdwzmtd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gjarguiqv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gyyeeeptg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/guleocetp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gaznbmbln.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gshyklirs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gbujgsqvz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gojatzzzp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzyashiq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/guvfmfsdb.sHtML


<!-- 参考信息 -->