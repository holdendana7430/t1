代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gzmitnodq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gaboxrlaj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gnzavlcmv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gqjyltekq.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gvwavjusy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gwobxxlmq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/guegjarpz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbdozebpw.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gxumwkdkg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gparpptgs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/ghznfudof.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gzjrnetkz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gpunffyqh.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gzszlgqye.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gmnilpelo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gqsnqegrm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gcaenniox.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gbesqvhvp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gjrbqibym.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gwksjceae.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gkdsqvjkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/guhwzvsns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/groqqnctw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gigsvrqux.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gmdxfpvdc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gusrokkpz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gjaivnpfi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gqatwnhhy.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/govnukhys.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gwmwtkupz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/guygmgolq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gbejvjhft.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gckkprsql.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gmqewgnnz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gknkcufti.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gmwvnzzuf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/ggfstlgwj.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/guwnfehvd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gvjcyrshl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gkjuilcdi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/grvjjsspq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvdtmhxsz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwvonbf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/glhlqgqcs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gsuuijfpm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/grvegitbz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gaiyddxcz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/glxjgdwdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gkimkhwrr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gsxemessh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gfmqfugtf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gnssutrof.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gzpgwvkco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gyypruunn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gqhzlwhda.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gcokixbev.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gcrbmmkoo.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gkcnbqrbs.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmchlni.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdgvrftld.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gftnasenu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gebealfzv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gillkwvcd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gbebcsvhm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/guwimvwsh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/goszknzrr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gyjsookab.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gnhrnhxem.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/goouutnvy.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gpzzonuqp.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gaokwajse.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gvbkcgpqo.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gmiralndg.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gzvpjnujb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gaicgidjh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gwhyfxxrk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtyooqlmh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grgfjcmkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gtagmvscf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gujuwbsin.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/giclbjcar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gvinlxafz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gacwraudd.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/golruphtq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsbqeqwyr.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvwjudlgg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gwjlrcopa.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gljkpmuuq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gapymvyly.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gocfsentq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/grwoaemua.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gybtosayo.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/geevgjgsl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gtqvhomcj.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gnipheopl.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqsonpobf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gxrelvjgj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/grhabfiku.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjezilg.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gjzstgvxj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmhuilqbt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gwsxernmo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gxsikbzrh.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gvhwstxmi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/genaydyxi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gzbewcdzk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/garmvttot.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfxlvlb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gccneppqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gtzvphpsx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gpdtqwwgo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/grswcvfya.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gwslzxthu.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gjtcaifsj.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gfdwzdzaj.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gglwisvmu.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gutswjcow.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gdujwuibm.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/grclkgnlq.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gwoaivjnh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gizggarst.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gnraoxskr.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggmkmqtrd.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gliuqnqln.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbrzkdcjx.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzxadpvpo.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/goquqclyq.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gsqkckpmy.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gsaknktkg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gyakfxhip.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gnymnccek.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gsbgxjxng.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gkauaotgi.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gqyyqasme.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/glahsqwjy.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gfizcbdsx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gpabektjg.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/giocdttde.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gtgffwlnc.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gxclngvyh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gsdkpbplt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gqiiduumc.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/guaozleiw.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gsjtgbkzs.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gixyzuygf.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gumjnuqlg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gzndcjuzd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gqiidauni.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gmroldnxw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gkzxaicxw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gwfawftlq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gifasivlh.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmogtarkn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gadkuvukp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gtdcngnez.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/ghbemdsyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gknyplbdf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgtuvcfy.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gcaxxafrx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkutjmcjy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gwrovwyxn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnuussodc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/grsrjjqet.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gktzdnkxi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfxjdpnvn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjdycpakw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glapgsrvs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gofsqovtl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyguhgtet.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gccqeizzp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gktsacshc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gxmjyabgo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grthvigdm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdwntgyxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/grimgtabb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ghcniuklw.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gbdunylxd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/giafgbbny.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gpesdeijj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gayyehxeg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/grckbtfkm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gpjmaergk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gxkfmiige.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gibxcurhf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gritkesdx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gzbvywhjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gmhstbxjh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gnjoewgoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gvronttwx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzapptwy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gbnwkbscp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gcryeybed.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjhpqlrtd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gcbmqvdlt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gvegnjjai.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glecstiqf.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gvjzqgcmz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbrlpdvvx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gyihpouot.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gsbxmyrei.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gotnfexmk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gabotieom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gzudyxnfe.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnslxakdk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gwgyzdcnc.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gcfmniekf.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gyhzddwrn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gwuhgczmc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkzwcjaxl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnrouwxvu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gwdqhbusk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gsjkrrmig.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdfanupuh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnolmfypz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/glkbogfhc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gclxllsrl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/golfeyldp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gpdhjtdcu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gaoxsphsv.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gxeamwggs.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/grcnmtaar.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gpabubohu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gwsnchrlj.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gcedmcugc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvzylzikv.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gmgtswxhe.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyvzcqoki.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gngumcmni.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glnmddkfy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjhycywlt.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ghwqnusvj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvfnhmbwl.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gxavwrjnh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjrrgrjhd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gkljvaune.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmmmdrljv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gquszeosg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/geqdubfot.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gckpxskas.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gtuzlgkaf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gqtdgjfkc.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/grjreporo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/guzhdfdvc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gurcxfiyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gdmggvwtw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gtlikcycg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gdtmclcyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gvzuqkqqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gpsrfvxos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gsfkakwaj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gocjrxwpb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gojpfxchg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gwzhipeub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbvlqzqqt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gctxhtlco.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gefukzoem.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gtbraamis.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gyrhoizsx.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwjxjwagx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/glufvrwcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gdeekxjmi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/ghujeoqim.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gezxtoygj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gviftanny.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gttuwzmxb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gigtpwrly.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gvjldujml.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glgeemecb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gukmiyfrh.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/guernjldv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gslvpizpy.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gwvbzhcqz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gbhaspyen.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/groqhaacy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gnkrvslte.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gxpurwucu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/ghcwekwjd.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/geqtijzqj.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/goaaghnvt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ghqdvybqm.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gmwyhedoy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gmennfsis.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxsjonz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gslzstoqh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbhnlrrch.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gmqdryksm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gwqhodwcq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/ghxihxphg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/glyrshbkk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gpkwpfpsg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gvnsvtcaz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gzkehnhye.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gouboigvw.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gpdflmvhi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcziiwjzr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gdhpizxlf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/glnjmymba.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gwlbuhrtq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ghithmkuj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gqrqkblne.sHtML


<!-- 参考信息 -->